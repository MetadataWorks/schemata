# Untitled string in HDR UK Dataset Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/usage/properties/is-referenced-by/items/allOf/0
```




| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## 0 Type

`string`

## 0 Constraints

**pattern**: the string must match the following regular expression: 

```regexp
^10.\d{4,9}/[-._;()/:a-zA-Z0-9]+$
```

[try pattern](https://regexr.com/?expression=%5E10.%5Cd%7B4%2C9%7D%2F%5B-._%3B()%2F%3Aa-zA-Z0-9%5D%2B%24 "try regular expression with regexr.com")
