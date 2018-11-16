Financial Report Vocabulary (FR)
=================================

FR is a simple Ontology defined with [OWL](https://www.w3.org/TR/owl2-primer/) to describe a generic financtial report.

It captures different perspectives of a report data like historical trends, cross-department and component breakdown . 

FR is an extension ofthe [W3C RDF Data Cube Vocabulary](https://www.w3.org/TR/vocab-data-cube)

FR is inspired by the [Financial Report Semantics and Dynamics Theory](doc/Theory-2017-06-26.pdf). 

The main concept in FR is the **Fact** that is an observation of a money amount described with some attributes: a reference period (e.g. year 2018), etc, etc. Facts  are grouped in **Component**s also described with a concept in a taxonomy, the set of all components define a **FinancialReport** .

Every fact and every component is strictly related to a taxonomy of **Concepts** . For defining Concepts FR reuses the skos vocabulary. 

Some fact properties, if not explicitly defined, can be inherited form the financial report attributes, that provide a default. Also the groups hierarchy can be inferred from the concepts taxonomy structure.

![FR UML diagram](doc/uml-diagram.png)

## Editing the FR ontology

FR is expressed in a [owl file](fr.owl) serialized as RDF xml. You can edit the file by hand or using [Protégé](https://protege.stanford.edu/)

## License

The FR ontology is available under the Creative Commons Attribution 3.0 license.