Financial Report Vocabulary (FR)
=================================

FR is a simple [OWL](https://www.w3.org/TR/owl2-primer/) vocabulary to describe a generic financial report.

FR vocabulary be used to capture different perspectives of a report data like historical trends, cross-department and component breakdown . 

FR extends the [W3C RDF Data Cube Vocabulary](https://www.w3.org/TR/vocab-data-cube) and it is inspired by the [Financial Report Semantics and Dynamics Theory](doc/Theory-2017-06-26.pdf). 

A **FinancialReport** is dataset that contains a tree of **Components*. The leaf components of such tree are **Facts**.
The **Fact** is an observation of a money amount described with some attributes that is reported in a **FinacialReport** dataset.

Fact and components SHOULD be related to one or more **Concept** in a  [SKOS vocabulary](https://www.w3.org/TR/skos-primer) taxonomy.

The following namespaces are used:

Prefix	        | Namespace	 | Description
--------------- | ------------------------------------------------- | ----------------
fr              | http://linkeddata.center/botk-fr/v1#              | this vocabulary
qb              | http://purl.org/linked-data/cube#                 | W3C RDF Data Cube Vocabulary
skos            | http://www.w3.org/2004/02/skos/core#              | the W3C SKOS vocabulary
time            | http://www.w3.org/2006/time#                      | the W3C ontology of temporal concepts
sdmx-code	    | http://purl.org/linked-data/sdmx/2009/code#	    | SKOS Concepts and ConceptSchemes for each COG defined code list
sdmx-dimension	| http://purl.org/linked-data/sdmx/2009/dimension#	| component properties corresponding to each COG concept that can be used as a dimension
sdmx-attribute	| http://purl.org/linked-data/sdmx/2009/attribute#	| component properties corresponding to each COG concept that can be used as an attribute
sdmx-measure	| http://purl.org/linked-data/sdmx/2009/measure#	| component properties corresponding to each COG concept that can be used as a measure


![FR UML diagram](doc/uml-diagram.png)

Some fact properties, if not explicitly defined, can be inherited form the financial report attributes, that provides a default. In some cases, the financial report components can be inferred from the concepts taxonomy structure.

For an usage example of FR vocabulary see [g0v fr-ap application profile](https://github.com/g0v-it/fr-ap)

## Editing the FR ontology

The namespace for FR terms is *http://linkeddata.center/botk-fr/v1#*

The suggested prefix for the FR vocabulary namespace is *fr*

FR is expressed in a [owl file](fr.owl) serialized as RDF xml. You can edit the file by hand or using [Protégé](https://protege.stanford.edu/)

## License

The FR ontology is available under the Creative Commons Attribution 3.0 license.
