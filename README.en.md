**Scegli la lingua / Choose your language**

[![Italiano](https://img.shields.io/badge/italiano-blue?style=for-the-badge)](README.md)
[![English](https://img.shields.io/badge/english-red?style=for-the-badge)](README.en.md)

# Semantic resources for the *ArCo4Archives* project

[![Arco4Archives](./img/arco4archives.jpeg "Portal of sources for the history of the Italian Republic.")](https://icar.cultura.gov.it/standard/standard-san/arco4archives)

## Introduction

This repository hosts the **ontology**, the **controlled vocabularies**, and the **external semantic alignments** that constitute the semantic assets designed and developed within the initiative for the creation of a network of ontologies **Arco4Archives**: [ICAR archival standards: Arco4Archives](https://icar.cultura.gov.it/standard/standard-san/arco4archives).

ICAR has set itself the goal of enriching interoperability tools through the development of a network of ontologies (ArCo4Archives) to represent the archival domain, extending the **ArCo - Architettura della conoscenza** ontologies developed by ICCD and CNR together with the University of Bologna, and serving as a reference model for the production and publication of the archives' **knowledge graph** based on data from the [SIA (Sistema Informativo Archivistico)](https://icar.cultura.gov.it/sistemi-e-portali/archivi-nazionali/sia).

The reference model on which the ArCo4Archives ontologies have been developed is the ICAR Import2 archival description interoperability standard.
The project's goal is to create an ontological model to produce structured data in a semantic **knowledge graph**, following the Linked Open Data paradigm.

### The Project

[Arco4Archives](https://portalefontirepubblicaitaliana.cnr.it/) is a project coordinated by **ICAR** and produced by [**BUP srl**](https://www.bupsolutions.com/) and the **Istituto di Scienze e Technologie della Cognizione del CNR** - **[ISTC-CNR](https://www.istc.cnr.it/)**, aimed at building an interoperable semantic infrastructure based on open standards for modeling the information catalogued within the SIA system. Starting from the requirements of the ICAR Import2 formats and the system's data model, it was possible to model the representation of archival resources and their hierarchical and containment relationships, the representation of contents, their arrangement, and their interconnections with people, organizations, institutions, and their development over time.

## Repository structure

This repository is organized to support the entire lifecycle of the ontologies, from design to publication and maintenance. The ontology modules follow a modular approach and an explicit versioning system, aimed at ensuring backward compatibility and stability of the URIs of the elements that make up the network of ontologies.

```text
assets/
└── controlled-vocabularies/     # Reference for controlled vocabularies
    ├── [vocabulary-name]/       # Individual vocabularies 
    │   └── vocab.ttl            # Vocabulary distributions
└── ontologies/                  # Reference for ontologies defined in OWL
    ├── [module-name]/           # 'archival-resource' module
    │   ├── v0.1/                # Version-specific snapshot
    │   ├── ...
    │   ├── latest/              # Copy of the latest stable version
    │   │   ├── module.owl       # OWL RDF/XML serialization 
    │   │   ├── module.rdf       # RDF/XML serialization
    │   │   └── module.ttl       # Turtle serialization
    │   └── ontology-diagrams/             
	│       ├── module.graphml   # Graffoo diagram source
	│       ├── module.jpeg      # Graffoo diagram
	│       ├── ...
	│       ├── module.jpeg      # Graffoo diagram
	│       ├── ...
    └── ...
    └── ...
```

📂 [`ontologies/`](./ontologies)

This is the core of the repository and contains the **ontology module** produced. The module is organized by version. The `latest/` directory always contains the most recent stable version of the ontology, made available in different RDF serializations (e.g. Turtle and RDF/XML).

For each module, graphical representations are also provided, produced as [Graffoo](https://essepuntato.it/graffoo/) diagrams. These diagrams formally describe the classes, properties, and axioms of the ontologies, and constitute the main visual reference for understanding the conceptual structure of the models.

## The network of ontologies

The portal's ontological network is designed as a modular set of interconnected ontologies, able to ensure a clear separation of the represented domains while maintaining a unified view of the different areas of knowledge and their domain data. The semantic architecture adopts a multilevel approach, balancing the modeling of specific domain knowledge with interoperability across different domains and the reuse of existing ontologies.

### Archival resource ontology - ArCo4Archives

**URI**: [`https://w3id.org/arco/archives/ontology/archival-resource`](https://w3id.org/arco/archives/ontology/archival-resource)

![Graphical representation of the archival resources ontology](https://github.com/IstitutoCentraleArchivi-ICAR/ICAR-Semantics/blob/main/assets/ontologies/archival-resource/v0.1/ontology-diagrams/ArchivalResource.jpg "Organizations ontology")

The *Archival Resource Ontology* (a-arc)
is the ArCo module for representing the archival domain. It expands and extends the [ArCo ontology network](https://github.com/ICCD-MiBACT/ArCo).

#### Archival resources
Starting from the semantic structure of the cultural heritage domain, the module extends and specializes various national models to accommodate the specificity of the archival domain. The superclass `a-arc:ArchivalResource` represents a generic resource that can be specialized into the three fundamental classes of the domain: `a-arc:ArchivalResourceSet`, the archival complex, `a-arc:ArchivalUnit`, the archival unit, and `a-arc:ArchivalItem`, the documentary unit.

#### Responsibility
In terms of extension, ArCo's `a-cd:Responsibility`, which represents an agent's responsibility for the creation of an asset, is extended with `a-arc:ArchivalResponsibility`, which presupposes the two foundational roles in the archival context: `a-arc:ArchivalCreator` and `a-arc:ArchivalHolder`.

#### Agents
![Graphical representation of the archival resources ontology](https://github.com/IstitutoCentraleArchivi-ICAR/ICAR-Semantics/blob/main/assets/ontologies/archival-resource/v0.1/ontology-diagrams/FormalOrganization.jpg "Organizations ontology")

Agents are specialized into persons, families, and organizations. A specialized model is applied for `a-arc:FormalOrganization`, with an effort to represent institutional profiles `a-arc:InstitutionalProlie`, also typed over time, and the historical-institutional context of provenance `a-arc:HistoricalOrInstitutionalContext`.

![Graphical representation of the modeling of persons](https://github.com/IstitutoCentraleArchivi-ICAR/ICAR-Semantics/blob/main/assets/ontologies/archival-resource/v0.1/ontology-diagrams/NaturalPerson.jpg)

`a-arc:NaturalPerson` entities, with their attributes over time (professions, qualifications, and titles of nobility), are represented following the national CPV ontology of OntoPiA, reusing ArCo for the semantic blocks already captured by the cultural domain and specializing entities to accommodate the verticals of the domain.

### Controlled vocabularies
In support of the ontological scaffolding, controlled vocabularies are produced and defined, which define the domain's classifying concepts. The controlled vocabularies are formalized in LOD according to the [**Simple Knowledge Organization System (SKOS)**](https://www.w3.org/TR/skos-reference/) standard.

## Namespace and base URI

To ensure persistence, stability, and long-term resolution of the URIs, the project uses the [w3id](https://w3id.org/) infrastructure, maintaining the following base URI:

* `https://w3id.org/arco/archives/`

This base URI is further organized into dedicated *namespaces* for ontologies and semantic resources, such as controlled vocabularies:

* Ontologies: `httphttps://w3id.org/arco/archives/ontology/`
* Controlled vocabularies: `httphttps://w3id.org/arco/archives/controlled-vocabulary/`

## License

![CC BY 4.0](https://licensebuttons.net/l/by/3.0/88x31.png)

The ontology modules and related documentation are released under the [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) license.
