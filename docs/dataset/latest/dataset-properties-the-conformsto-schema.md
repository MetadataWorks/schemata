# The conformsTo schema Schema

```txt
#/properties/conformsTo#/properties/conformsTo
```

An explanation about the purpose of this instance.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                                         |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../../../schema/dataset/latest/dataset.schema.json "open original schema") |

## conformsTo Type

`string` ([The conformsTo schema](dataset-properties-the-conformsto-schema.md))

## conformsTo Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value        | Explanation |
| :----------- | ----------- |
| `"HL7 FHIR"` |             |
| `"HL7 V2"`   |             |
| `"HL7 CDA"`  |             |
| `"HL7 CCOW"` |             |
| `"LOINC"`    |             |
| `"DICOM"`    |             |
| `"I2B2"`     |             |
| `"IHE"`      |             |
| `"OMOP"`     |             |
| `"OPENEHR"`  |             |
| `"SENTINEL"` |             |
| `"PCORNET"`  |             |
| `"CDISC"`    |             |
| `"LOCAL"`    |             |
| `"OTHER"`    |             |
