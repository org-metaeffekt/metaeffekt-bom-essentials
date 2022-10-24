# SBOM and MBOM Essentials

## Definitions

### Assets, Software Assets and Hardware Assets
An Asset is concept or unit of value. Here, either a Software or Hardware Asset.

### Software Asset
A Software Asset is an Asset consisting of Software. Software Assets are for example:
* Software archives for distribution
* Software Container Images
* Virtual Machine Images

### Hardware Asset
A Hardware Asset is an Asset consisting of Hardware. Hardware assets are for example:
* Devices (stationary devices and equipment, mobile devices, robots)
* Server appliances

### Bill of Materials (BOM)

A Bill of Materials is a listing details of an asset in a human- or 
machine-machine fashion. BOMs can container hierarchy or relationship information.

### Software Artifacts / Artifacts

Substructures or details of a Software Asset are Software Artifacts or just 
Artifacts.

### Hardware Parts / Parts

Details of Hardware Asset are Hardware Parts or just Parts.

### Software Bill of Materials (SBOM)

A human- or machine-readable BOM lists Software Artefacts providing detail 
on one or more Software Assets.

### Manufacturing Bill of Materials (MBOM)

A human- or machine-readable BOM lists Hardware Parts detailing on one or 
more Hardware Assets. An MBOM consists all Hardware Parts required to build a 
complete and shippable product.

The term MBOM is defined in early ANSI/ISA-95 (IEC 62264-1 Models and Terminology).
Other refer to an Hardware Bill of Materials as HBOM.

## SBOM Essentials

To outline SBOM essentials the different use cases around SBOMs are inspected.

* [Creating an SBOM](docs/sbom-create.md)
* Creating Software Documentation using SBOMs
* Monitoring Vulnerabilities using SBOMs
* Creating Vulnerability Disclosure Reports using SBOMs

## Implementations

* SPDX
* CycloneDX
* SWID
* metæffekt Inventory
* ORT Analysis Output

### External References

* [NTIA Software Bill of Materials](https://ntia.gov/SBOM) - very complete materials on SBOMs.
