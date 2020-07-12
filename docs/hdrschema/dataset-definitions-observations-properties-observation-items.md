# Untitled undefined type in HDR UK Dataset Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/observations/properties/observation/items
```

Multiple observations about the dataset may be provided and users are expected to provide at least one observation (1..\*). We will be supporting the schema.org observation model (<https://schema.org/Observation>) with default values. Users will be encouraged to provide their own statistical populations as the project progresses. Example: &lt;b> Statistical Population 1 &lt;/b> type: StatisticalPopulation populationType: Persons numConstraints: 0 &lt;b> Statistical Population 2 &lt;/b> type: StatisticalPopulation populationType: Events numConstraints: 0 &lt;b> Statistical Population 3 &lt;/b> type: StatisticalPopulation populationType: Findings numConstraints: 0 typeOf: Observation observedNode: &lt;b> Statistical Population 1 &lt;/b> measuredProperty: count measuredValue: 32937 observationDate: “2017”


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## items Type

merged type ([Details](dataset-definitions-observations-properties-observation-items.md))

all of

-   [Untitled object in HDR UK Dataset](dataset-definitions-observation.md "check type definition")
