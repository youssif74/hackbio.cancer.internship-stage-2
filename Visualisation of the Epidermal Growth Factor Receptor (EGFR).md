**Visualisation of the Epidermal Growth Factor Receptor (EGFR)**  
 Author: Jana (@JanaMoussa.0), Habiba (@pop-12),Youssif (@youssif74), Jackline (@jackeywes).

The Epidermal Growth Factor Receptor (EGFR) is a transmembrane glycoprotein  involved in cellular processes like growth, proliferation, and differentiation. EGFR, a member of the ErbB family, plays a pivotal role in signalling pathways such as MAPK, PI3K/Akt, and JAK/STAT, influencing cell behaviour in both physiological and pathological conditions.

**Structure of EGFR**

EGFR consists of 1,186 amino acids. Its extracellular region has four distinct domains (I-IV) for ligand binding. Upon epidermal growth factor (EGF) interaction, receptor dimerization occurs, bringing the cytoplasmic tyrosine kinase domains closer for autophosphorylation and activation of downstream pathways.

**Role in Cancer**

Overexpression or mutations in EGFR can lead to uncontrolled cell proliferation. Such mutations often result in constitutive receptor activation, contributing to tumorigenesis

**The Visualisation Steps**

1. **Selection of Protein:** Crystal structure of the Human Epidermal Growth Factor Complex and Receptor Extracellular Domains (PDB ID: 1IVO) \[[https://doi.org/10.2210/pdb1IVO/pdb](https://doi.org/10.2210/pdb1IVO/pdb)\]  
2. **Structure Retrieval:** Downloaded the protein structure from the Protein Data Bank (PDB).  
3. **Homology Modeling:** Performed using SWISS-MODEL.  
4. **AlphaFold Modeling:** Generated the protein model using AlphaFold.  
5. **Visualisation:** Analysed the protein structures using PyMOL.
6.![Models Image](https://raw.githubusercontent.com/jana-glitch/hackbio.cancer.internship/main/image%20models%20white.png)

7. **Comparison:** Compared the models from SWISS-MODEL (colour-coded in green) and AlphaFold (colour-coded in blue).  
8. **Analysis:** Analysed protein features and confirmation generated by the models.

**Features of the Protein's Structure**

1. Ligands: (visualised and coloured in red).  
   * 2 x NAG  
   * 1 x NAG-NAG
   * ![Ligands Image](https://raw.githubusercontent.com/jana-glitch/hackbio.cancer.internship/main/ligands%20white.png)

2.  Active Sites: Tyrosine Kinase Domain:  
   * Location: The active site is in the C-terminal region of EGFR
   ![Active Site Image](https://raw.githubusercontent.com/jana-glitch/hackbio.cancer.internship/main/active%20site.jpg)

3. Binding Sites: Site 1 (Domain I), Site 2 (Domain III), Site 3 (Domain III)
4. ![Binding Site Image](https://raw.githubusercontent.com/jana-glitch/hackbio.cancer.internship/main/binding%20site.jpg)

5. Domains: Identified and colour-coded domains (FU and EGF) using PyMOL.
![Domains Image](https://raw.githubusercontent.com/jana-glitch/hackbio.cancer.internship/main/domains%20white.png)
 
6. Mutations: (coloured them in orange)  
   * Receptor Dimerization Interface Mutations:  
     * R285S: Reduction in bioactivity; R285Y had a negligible effect.  
     * R285S \+ Y251A or F263A: Near complete loss of activity.  
     * Y251A and F263A: Individual mutations had negligible effects.  
   * Domain II-III Interface Mutation:  
     * R405E: Abolished EGF-dependent ERK phosphorylation and high-affinity EGF binding, highlighting the importance of domain-domain interaction.
![Mutations Image](https://raw.githubusercontent.com/jana-glitch/hackbio.cancer.internship/main/mutations%20white.png)


**Protein Modeling Techniques**

1. Homology Modeling with SWISS-MODEL: Uses template-based predictions by aligning target sequences with known structures. Accuracy depends on sequence identity and template quality.  
2. AlphaFold: Uses deep learning to predict protein structures from amino acid sequences without homologous templates.

**Comparison**

* Similarities: Both methods predict 3D protein structures from amino acid sequences.  
* Differences: Homology modelling requires known homologous structures, while AlphaFold does not. AlphaFold generally offers higher accuracy and faster predictions.

**Conformation Analysis: both models generated an agonist confirmation** (colour-coded 1Z9I purple, 1M17 yellow, 3KEX pink)

* AlphaFold Model:  
  * Agonist (1Z9I): RMSD \= 8.579  
  * Antagonist (1M17): RMSD \= 16.406  
  * Apo (3KEX): RMSD \= 12.536
  * ![Comparison Alpha Image](https://raw.githubusercontent.com/jana-glitch/hackbio.cancer.internship/main/comparison%20alpha.png)


* Homology Modeling (SWISS-MODEL):  
  * Agonist (1Z9I): RMSD \= 8.715  
  * Antagonist (1M17): RMSD \= 16.476  
  * Apo (3KEX): RMSD \= 12.696
  * ![Comparison Swiss Image](https://raw.githubusercontent.com/jana-glitch/hackbio.cancer.internship/main/comparison%20swiss.png)


**Conclusion**   
Despite apparent similarities, the SWISS-MODEL showed ligands while the AlphaFold model did not. Both techniques provide valuable insights into the protein structure, though AlphaFold generally offers superior accuracy.

**References**  
Ogiso, H., Ishitani, R., Nureki, O., Fukai, S., Yamanaka, M., Kim, J. H., … & Yokoyama, S. (2002). Crystal structure of the complex of human epidermal growth factor and receptor extracellular domains. *Cell, 110*(6), 775-787. [https://doi.org/10.1016/s0092-8674(02)00963-7](https://doi.org/10.1016/s0092-8674\(02\)00963-7)
