# Dataset identifier Schema

```txt
#/properties/id#/properties/id
```

Dataset identifier


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                    |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ----------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../schema/dataset.schema.json "open original schema") |

## id Type

`string` ([Dataset identifier](dataset-properties-dataset-identifier.md))

## id Constraints

**maximum length**: the maximum number of characters for this string is: `36`

**minimum length**: the minimum number of characters for this string is: `36`

**pattern**: the string must match the following regular expression: 

```regexp
^[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}$
```

[try pattern](https://regexr.com/?expression=%5E%5Ba-fA-F0-9%5D%7B8%7D-%5Ba-fA-F0-9%5D%7B4%7D-%5Ba-fA-F0-9%5D%7B4%7D-%5Ba-fA-F0-9%5D%7B4%7D-%5Ba-fA-F0-9%5D%7B12%7D%24 "try regular expression with regexr.com")
