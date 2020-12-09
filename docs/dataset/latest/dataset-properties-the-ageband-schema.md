# The ageBand schema Schema

```txt
#/properties/ageBand#/properties/ageBand
```

Please indicate the age range in whole years of participants in the dataset. Please provide range in the following format ‘[min age] – [max age]’ where both the minimum and maximum are whole numbers (integers).


> FIXME: Rename MDC response to ageRange according to spec
>

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../../../schema/dataset/latest/dataset.schema.json "open original schema") |

## ageBand Type

`string` ([The ageBand schema](dataset-properties-the-ageband-schema.md))

## ageBand Constraints

**pattern**: the string must match the following regular expression: 

```regexp
\d{1,3}-\d{1,3}
```

[try pattern](https://regexr.com/?expression=%5Cd%7B1%2C3%7D-%5Cd%7B1%2C3%7D "try regular expression with regexr.com")
