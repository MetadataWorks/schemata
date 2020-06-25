# Conforms To Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/formatStandards/properties/conforms-to
```

List standardised data models that the dataset has been stored in or transformed to, such as OMOP or FHIR. If the data is only available in a local format, please make that explicit. If you are using a standard that has not been included in the list, please use “other” and contact support desk to ask for an addition.


> dct:conformsTo
>

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## conforms-to Type

merged type ([Conforms To](dataset-definitions-formatstandards-properties-conforms-to.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-standardiseddatamodels.md "check type definition")

## conforms-to Default Value

The default value is:

```json
"LOCAL"
```
