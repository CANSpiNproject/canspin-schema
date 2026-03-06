![version](https://img.shields.io/badge/version-1.0.0-blue)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

# canspin-schema
CANSpiN repository for the XML-TEI schemas used for the corpus files

There are two schemas:
- one for the text files of the literary works themselves
- one for an XML-TEI file listing all the authors of the works in the corpus

For each of the schemas, an ODD file is provided and an RNG file. The latter can be linked to from the XML-TEI files to validate them:

``` 
<?xml-model href="https://raw.githubusercontent.com/CANSpiNproject/canspin-schema/refs/heads/main/tei_canspin_texts.rng" type="application/xml" schematypens="http://relaxng.org/ns/structure/1.0"?>
<?xml-model href="https://raw.githubusercontent.com/CANSpiNproject/canspin-schema/refs/heads/main/tei_canspin_texts.rng" type="application/xml"
	schematypens="http://purl.oclc.org/dsdl/schematron"?>
``` 

The first link is for checking the XML elements and attributes, the second link to check for additional rules in schematron.

In addition to the schema files, there are two example files (one for a literary text and the other one for an author-file).

The schema for the texts is kept simple and was inspired by the ELTeC schema, level 0: https://github.com/COST-ELTeC/Schemas
