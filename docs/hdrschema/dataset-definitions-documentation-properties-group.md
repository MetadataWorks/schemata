# Group Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/documentation/properties/is-part-of
```

Please complete only if the dataset is part of a group or family of datasets i.e. Hospital Episode Statistics has several constituents.


>     https://schema.org/isPartOf NOTE: we may make Groups first class citizens so the are navigable
>

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## is-part-of Type

`string` ([Group](dataset-definitions-documentation-properties-group.md))

## is-part-of Default Value

The default value is:

```json
"Not Applicable"
```

## is-part-of Examples

```json
"Hospital Episodes Statistics datasets (A&E, APC, OP, AC MSDS)."
```
