# Untitled string in HDR UK Dataset Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/access/properties/jurisdiction/items/allOf/0
```




> FIXME: Add ISO 3166-2 Subdivision code pattern
>

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## 0 Type

`string`

## 0 Constraints

**pattern**: the string must match the following regular expression: 

```regexp
^[A-Z]{2}(-[A-Z]{2,3})?$
```

[try pattern](https://regexr.com/?expression=%5E%5BA-Z%5D%7B2%7D(-%5BA-Z%5D%7B2%2C3%7D)%3F%24 "try regular expression with regexr.com")
