# SBOM and MBOM Essentials

## Definitions

In advance to the details definitions on terminology are provided.

### Generic

#### Asset
An Asset is concept or unit of value. Here, either a Software or Hardware Asset. Assets may also be documents
or data sets; content in general.

#### Bill of Materials (BOM)

A Bill of Materials is listing details of an asset in a human- or machine-readable fashion. BOMs can contain hierarchy 
or relationship information.

#### Supplier

The supplier is a person or legal entity that produces a Software or Hardware Asset. The supplier is the originator, 
creator, or manufacturer of an Asset.

#### Distributor

A distributor may distribute Software and Hardware Assets. The Software and Hardware Assets are not modified as such
and distributed "AS IS".

#### Vendor

A vendor is a supplier or distributor that acts in a commercial context / relationship with a consumer of an Asset.

### Software

#### Software Asset
A Software Asset is an Asset consisting of Software. Software Assets are for example:
* Software archives for distribution
* Software Container Images
* Virtual Machine Images

#### Software Artifacts / Artifacts

Substructures or details of a Software Asset are Software Artifacts or just Artifacts.

### Software Components

Software Components group Software Artifacts into a logical unit. Often these artifacts have consistent characteristics.

#### Software Bill of Materials (SBOM)

A human- or machine-readable BOM lists Software Artifacts providing details on one or more Software Assets.

### Hardware 

#### Hardware Asset
A Hardware Asset is an Asset consisting of Hardware. Hardware assets are for example:
* Devices (stationary devices and equipment, mobile devices, robots)
* Server appliances

A Hardware Asset may require software to operate (microcontroller programs, FPGA programs, operating systems and 
other software components).

#### Hardware Parts / Parts

Details of Hardware Asset are Hardware Parts or just Parts.

#### Hardware Bill of Materials (HBOM)

A human- or machine-readable BOM lists Hardware Parts detailing on one or more Hardware Assets. An HBOM consists 
primarily of all Hardware Parts required to build a complete and shippable product. In addition, the HBOM may also
refer to software and service information to refer to additional information.

*Background:
The term Manufacturing Bill of Materials (MBOM) is defined in early ANSI/ISA-95 (IEC 62264-1 Models and Terminology).
Recently the term Hardware Bill of Materials (HBOM) is used commonly. See also [CISA - A HBOM Framework for Supply Chain
Risk Management](https://www.cisa.gov/resources-tools/resources/hardware-bill-materials-hbom-framework-supply-chain-risk-management).*

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

## HBOM Essentials

HBOM creation can usually not be automated. HBOMs - in the best case - can be exported from hardware or mechanical 
design tools.

### HBOM Use Cases

Based on an HBOM the following use cases are anticipated:

* Linking the HBOM to SBOMs. Specifically with respect to software placed on the hardware (firmware, loadable 
  application code)
* Monitoring Vulnerabilities of Hardware and in correlation with Software.

*Background:
Some vulnerabilities only surface in combination with hardware. E.g., a specific hardware running a specific software 
configuration.*

## External References

* [NTIA Software Bill of Materials](https://ntia.gov/SBOM) - very complete materials on SBOMs.
* [Awesome SBOM](https://github.com/awesomeSBOM/awesome-sbom) - Collection of various resources around SBOMs.
* [Open CODE SPDX Conformance](https://gitlab.opencode.de/open-code/spdx-conformance) - Initial defintions regarding SBOMs by Open CoDE.
* [CISA - A Hardware Bill of Materials (HBOM) for Supply Chain Risk Management](https://www.cisa.gov/resources-tools/resources/hardware-bill-materials-hbom-framework-supply-chain-risk-management) - HBOM-centric framework.

# License
Creative Commons Attribute-NoDerivatives 4.0 International
- Copyright (c) 2022-2023 Karsten Klein, metaeffekt GmbH
- Copyright (c) 2022 Thomas Schulte, metaeffekt GmbH
