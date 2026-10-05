# OWL ontologies

A collection of real-world OWL and RDFS ontologies under open licenses, used to test converting OWL to LinkML and back. The files are taken as published and converted to gzip-compressed N-Triples, without other changes to their content. Each folder holds one data file, `main.nt.gz`. See the README in each folder for the source, license and download details.

| Folder | Ontology | Domain | Triples | License |
|---|---|---|---:|---|
| `sosa` | SOSA (W3C/OGC) | sensors and observations | 345 | W3C Software and Document License |
| `ssn` | SSN (W3C/OGC), imports SOSA | sensors and observations | 520 | W3C Software and Document License |
| `prov-o` | PROV-O (W3C) | provenance | 1,146 | W3C Software and Document License |
| `shacl` | SHACL vocabulary (W3C) | data validation | 1,128 | W3C Software and Document License |
| `reproschema` | ReproSchema (ReproNim) | research assessments | 351 | Apache 2.0 |
| `foaf-snippet` | An excerpt of FOAF, from schema-automator's tests | people | 13 | CC BY 1.0 |
| `foaf` | FOAF 0.99 | people | 631 | CC BY 1.0 |
| `skos` | SKOS vocabulary (W3C) | knowledge organization | 252 | W3C Software and Document License |
| `dcat3` | DCAT 3 (W3C) | data catalogs | 1,695 | CC BY 4.0 |
| `org` | Organization Ontology (W3C) | organizations | 748 | PDDL 1.0 |
| `time` | OWL-Time (W3C/OGC) | time | 1,296 | CC BY 4.0 |
| `saref` | SAREF core (ETSI) | smart appliances, IoT | 1,324 | BSD-3-Clause (ETSI) |
| `gist` | gist core 14.1.0 (Semantic Arts) | upper ontology for business | 2,317 | CC BY 4.0 |
| `d3fend` | D3FEND (MITRE) | cybersecurity | 43,643 | MIT |
| `fabio` | FaBiO (SPAR), imports FRBR | publishing | 3,390 | CC BY 4.0 |
| `frbr` | FRBR core (SPAR) | bibliographic records | 1,169 | CC BY 4.0 |
| `cito` | CiTO (SPAR) | citations | 972 | CC BY 4.0 |
| `fibo-agents` | FIBO FND Agents (EDM Council) | finance | 28 | MIT |
| `fibo-annotation-vocabulary` | FIBO FND Annotation Vocabulary (EDM Council) | finance | 65 | MIT |
| `commons-annotation-vocabulary` | OMG Commons Annotation Vocabulary | metadata | 196 | MIT |
| `commons-classifiers` | OMG Commons Classifiers | classification | 72 | MIT |
| `commons-collections` | OMG Commons Collections | collections | 113 | MIT |
| `commons-designators` | OMG Commons Designators | names and identifiers | 116 | MIT |
| `commons-text-datatype` | OMG Commons Text Datatype | text | 38 | MIT |
| `bfo` | BFO 2020 core | upper ontology (OBO) | 1,015 | CC BY 4.0 |
| `ro-core` | OBO Relation Ontology core | relations (OBO) | 519 | CC0 1.0 |
| `schemaorg` | Schema.org 30.1 | general purpose | 17,515 | CC BY-SA 3.0 |
| `dcterms` | DCMI Metadata Terms | metadata | 700 | CC BY 4.0 |
| `odrl` | ODRL 2.2 (W3C) | rights and policies | 2,157 | W3C Software and Document License |

The first six come from the test resources of LinkML's [schema-automator](https://github.com/linkml/schema-automator).

Several import others in the collection, so that importing with the imports mapped to their own schemas can be tested: `ssn` imports `sosa`; `dcat3` imports `dcterms`, `skos` and `prov-o`; `fabio` imports `frbr`; and the FIBO and Commons modules import each other, four levels deep from `fibo-agents`.
