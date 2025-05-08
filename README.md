# CBM KG: A Comorbidity-Centric Knowledge Graph Uncovering Causal Pathomechanisms Between COVID-19 and Neurodegenerative Diseases 
a manually curated, comorbidity-centric, cause-and-effect knowledge graph that systematically represents the putative molecular and clinical associations between COVID-19 and neurodegenerative diseases

## Overview

- CBM KG comprises over 2,800 cause-and-effect or correlative relationships from 63 peer-reviewed publications, encoded in Biological Expression Language (BEL; https://bel.bio/) and implemented in a Neo4j graph database.
  
- It captures a diverse spectrum of multi-level interactions spanning viral entry mechanisms, neuroinflammatory cascades, blood-brain barrier disruption, and genetic risk factors, as well as convergent pathways such as oxidative stress and protein aggregation.

- By integrating a wide range of biological entities including proteins, genes, drugs, compounds, phenotypes, molecular and biological processes, pathologies, and clinical endpoints, as well as protein/gene variants, fragments, complexes, and post-translational modifications, the CBM KG delivers high-resolution biomedical information, enabling the construction of more informative causal chains that link molecular mechanisms to clinical outcomes.
  
- Each relationship in the graph is fully traceable, supported by evidence statements from the source literature to ensure transparency and reproducibility.
  
- As a significant outcome of the collaboration within the EU-funded COMMUTE project (www.commute-project.eu), the CBM KG is publicly accessible for querying, hypothesis generation, and functional interpretation of experimental data aimed at unraveling the molecular and cellular basis of the putative comorbidity between COVID-19 and neurodegenerative diseases.

![WP2_KG_figure](https://github.com/user-attachments/assets/723f34f8-0f54-4670-af44-9d50a2b5267b)

## Repository Contents

- `bel_files/`: Contains `.bel` and `.json` files for each publication in the corpus, detailing the curated relationships.
- `cbm-kg_shared-mechanisms/`: Includes `.cypher` and `.graphml` files representing shared disease mechanisms.
- `CBM_Comorbidity_KG.cys`: Cytoscape session file for visualizing the knowledge graph and shared mechanisms.
- `cbm-kg-070425.cypher`: Cypher file containing the graph structure and data for the CBM Knowledge Graph.
- `pmid.csv`: List of PubMed IDs corresponding to the curated literature sources.
- `README.md`: This documentation file.


