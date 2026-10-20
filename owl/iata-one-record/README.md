ONE Record Ontology (the data model), by IATA. Version 3.3 RC1, ontology IRI `https://onerecord.iata.org/ns/cargo`. https://www.iata.org/one-record/

Downloaded on 2026-10-20 from https://raw.githubusercontent.com/IATA-Cargo/ONE-Record/2445a2b05087bf0bbdfba3bf76b9a8702edefd76/working_draft/ontology/IATA-1R-DM-Ontology.ttl

It imports the ONE Record code lists, which are in the `iata-one-record-codes` folder. The `owl:imports` in the file points at a `raw.githubusercontent.com` URL on the `master` branch rather than at the code lists' ontology IRI (`https://onerecord.iata.org/ns/code-lists`).

Note that many properties here have no `rdfs:domain`. Where a domain is meant, it is often only written as an annotation, for example `owl:comment "Domain :BookingTimes"@en` on `:totalTransitTime`.

# Copyright

Copyright (c) 2025 IATA-Cargo. Licensed under the MIT license: https://opensource.org/licenses/MIT. The license is in the LICENSE file of the repository, not in the ontology file itself.

# Changes

The file was converted from Turtle to N-Triples with rdflib. The triples are unchanged (same triple count before and after, and the graphs are isomorphic). The result is gzip-compressed.
