# Title Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/title
```

Name of the dataset limited to 80 characters. It should provide a short description of the dataset and be unique across the gateway. If your title is not unique, please add a prefix with your organisation name or identifier to differentiate it from other datasets within the Gateway. Please avoid acronyms wherever possible. Good titles should summarise the content of the dataset and if relevant, the region the dataset covers. Notes: if the dataset is a “linked dataset”, please indicate this using the prefix “Linked”.


> dct:title
>

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## title Type

merged type ([Title](dataset-definitions-summary-properties-title.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-eightycharacters.md "check type definition")

## title Examples

```json
"North West London COVID-19 Patient Level Situation Report"
```
