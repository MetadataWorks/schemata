# Dataset publisher Schema

```txt
#/properties/publisher#/properties/publisher
```

This is the organisation responsible for running or supporting the data access request process, as well as publishing and maintaining the metadata. In most this will be the same as the HDR UK Organisation (Hub or Alliance Member). However, in some cases this will be different i.e. Tissue Directory are an HDR UK Gateway organisation but coordinate activities across a number of data publishers i.e. Cambridge Blood and Stem Cell Biobank.


> Conforms to spec, but this MAY be an an object of organisation
>

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../../../schema/dataset/latest/dataset.schema.json "open original schema") |

## publisher Type

`string` ([Dataset publisher](dataset-properties-dataset-publisher.md))

## publisher Constraints

**maximum length**: the maximum number of characters for this string is: `80`

**minimum length**: the minimum number of characters for this string is: `2`
