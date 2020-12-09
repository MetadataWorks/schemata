# The periodicity schema Schema

```txt
#/properties/periodicity#/properties/periodicity
```

The frequency at which dataset is published.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../../../schema/dataset/latest/dataset.schema.json "open original schema") |

## periodicity Type

`string` ([The periodicity schema](dataset-properties-the-periodicity-schema.md))

## periodicity Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | ----------- |
| `"STATIC"`     |             |
| `"ANNUAL"`     |             |
| `"BIENNIAL"`   |             |
| `"QUARTERLY"`  |             |
| `"BIMONTHLY"`  |             |
| `"MONTHLY"`    |             |
| `"BIWEEKLY"`   |             |
| `"WEEKLY"`     |             |
| `"SEMIWEEKLY"` |             |
| `"DAILY"`      |             |
| `"IRREGULAR"`  |             |
| `"CONTINUOUS"` |             |
