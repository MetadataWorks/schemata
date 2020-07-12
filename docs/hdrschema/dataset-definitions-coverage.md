# Coverage Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/coverage
```

This information includes attributes for geographical and temporal coverage, cohort details etc. to enable a deeper understanding of the dataset content so that researchers can make decisions about the relevance of the underlying data.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## coverage Type

`object` ([Coverage](dataset-definitions-coverage.md))

# Coverage Properties

| Property                                                      | Type    | Required | Nullable       | Defined by                                                                                                                                                                                                      |
| :------------------------------------------------------------ | ------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [spatial](#spatial)                                           | `url`   | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-coverage-properties-geographic-coverage.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/coverage/properties/spatial")                               |
| [physical-sample-availability](#physical-sample-availability) | `array` | Required | cannot be null | [HDR UK Dataset](dataset-definitions-coverage-properties-physical-sample-availability.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/coverage/properties/physical-sample-availability") |
| [typical-age-range](#typical-age-range)                       | Merged  | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-coverage-properties-age-range.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/coverage/properties/typical-age-range")                               |
| [followup](#followup)                                         | Merged  | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-coverage-properties-followup.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/coverage/properties/followup")                                         |
| [pathway](#pathway)                                           | Merged  | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-coverage-properties-pathway.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/coverage/properties/pathway")                                           |

## spatial

The geographical area covered by the dataset. Notes: It is recommended that links are to entries in a well-maintained gazetteer such as <https://www.geonames.org/>


> dct:spatial
>

`spatial`

-   is optional
-   Type: `url` ([Geographic Coverage](dataset-definitions-coverage-properties-geographic-coverage.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-coverage-properties-geographic-coverage.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/coverage/properties/spatial")

### spatial Type

`url` ([Geographic Coverage](dataset-definitions-coverage-properties-geographic-coverage.md))

### spatial Examples

```json
"https://www.geonames.org/11609043/north-yorkshire.html"
```

## physical-sample-availability




> No standard identified
>

`physical-sample-availability`

-   is required
-   Type: an array of merged types ([Details](dataset-definitions-coverage-properties-physical-sample-availability-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-coverage-properties-physical-sample-availability.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/coverage/properties/physical-sample-availability")

### physical-sample-availability Type

an array of merged types ([Details](dataset-definitions-coverage-properties-physical-sample-availability-items.md))

### physical-sample-availability Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

### physical-sample-availability Examples

```json
"BONE MARROW"
```

## typical-age-range

Guidance: Please indicate the age range in whole years of participants in the dataset. Please provide range in the following format ‘[min age] – [max age]’ where both the minimum and maximum are whole numbers (integers).


> <https://schema.org/typicalAgeRange>
>

`typical-age-range`

-   is optional
-   Type: merged type ([Age Range](dataset-definitions-coverage-properties-age-range.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-coverage-properties-age-range.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/coverage/properties/typical-age-range")

### typical-age-range Type

merged type ([Age Range](dataset-definitions-coverage-properties-age-range.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-agerange.md "check type definition")

### typical-age-range Examples

```json
"0-18"
```

## followup

If known, what is the typical time span that a patient appears in the dataset (follow up period)


> No standard identified
>

`followup`

-   is optional
-   Type: merged type ([Followup](dataset-definitions-coverage-properties-followup.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-coverage-properties-followup.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/coverage/properties/followup")

### followup Type

merged type ([Followup](dataset-definitions-coverage-properties-followup.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-followup.md "check type definition")

### followup Default Value

The default value is:

```json
"UNKNOWN"
```

## pathway

Please indicate if the dataset is representative of the patient pathway and any limitations the dataset may have with respect to pathway coverage. This could include if the dataset is from a single speciality or area, a single tier of care, linked across two tiers (e.g. primary and secondary care), or an integrated care record covering the whole patient pathway.


> No standard identified
>

`pathway`

-   is optional
-   Type: merged type ([Pathway](dataset-definitions-coverage-properties-pathway.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-coverage-properties-pathway.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/coverage/properties/pathway")

### pathway Type

merged type ([Pathway](dataset-definitions-coverage-properties-pathway.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-description.md "check type definition")
