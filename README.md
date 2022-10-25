# SBOM and MBOM Essentials

## Definitions

In advance to the details some definitions on terminology is provided.

### Generic

#### Asset
An Asset is concept or unit of value. Here, either a Software or Hardware Asset. Assets may also include documents
and data.

#### Bill of Materials (BOM)

A Bill of Materials is listing details of an asset in a human- or
machine-machine fashion. BOMs can contain hierarchy or relationship information.

### Software

#### Software Asset
A Software Asset is an Asset consisting of Software. Software Assets are for example:
* Software archives for distribution
* Software Container Images
* Virtual Machine Images

#### Software Artifacts / Artifacts

Substructures or details of a Software Asset are Software Artifacts or just
Artifacts.

#### Software Bill of Materials (SBOM)

A human- or machine-readable BOM lists Software Artifacts providing details on one or more Software Assets.

### Hardware 

#### Hardware Asset
A Hardware Asset is an Asset consisting of Hardware. Hardware assets are for example:
* Devices (stationary devices and equipment, mobile devices, robots)
* Server appliances

#### Hardware Parts / Parts

Details of Hardware Asset are Hardware Parts or just Parts.

#### Manufacturing Bill of Materials (MBOM)

A human- or machine-readable BOM lists Hardware Parts detailing on one or more Hardware Assets. An MBOM consists 
of all Hardware Parts required to build a complete and shippable product.

*Background:
The term MBOM is defined in early ANSI/ISA-95 (IEC 62264-1 Models and Terminology).
Often also the term Hardware Bill of Materials (HBOM) is used.*

## SBOM Essentials

To outline SBOM essentials the different use cases around SBOMs are inspected.

### SBOM Use Cases

* [Creating an SBOM from Software Assets](docs/01-asset-to-sbom.md)
* [Creating Software Documentation based on an SBOM](docs/02-sbom-to-annex.md)
* [Monitoring Vulnerabilities using an SBOM](docs/03-sbom-to-dashboard.md)
* [Reporting Vulnerabilities using an SBOM](docs/04-sbom-to-report.md)
* [Scanning Software based on an SBOM](docs/05-sbom-to-scan.md)

### Implementations

The following projects define SBOM data models and format definition:

* [SPDX](https://spdx.github.io/spdx-spec/)
* [CycloneDX](https://cyclonedx.org/)
* [SWID](https://www.iso.org/standard/65666.html)
* [{metæffekt} Inventory](https://github.com/org-metaeffekt/metaeffekt-core)
* [ORT Analyser YAML/JSON Output](https://github.com/oss-review-toolkit/ort)

## MBOM Essentials

MBOM creation can usually not be automated. MBOMs - in the best case - can be exported from hardware or mechanical 
design tools.

### HBOM Use Cases

Based on an MBOM the following use cases are anticipated:

* Linking the MBOM to SBOMs. Specifically with respect to software placed on the hardware (firmware, loadable 
  application code)
* Monitoring Vulnerabilities of Hardware and in correlation with Software.

*Background:
Some vulnerabilities only surface in combination with hardware. E.g., a specific hardware running a specific software 
configuration.*

## External References

* [NTIA Software Bill of Materials](https://ntia.gov/SBOM) - very complete materials on SBOMs.
* [Awesome SBOM](https://github.com/awesomeSBOM/awesome-sbom) - Collection of various resources around SBOMs.

# License
Creative Commons Attribute-NoDerivatives 4.0 International
- Copyright (c) 2022 Karsten Klein, metaeffekt GmbH
- Copyright (c) 2022 Thomas Schulte, metaeffekt GmbH
