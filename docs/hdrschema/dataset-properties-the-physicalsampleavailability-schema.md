# The physicalSampleAvailability schema Schema

```txt
#/properties/physicalSampleAvailability#/properties/physicalSampleAvailability
```

Availability of physical samples associated with the dataset. If samples are available, please indicate the types of samples that are available.


| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                    |
| :------------------ | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ----------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../schema/dataset.schema.json "open original schema") |

## physicalSampleAvailability Type

`string` ([The physicalSampleAvailability schema](dataset-properties-the-physicalsampleavailability-schema.md))

## physicalSampleAvailability Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                            | Explanation |
| :------------------------------- | ----------- |
| `"Not Available"`                |             |
| `"Bone Marrow"`                  |             |
| `"Cancer Cell Lines"`            |             |
| `"Core Biopsy"`                  |             |
| `"CDNA/MRNA"`                    |             |
| `"DNA"`                          |             |
| `"Faeces"`                       |             |
| `"Immortalized Cel Lines"`       |             |
| `"MicroRNA"`                     |             |
| `"Peripheral Blood Cells"`       |             |
| `"Plasma"`                       |             |
| `"PM Tissue"`                    |             |
| `"Primary Cells"`                |             |
| `"RNA"`                          |             |
| `"Saliva"`                       |             |
| `"Serum"`                        |             |
| `"Swabs"`                        |             |
| `"Tissue"`                       |             |
| `"Urine"`                        |             |
| `"Whole Blood"`                  |             |
| `"Availability To Be Confirmed"` |             |

## physicalSampleAvailability Examples

```json
"Not Available"
```
