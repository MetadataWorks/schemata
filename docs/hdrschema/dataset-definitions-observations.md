# Observations Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/observations
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## observations Type

`object` ([Observations](dataset-definitions-observations.md))

# Observations Properties

| Property                    | Type    | Required | Nullable       | Defined by                                                                                                                                                                            |
| :-------------------------- | ------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [observation](#observation) | `array` | Required | cannot be null | [HDR UK Dataset](dataset-definitions-observations-properties-observation.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observations/properties/observation") |

## observation




`observation`

-   is required
-   Type: an array of merged types ([Observation](dataset-definitions-observations-properties-observation-observation.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-observations-properties-observation.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observations/properties/observation")

### observation Type

an array of merged types ([Observation](dataset-definitions-observations-properties-observation-observation.md))

### observation Constraints

**minimum number of items**: the minimum number of items for this array is: `1`
