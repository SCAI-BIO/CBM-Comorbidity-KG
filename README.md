# CBM KG: A Comorbidity-Centric Knowledge Graph Uncovering Causal Pathomechanisms Between COVID-19 and Neurodegenerative Diseases 
a manually curated, comorbidity-centric, cause-and-effect knowledge graph that systematically represents the putative molecular and clinical associations between COVID-19 and neurodegenerative diseases

## Overview

- CBM KG comprises over 2,800 cause-and-effect or correlative relationships from 63 peer-reviewed publications, encoded in Biological Expression Language (BEL; https://bel.bio/) and implemented in a Neo4j graph database.
  
- It captures a diverse spectrum of multi-level interactions spanning viral entry mechanisms, neuroinflammatory cascades, blood-brain barrier disruption, and genetic risk factors, as well as convergent pathways such as oxidative stress and protein aggregation.

- By integrating a wide range of biological entities including proteins, genes, drugs, compounds, phenotypes, molecular and biological processes, pathologies, and clinical endpoints, as well as protein/gene variants, fragments, complexes, and post-translational modifications, the CBM KG delivers high-resolution biomedical information, enabling the construction of more informative causal chains that link molecular mechanisms to clinical outcomes.
  
- Each relationship in the graph is fully traceable, supported by evidence statements from the source literature to ensure transparency and reproducibility.
  
- As a significant outcome of the collaboration within the EU-funded COMMUTE project (www.commute-project.eu), the CBM KG is publicly accessible for querying, extension, hypothesis generation, and functional interpretation of experimental data aimed at unraveling the molecular and cellular basis of the putative comorbidity between COVID-19 and neurodegenerative diseases.

![WP2_KG_figure](https://github.com/user-attachments/assets/723f34f8-0f54-4670-af44-9d50a2b5267b)

## Repository Contents

- `bel_files/`: Contains `.bel` and `.json` files for each publication in the corpus, detailing the curated relationships.
- `cbm-kg_shared-mechanisms/`: Includes `.cypher` and `.graphml` files representing shared disease mechanisms.
- `CBM_Comorbidity_KG.cys`: Cytoscape session file for visualizing the knowledge graph and shared mechanisms.
- `cbm-kg-070425.cypher`: Cypher file containing the graph structure and data for the CBM Knowledge Graph.
- `pmid.csv`: List of PubMed IDs corresponding to the curated literature sources.
- `README.md`: This documentation file.

## Getting Started

To explore the knowledge graph:

1. **Visualize with Cytoscape:**
   - Install [Cytoscape](https://cytoscape.org/) (version 3.10.2 or later).
   - Launch Cytoscape and open the `CBM_Comorbidity_KG.cys` session file by by navigating to **File -> Open Session**.
2. **Import into Neo4j:**
   - Install [Neo4j](https://neo4j.com/).
   - Execute the following command to import the `cbm-kg-070425.cypher` file:
     ```bash
     /path/to/neo4j/bin/cypher-shell -u <username> -p <password> -d <database> -f path/to/cbm-kg-070425.cypher
     ```
     For more information on using `cypher-shell`, refer to the [Neo4j Cypher Shell documentation](https://neo4j.com/docs/operations-manual/current/tools/cypher-shell/).


