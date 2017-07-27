## Content

A set of Noark 5.3 extractions which were validated using version 0.2.0 of the [noark-extraction-validator tool](https://github.com/documaster/noark-extraction-validator). Each directory contains:

* extraction: a Noark 5.3 extraction
* reports: one or more set of reports produced by the noark-extraction-validator tool
* README: a README file that provides a brief description about the included extraction

### Valid extractions:

The following directories contain valid Noark 5.3 extractions:

* valid-case-archive
* valid-mixed-archive

### Invalid extractions:

The following directories contain invalid Noark 5.3 extractions:

* duplicate-system-ids
* ignore-non-compliant-xml
* incomplete-structure
* invalid-pdfa
* missing-loependeJornal-references
* missing-optional-journals
* tampered-extraction

## Disclaimer

You will notice one thing that all validation reports have in common. That is, all reports indicate an issue with the change log. The reason is that the Noark 5.3 standard does not define a systemID field for DocumentObjects which means that the entity does not have a unique global identifier. The system that produced these extractions, however, does implement such a field to overcome this shortcoming. As a result, noark-extraction-validator issues a warning that there are entities (DocumentObjects) that are referred to in endringslogg.xml, but not found in arkivstruktur.xml.
