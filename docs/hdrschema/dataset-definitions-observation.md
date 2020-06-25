# Untitled object in HDR UK Dataset Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/observations/properties/observation/items/allOf/0
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## 0 Type

`object` ([Details](dataset-definitions-observation.md))

# undefined Properties

| Property                                                  | Type        | Required | Nullable       | Defined by                                                                                                                                                                                                        |
| :-------------------------------------------------------- | ----------- | -------- | -------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [observed-node](#observed-node)                           | Merged      | Required | cannot be null | [HDR UK Dataset](dataset-definitions-observation-properties-statistical-population.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observation/properties/observed-node")                  |
| [measured-value](#measured-value)                         | `integer`   | Required | cannot be null | [HDR UK Dataset](dataset-definitions-observation-properties-measured-value.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observation/properties/measured-value")                         |
| [disambiguating-description](#disambiguating-description) | Merged      | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-observation-properties-disambiguating-description.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observation/properties/disambiguating-description") |
| [observation-date](#observation-date)                     | `date-time` | Required | cannot be null | [HDR UK Dataset](dataset-definitions-observation-properties-observation-date.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observation/properties/observation-date")                     |
| [measured-property](#measured-property)                   | `string`    | Required | cannot be null | [HDR UK Dataset](dataset-definitions-observation-properties-measured-property.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observation/properties/measured-property")                   |

## observed-node

Please select one of the following statistical populations for you observation


> <https://schema.org/observedNode>
>

`observed-node`

-   is required
-   Type: merged type ([Statistical Population](dataset-definitions-observation-properties-statistical-population.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-observation-properties-statistical-population.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observation/properties/observed-node")

### observed-node Type

merged type ([Statistical Population](dataset-definitions-observation-properties-statistical-population.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-statisticalpopulationcontrained.md "check type definition")

### observed-node Examples

```json
""
```

## measured-value

Please provide the population size associated with the population type the dataset i.e. 1000 people in a study, or 87 images (MRI) of Knee Usage Note: Used with Statistical Population, which specifies the type of the population in the dataset.


> <https://schema.org/measuredValue>
>

`measured-value`

-   is required
-   Type: `integer` ([Measured Value](dataset-definitions-observation-properties-measured-value.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-observation-properties-measured-value.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observation/properties/measured-value")

### measured-value Type

`integer` ([Measured Value](dataset-definitions-observation-properties-measured-value.md))

## disambiguating-description

If SNOMED CT term does not provide sufficient detail, please provide a description that disambiguates the population type.


> <https://schema.org/disambiguatingDescription> 
>

`disambiguating-description`

-   is optional
-   Type: merged type ([Disambiguating Description](dataset-definitions-observation-properties-disambiguating-description.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-observation-properties-disambiguating-description.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observation/properties/disambiguating-description")

### disambiguating-description Type

merged type ([Disambiguating Description](dataset-definitions-observation-properties-disambiguating-description.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-abstract.md "check type definition")

## observation-date

Please provide the date of the observation


> <https://schema.org/observationDate>
>

`observation-date`

-   is required
-   Type: `date-time` ([Observation Date](dataset-definitions-observation-properties-observation-date.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-observation-properties-observation-date.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observation/properties/observation-date")

### observation-date Type

`date-time` ([Observation Date](dataset-definitions-observation-properties-observation-date.md))

### observation-date Default Value

The default value is:

```json
"release date"
```

## measured-property

Initially this will be defaulted to "Count"


> <https://schema.org/measuredProperty>
>

`measured-property`

-   is required
-   Type: `string` ([Measured Property](dataset-definitions-observation-properties-measured-property.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-observation-properties-measured-property.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observation/properties/measured-property")

### measured-property Type

`string` ([Measured Property](dataset-definitions-observation-properties-measured-property.md))

### measured-property Default Value

The default value is:

```json
"Count"
```
