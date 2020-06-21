# The keywords schema Schema

```txt
#/properties/keywords#/properties/keywords
```

An explanation about the purpose of this instance.


> Conforms to spec, but this MAY be an array of strings
>

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                    |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ----------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../schema/dataset.schema.json "open original schema") |

## keywords Type

`string` ([The keywords schema](dataset-properties-the-keywords-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-keywords-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-keywords-schema-anyof-1.md "check type definition")

## keywords Constraints

**pattern**: the string must match the following regular expression: 

```regexp
[0-9a-zA-Z._\-]+(,[0-9a-zA-Z.\-_]+)*
```

[try pattern](https://regexr.com/?expression=%5B0-9a-zA-Z._%5C-%5D%2B(%2C%5B0-9a-zA-Z.%5C-_%5D%2B)* "try regular expression with regexr.com")
