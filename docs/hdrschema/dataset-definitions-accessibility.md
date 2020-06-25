# Accessibility Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/accessibility
```

Accessibility information allows researchers to understand access, usage, limitations, formats, standards and linkage or interoperability with toolsets.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## accessibility Type

`object` ([Accessibility](dataset-definitions-accessibility.md))

# Accessibility Properties

| Property                                | Type   | Required | Nullable       | Defined by                                                                                                                                                                                               |
| :-------------------------------------- | ------ | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [usage](#usage)                         | Merged | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-accessibility-properties-usage.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/accessibility/properties/usage")                              |
| [access](#access)                       | Merged | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-accessibility-properties-access.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/accessibility/properties/access")                            |
| [formatStandards](#formatStandards)     | Merged | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-accessibility-properties-formats-and-standards.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/accessibility/properties/formatStandards")    |
| [enrichmentLinkage](#enrichmentLinkage) | Merged | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-accessibility-properties-enrichment-and-linkage.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/accessibility/properties/enrichmentLinkage") |

## usage

This section includes information about how the data can be used and how it is currently being used


`usage`

-   is optional
-   Type: merged type ([Usage](dataset-definitions-accessibility-properties-usage.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-accessibility-properties-usage.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/accessibility/properties/usage")

### usage Type

merged type ([Usage](dataset-definitions-accessibility-properties-usage.md))

all of

-   [Untitled object in HDR UK Dataset](dataset-definitions-usage.md "check type definition")

## access

This section includes information about data access.


`access`

-   is optional
-   Type: merged type ([Access](dataset-definitions-accessibility-properties-access.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-accessibility-properties-access.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/accessibility/properties/access")

### access Type

merged type ([Access](dataset-definitions-accessibility-properties-access.md))

all of

-   [Untitled object in HDR UK Dataset](dataset-definitions-access.md "check type definition")

## formatStandards

Section includes technical attributes for language vocabularies, sizes etc. and gives researchers facts about and processing the underlying data in the dataset.


`formatStandards`

-   is optional
-   Type: merged type ([Formats and Standards](dataset-definitions-accessibility-properties-formats-and-standards.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-accessibility-properties-formats-and-standards.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/accessibility/properties/formatStandards")

### formatStandards Type

merged type ([Formats and Standards](dataset-definitions-accessibility-properties-formats-and-standards.md))

all of

-   [Untitled object in HDR UK Dataset](dataset-definitions-formatstandards.md "check type definition")

## enrichmentLinkage

This section includes information about related datasets that may have previously been linked, as well as indicating if there is the opportunity to link to other datasets in the future. If a dataset has been enriched and/or derivations, scores and existing tools are available this section allows providers to indicate this to researchers.


`enrichmentLinkage`

-   is optional
-   Type: merged type ([Enrichment and Linkage](dataset-definitions-accessibility-properties-enrichment-and-linkage.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-accessibility-properties-enrichment-and-linkage.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/accessibility/properties/enrichmentLinkage")

### enrichmentLinkage Type

merged type ([Enrichment and Linkage](dataset-definitions-accessibility-properties-enrichment-and-linkage.md))

all of

-   [Untitled object in HDR UK Dataset](dataset-definitions-enrichmentlinkage.md "check type definition")
