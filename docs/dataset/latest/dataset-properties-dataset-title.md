# Dataset title Schema

```txt
#/properties/title#/properties/title
```

Name of the dataset limited to 80 characters. It should provide a short description of the dataset and be unique across the gateway. If your title is not unique, please add a prefix with your organisation name or identifier to differentiate it from other datasets within the Gateway. Please avoid acronyms wherever possible. Good titles should summarise the content of the dataset and if relevant, the region the dataset covers.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../../../schema/dataset/latest/dataset.schema.json "open original schema") |

## title Type

`string` ([Dataset title](dataset-properties-dataset-title.md))

## title Constraints

**maximum length**: the maximum number of characters for this string is: `80`

**minimum length**: the minimum number of characters for this string is: `2`
