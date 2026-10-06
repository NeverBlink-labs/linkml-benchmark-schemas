# RDFS vocabularies

A collection of real-world vocabularies written in RDFS (`rdfs:Class`, `rdf:Property`, `rdfs:subClassOf`, `rdfs:domain`, `rdfs:range` and annotations) under open licenses, used to test converting RDFS to LinkML and back. Some use a few OWL terms on top: Schema.org and DC terms map their terms to others with `owl:equivalentClass` and `owl:equivalentProperty`, and several have an `owl:Ontology` header. The files are taken as published and converted to gzip-compressed N-Triples, without other changes to their content. Each folder holds one data file, `main.nt.gz`. See the README in each folder for the source, license and download details.

| Folder | Vocabulary | Domain | Triples | License |
|---|---|---|---:|---|
| `shacl` | SHACL vocabulary (W3C) | data validation | 1,128 | W3C Software and Document License |
| `reproschema` | ReproSchema (ReproNim) | research assessments | 351 | Apache 2.0 |
| `schemaorg` | Schema.org 30.1 | general purpose | 17,515 | CC BY-SA 3.0 |
| `dcterms` | DCMI Metadata Terms | metadata | 700 | CC BY 4.0 |
| `dcelements` | Dublin Core Metadata Element Set 1.1 | metadata | 107 | CC BY 4.0 |
| `dcmitype` | DCMI Type Vocabulary | metadata | 89 | CC BY 4.0 |
| `geo-wgs84` | WGS84 Geo Positioning (W3C) | geographic positions | 33 | W3C Software and Document License |
| `web-annotation` | Web Annotation Vocabulary (W3C) | annotations | 334 | W3C Software and Document License |
| `hydra` | Hydra Core Vocabulary (W3C Hydra CG) | web APIs | 469 | CC BY 4.0 |

`shacl` and `reproschema` come from the test resources of LinkML's [schema-automator](https://github.com/linkml/schema-automator). `dcat3` in `../owl` imports `dcterms`.
