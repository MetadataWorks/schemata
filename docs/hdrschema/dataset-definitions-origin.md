# Untitled object in HDR UK Dataset Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/provenance/properties/origin/allOf/0
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## 0 Type

`object` ([Details](dataset-definitions-origin.md))

# undefined Properties

| Property                                                      | Type    | Required | Nullable       | Defined by                                                                                                                                                                             |
| :------------------------------------------------------------ | ------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [purpose](#purpose)                                           | `array` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-origin-properties-purpose.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/origin/properties/purpose")                      |
| [source](#source)                                             | `array` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-origin-properties-source.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/origin/properties/source")                        |
| [type-of-collection-situation](#type-of-collection-situation) | `array` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-origin-properties-setting.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/origin/properties/type-of-collection-situation") |

## purpose




> <https://ddialliance.org/Specification/DDI-Lifecycle/3.3/XMLSchema/FieldLevelDocumentation/>
>

`purpose`

-   is optional
-   Type: an array of merged types ([Details](dataset-definitions-origin-properties-purpose-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-origin-properties-purpose.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/origin/properties/purpose")

### purpose Type

an array of merged types ([Details](dataset-definitions-origin-properties-purpose-items.md))

### purpose Constraints

**minimum number of items**: the minimum number of items for this array is: `0`

## source




> <https://dublincore.org/specifications/dublin-core/dcmi-terms/#source>
>

`source`

-   is optional
-   Type: an array of merged types ([Details](dataset-definitions-origin-properties-source-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-origin-properties-source.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/origin/properties/source")

### source Type

an array of merged types ([Details](dataset-definitions-origin-properties-source-items.md))

### source Constraints

**minimum number of items**: the minimum number of items for this array is: `0`

## type-of-collection-situation




> <https://ddialliance.org/Specification/DDI-Lifecycle/3.2/XMLSchema/FieldLevelDocumentation/>
>

`type-of-collection-situation`

-   is optional
-   Type: an array of merged types ([Details](dataset-definitions-origin-properties-setting-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-origin-properties-setting.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/origin/properties/type-of-collection-situation")

### type-of-collection-situation Type

an array of merged types ([Details](dataset-definitions-origin-properties-setting-items.md))

### type-of-collection-situation Constraints

**minimum number of items**: the minimum number of items for this array is: `0`
