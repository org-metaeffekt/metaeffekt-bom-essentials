# Creating Software Documentation based on an SBOM

Based on an SBOM further compliance documents can be created: 

![Software Annex created from SBOM](figures/02-sbom-to-annex.svg)

SBOMs may include references to external files. Nevertheless, for a comprehensive software
documentation the above details are recommended to be aggregated in one archive, that is delivered
with the Software Asset. In the terminology applied by {metæffekt} this archive is called the
Software Asset Annex.

It is important to note, that an SBOM as such does not necessarily address compliance requirements and obligations from the used 
licenses.

## Requirements for Compliance

* Effective license determination
* Corresponding License Text and License Notice files
* Justification with respect to copyleft and other reciprocal effects  
* Written offer with respect to source code availability
* Compulsory statements regarding individual license obligations
* Source Code (depending on source code handling)

As such the Software Asset Annex contains to its full extend:
* A PDF document for human readability containing
    * Describing the project/product/solution in brief
    * Providing information on compliance policies (source code handling, import/export)
    * A List of all Assets within the project/product/solution
    * Lists of Artifacts with detailed licensing information (associated and effective) for each Asset
    * Uniform license overviews (both on asset- and on artifact-level)
    * Compulsory statements per artifact/license.
    * A context-sensitive glossary of terms
* The actual license files (some license files may only be referencing placeholders in case the license 
  is confidential)
* License notice files or detailed license attribution (copyright, copying) files  
* Source code of artefacts that have been identified to be shared within the Software Asset Annex
  

Back to [SBOM Essentials](../README.md#SBOM-Essentials).