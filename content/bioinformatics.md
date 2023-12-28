+++
title = "Bioinformatics"
date = 2023-12-26T20:39:07-06:00
name = "Manuel Aguilar"
+++

Contributed to a bioinformatics team at the university as part of undergraduate research.
With a background in computer science, I leveraged programming skills to learn and apply computational methods in bioinformatics, despite lacking prior experience in the field.

### Initial Research

Contributed to a bioinformatics research group at [UTEP’s School of Pharmacy](https://github.com/sirimullalab), specializing in drug discovery. 
Established infrastructure for group members to access data from CSV, MySQL, and NoSQL databases.
Developed visualizations from computed results using a set of protein and gene names or identifiers. The primary objective was to investigate the subcellular location of specific drugs.

#### Project: Knowledge Graph for Drug Discovery

Created a Neo4j knowledge graph by integrating bioinformatics data from MySQL, CSV, and JSON sources, facilitating organized data representation based on common elements across sources.

* ChEMBL
    * type: MySQL
* Chebi 
    * type: MySQL
* Metabolomics Workbench
    * type: CSV, REST-API

The objective was to construct a Neo4j knowledge graph from processed data in diverse formats.
This involved consolidating the data through common elements in each source to generate machine learning datasets with cross-referenced matches.

![chemical-knowledge-graph-1](/RadialEmbedding.png)

#### Project: Subcellular location for genes.

Utilized the [HubMap Consortium portal](https://portal.hubmapconsortium.org/) to obtain data pinpointing the cellular locations reported by samples in each organ.

![violinplot](/violinplot.png)
![heatmap-RNA](/heatmap-RNA.png)
![heatmap-ATAC](/heatmap-ATAC.png)

#### Project: Drug similarity calculations

Utilizing an NCATS [repository](https://github.com/ncats/neo4covid19), established a Neo4j database housing COVID-19 data, specifically focusing on protein-to-protein interactions involving pathogens and host proteins.
Integrated new drug samples akin to existing data from NCATS, linking them to the pathogen protein. Computed similarity in SMILES using the Tanimoto coefficient.

| Starting Graph                               | Introduced Drugs                                                                       | Computed Graph                                                    |
|----------------------------------------------|----------------------------------------------------------------------------------------|-------------------------------------------------------------------|
| ![neo4covid-graph.png](/neo4covid-graph.png) | ![neo4covid-neo4covid-no-connect-graph.png](/neo4covid-neo4covid-no-connect-graph.png) | ![neo4covid-neo4covid-graph.png](/neo4covid-neo4covid-graph.png)  |

![heatmap.png](/heatmap.png)

| Bar Chart                     | Histogram KDE                                          |
|-------------------------------|--------------------------------------------------------|
| ![perospirone_barplot.png](/perospirone_barplot.png) | ![perospirone_histplot.png](/perospirone_histplot.png) |

### Current Interests

Researching novel computing methods for the advancement of computing techniques in bioinformatics. 

#### Project: Chat-GPT conversational agent for UniProt 

A [dash application](https://github.com/manguilar22/langchain-dash-app) to conversate with Chat-GPT on gene and protein entries from the [Uniprot](https://www.uniprot.org/) knowledge base.
Context is given to Chat-GPT using a Retreival Augmented Generation (RAG) to enhance responses by providing context beforehand.
Redis is used as the main database and computing platform for aggregated data retrieved through a REST-API.   

![uniprot-demo.gif](/uniprot-demo.gif)