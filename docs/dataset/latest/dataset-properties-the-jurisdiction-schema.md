# The jurisdiction schema Schema

```txt
#/properties/jurisdiction#/properties/jurisdiction
```

Please use country code from ISO 3166-1 country codes and the associated ISO 3166-2 for regions, cities, states etc. for the country/state under whose laws the data subjects’ data is collected, processed and stored.


> FIXME: Add ISO 3166-2 Subdivision code pattern
>

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../../../schema/dataset/latest/dataset.schema.json "open original schema") |

## jurisdiction Type

`string` ([The jurisdiction schema](dataset-properties-the-jurisdiction-schema.md))

## jurisdiction Constraints

**pattern**: the string must match the following regular expression: 

```regexp
^[A-Z]{2}(-[A-Z]{2,3})?$
```

[try pattern](https://regexr.com/?expression=%5E%5BA-Z%5D%7B2%7D(-%5BA-Z%5D%7B2%2C3%7D)%3F%24 "try regular expression with regexr.com")
