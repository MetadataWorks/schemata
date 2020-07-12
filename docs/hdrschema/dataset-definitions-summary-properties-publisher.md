# Publisher Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/publisher
```

Completion Notes: This is the organisation responsible for running or supporting the data access request process, as well as publishing and maintaining the metadata. In most this will be the same as the HDR UK Organisation (Hub or Alliance Member). However, in some cases this will be different i.e. Tissue Directory are an HDR UK Gateway organisation but coordinate activities across a number of data publishers i.e. Cambridge Blood and Stem Cell Biobank.


> dct:publisher
>

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## publisher Type

merged type ([Publisher](dataset-definitions-summary-properties-publisher.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-eightycharacters.md "check type definition")

## publisher Default Value

The default value is:

```json
"Defaulted to the organisation registered the metadata in the catalogue"
```

## publisher Examples

```json
"Cambridge Blood and Stem Cell Biobank"
```
