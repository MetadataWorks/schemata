# The disabmiguatingDescription schema Schema

```txt
#/properties/disabmiguatingDescription#/properties/disabmiguatingDescription
```

If SNOMED CT term does not provide sufficient detail, please provide a description that disambiguates the population type.


> FIXME: Rename MDC response to ageRange according to spec
>

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                    |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ----------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../schema/dataset.schema.json "open original schema") |

## disabmiguatingDescription Type

`string` ([The disabmiguatingDescription schema](dataset-properties-the-disabmiguatingdescription-schema.md))

## disabmiguatingDescription Constraints

**pattern**: the string must match the following regular expression: 

```regexp
\d{1,3}-\d{1,3}
```

[try pattern](https://regexr.com/?expression=%5Cd%7B1%2C3%7D-%5Cd%7B1%2C3%7D "try regular expression with regexr.com")
