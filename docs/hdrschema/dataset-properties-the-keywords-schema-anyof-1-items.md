# Untitled string in HDR UK Dataset Schema

```txt
#/properties/keywords#/properties/keywords/anyOf/1/items
```




| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                    |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ----------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../schema/dataset.schema.json "open original schema") |

## items Type

`string`

## items Constraints

**pattern**: the string must match the following regular expression: 

```regexp
[0-9a-zA-Z._\-]+(,[0-9a-zA-Z.\-_]+)*
```

[try pattern](https://regexr.com/?expression=%5B0-9a-zA-Z._%5C-%5D%2B(%2C%5B0-9a-zA-Z.%5C-_%5D%2B)* "try regular expression with regexr.com")
