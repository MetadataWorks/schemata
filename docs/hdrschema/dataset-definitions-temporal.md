# Untitled object in HDR UK Dataset Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/provenance/properties/temporal/allOf/0
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## 0 Type

`object` ([Details](dataset-definitions-temporal.md))

# undefined Properties

| Property                                                | Type   | Required | Nullable       | Defined by                                                                                                                                                                                   |
| :------------------------------------------------------ | ------ | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [accrual-periodicity](#accrual-periodicity)             | Merged | Required | cannot be null | [HDR UK Dataset](dataset-definitions-temporal-properties-periodicity.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/temporal/properties/accrual-periodicity")        |
| [time-lag](#time-lag)                                   | Merged | Required | cannot be null | [HDR UK Dataset](dataset-definitions-temporal-properties-time-lag.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/temporal/properties/time-lag")                      |
| [distribution-release-date](#distribution-release-date) | `date` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-temporal-properties-release-date.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/temporal/properties/distribution-release-date") |
| [start-date](#start-date)                               | `date` | Required | cannot be null | [HDR UK Dataset](dataset-definitions-temporal-properties-start-date.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/temporal/properties/start-date")                  |
| [end-date](#end-date)                                   | `date` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-temporal-properties-end-date.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/temporal/properties/end-date")                      |

## accrual-periodicity

Please indicate the frequency of publishing. If a dataset is published regularly please choose a publishing periodicity from the constrained list and indicate the next release date. When the release date becomes historical, a new release date will be calculated based on the publishing periodicity. If a dataset has been published and will remain static please indicate that it is static and indicated when it was released. If a dataset is released on an irregular basis or “on-demand” please indicate that it is Irregular and leave release date as null. If a dataset can be published in real-time or near-real-time please indicate that it is continuous and leave release date as null. Notes: see <https://www.dublincore.org/specifications/dublin-core/collection-description/frequency/>


> dct:accrualPeriodicity
>

`accrual-periodicity`

-   is required
-   Type: merged type ([Periodicity](dataset-definitions-temporal-properties-periodicity.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-temporal-properties-periodicity.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/temporal/properties/accrual-periodicity")

### accrual-periodicity Type

merged type ([Periodicity](dataset-definitions-temporal-properties-periodicity.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-periodicity.md "check type definition")

## time-lag

Please indicate the typical time-lag between an event and the data for that event appearing in the dataset


> No standard identified
>

`time-lag`

-   is required
-   Type: merged type ([Time Lag](dataset-definitions-temporal-properties-time-lag.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-temporal-properties-time-lag.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/temporal/properties/time-lag")

### time-lag Type

merged type ([Time Lag](dataset-definitions-temporal-properties-time-lag.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-timelag.md "check type definition")

## distribution-release-date

Date of the latest release of the dataset. If this is a regular release i.e. quarterly, or this is a static dataset please complete this alongside Periodicity. If this is Irregular or Continuously released please leave this blank. Notes: Periodicity and release date will be used to determine when the next release is expected. i.e. the next release date can then be calculated automatically. E.g. if the release date is documented as 01/01/2020 and it is now 20/04/2020 and there is a quarterly release schedule, the latest release will be calculated as 01/04/2020.


> dcat:distribution_release_date
>

`distribution-release-date`

-   is optional
-   Type: `date` ([Release Date](dataset-definitions-temporal-properties-release-date.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-temporal-properties-release-date.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/temporal/properties/distribution-release-date")

### distribution-release-date Type

`date` ([Release Date](dataset-definitions-temporal-properties-release-date.md))

## start-date

The start of the time period that the dataset provides coverage for. If there are multiple cohorts in the dataset with varying start dates, please provide the earliest date and use the description or the media attribute to provide more information.


> dcat:startDate
>

`start-date`

-   is required
-   Type: `date` ([Start Date](dataset-definitions-temporal-properties-start-date.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-temporal-properties-start-date.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/temporal/properties/start-date")

### start-date Type

`date` ([Start Date](dataset-definitions-temporal-properties-start-date.md))

## end-date

The end of the time period that the dataset provides coverage for. If the dataset is “Continuous” and has no known end date, please leave blank. If there are multiple cohorts in the dataset with varying end dates, please provide the latest date and use the description or the media attribute to provide more information.


> dcat:endDate
>

`end-date`

-   is optional
-   Type: `date` ([End Date](dataset-definitions-temporal-properties-end-date.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-temporal-properties-end-date.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/temporal/properties/end-date")

### end-date Type

`date` ([End Date](dataset-definitions-temporal-properties-end-date.md))
