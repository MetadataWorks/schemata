# Provenance Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/provenance
```

Provenance information allows researchers to understand data within the context of its origins and can be an indicator of quality, authenticity and timeliness.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## provenance Type

`object` ([Provenance](dataset-definitions-provenance.md))

# Provenance Properties

| Property              | Type   | Required | Nullable       | Defined by                                                                                                                                                                  |
| :-------------------- | ------ | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [origin](#origin)     | Merged | Required | cannot be null | [HDR UK Dataset](dataset-definitions-provenance-properties-origin.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/provenance/properties/origin")     |
| [temporal](#temporal) | Merged | Required | cannot be null | [HDR UK Dataset](dataset-definitions-provenance-properties-temporal.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/provenance/properties/temporal") |

## origin

Indicators of the origin of the data.


`origin`

-   is required
-   Type: merged type ([Origin](dataset-definitions-provenance-properties-origin.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-provenance-properties-origin.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/provenance/properties/origin")

### origin Type

merged type ([Origin](dataset-definitions-provenance-properties-origin.md))

all of

-   [Untitled object in HDR UK Dataset](dataset-definitions-origin.md "check type definition")

## temporal

Information indicative of temporal provenance.


`temporal`

-   is required
-   Type: merged type ([Temporal](dataset-definitions-provenance-properties-temporal.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-provenance-properties-temporal.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/provenance/properties/temporal")

### temporal Type

merged type ([Temporal](dataset-definitions-provenance-properties-temporal.md))

all of

-   [Untitled object in HDR UK Dataset](dataset-definitions-temporal.md "check type definition")
