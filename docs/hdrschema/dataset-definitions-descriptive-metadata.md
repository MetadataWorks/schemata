# Descriptive Metadata Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/allOf/0
```

Describes a resource for purposes of discovery and identification.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## 0 Type

`object` ([Descriptive Metadata](dataset-definitions-descriptive-metadata.md))

# Descriptive Metadata Properties

| Property                        | Type     | Required | Nullable       | Defined by                                                                                                                                                                |
| :------------------------------ | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [summary](#summary)             | `object` | Required | cannot be null | [HDR UK Dataset](dataset-definitions-summary.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/summary")             |
| [documentation](#documentation) | `object` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-documentation.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/documentation") |
| [coverage](#coverage)           | `object` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-coverage.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/coverage")           |
| [provenance](#provenance)       | `object` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-provenance.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/provenance")       |
| [accessibility](#accessibility) | `object` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-accessibility.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/accessibility") |
| [observations](#observations)   | `object` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-observations.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/observations")   |

## summary

Summary metadata must be completed by Data Custodians onboarding metadata into the Innovation Gateway MVP.


`summary`

-   is required
-   Type: `object` ([Summary](dataset-definitions-summary.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-summary.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/summary")

### summary Type

`object` ([Summary](dataset-definitions-summary.md))

## documentation

Documentation can include a rich text description of the dataset or links to media such as documents, images, presentations, videos or links to data dictionaries, profiles or dashboards. Organisations are required to confirm that they have permission to distribute any additional media.


`documentation`

-   is optional
-   Type: `object` ([Documentation](dataset-definitions-documentation.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-documentation.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/documentation")

### documentation Type

`object` ([Documentation](dataset-definitions-documentation.md))

## coverage

This information includes attributes for geographical and temporal coverage, cohort details etc. to enable a deeper understanding of the dataset content so that researchers can make decisions about the relevance of the underlying data.


`coverage`

-   is optional
-   Type: `object` ([Coverage](dataset-definitions-coverage.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-coverage.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/coverage")

### coverage Type

`object` ([Coverage](dataset-definitions-coverage.md))

## provenance

Provenance information allows researchers to understand data within the context of its origins and can be an indicator of quality, authenticity and timeliness.


`provenance`

-   is optional
-   Type: `object` ([Provenance](dataset-definitions-provenance.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-provenance.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/provenance")

### provenance Type

`object` ([Provenance](dataset-definitions-provenance.md))

## accessibility

Accessibility information allows researchers to understand access, usage, limitations, formats, standards and linkage or interoperability with toolsets.


`accessibility`

-   is optional
-   Type: `object` ([Accessibility](dataset-definitions-accessibility.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-accessibility.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/accessibility")

### accessibility Type

`object` ([Accessibility](dataset-definitions-accessibility.md))

## observations




`observations`

-   is optional
-   Type: `object` ([Observations](dataset-definitions-observations.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-observations.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/observations")

### observations Type

`object` ([Observations](dataset-definitions-observations.md))
