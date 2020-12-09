# The accessRequestDuration schema Schema

```txt
#/properties/accessRequestDuration#/properties/accessRequestDuration
```

Please provide an indication of the typical processing times based on the types of requests typically received.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../../../schema/dataset/latest/dataset.schema.json "open original schema") |

## accessRequestDuration Type

`string` ([The accessRequestDuration schema](dataset-properties-the-accessrequestduration-schema.md))

## accessRequestDuration Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | ----------- |
| `"<1 Week"`    |             |
| `"1-2 Weeks"`  |             |
| `"2-4 Weeks"`  |             |
| `"1-2 Months"` |             |
| `"2-6 Months"` |             |
| `">6 Months"`  |             |
| `"Other"`      |             |
