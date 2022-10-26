# Monitoring Vulnerabilities using an SBOM

Based on SBOMs outputs supporting vulnerability monitoring and vulnerability assessment can be generated:

![Vulnerability Dashboards created from SBOM](figures/03-sbom-to-dashboard.svg)

This process is configured to produce different dashboards for different assessment contexts.

See key aspects below.

## Vulnerability Assessment Context

The assessment of vulnerabilities depends on the integration and deployment context. A vulnerability within a single
Software Artifact may impose a critical issue in one context while being insignificant in another context.

## Vulnerability Assessment Process

Vulnerability assessment is not trivial. It is subject to a dedicated process by specific roles and oftern requires 
in-depth integration and technical backgrounds.

## Capturing Reusable Vulnerability Assessment Results

Vulnerability assessment for different assets in different configurations need to organized in reusable fashion. To 
foster reuse of assessment results additional concepts are required.

## Vulnerability Reassessment

Vulnerability assessments represent a snapshot at a given time. The boundary conditions may
however change (changes to vulnerability details, changes to the software). Therefore, assessment 
reviews need to be conducted regularly. 

Vulnerability Reassessment activities need to be captured by the aforementioned Vulnerability 
Assessment Process.

## Excessive Vulnerabilities

Vulnerability monitoring and assessment may face a significant amount of vulnerabilities to process. Techniques are 
required to enable bulk vulnerability processing and skim the relevant threats for prioritization.


Back to [SBOM Essentials](../README.md#SBOM-Essentials).