# Untitled object in HDR UK Dataset Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/accessibility/properties/enrichmentLinkage/allOf/0
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## 0 Type

`object` ([Details](dataset-definitions-enrichmentlinkage.md))

# undefined Properties

| Property                                  | Type    | Required | Nullable       | Defined by                                                                                                                                                                                                 |
| :---------------------------------------- | ------- | -------- | -------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [qualified-relation](#qualified-relation) | `array` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-enrichmentlinkage-properties-linked-datasets.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/enrichmentLinkage/properties/qualified-relation") |
| [derivation](#derivation)                 | `array` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-enrichmentlinkage-properties-derivations.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/enrichmentLinkage/properties/derivation")             |
| [tools](#tools)                           | `array` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-enrichmentlinkage-properties-tools.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/enrichmentLinkage/properties/tools")                        |

## qualified-relation




> dcat:qualifiedRelation
>

`qualified-relation`

-   is optional
-   Type: an array of merged types ([Details](dataset-definitions-enrichmentlinkage-properties-linked-datasets-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-enrichmentlinkage-properties-linked-datasets.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/enrichmentLinkage/properties/qualified-relation")

### qualified-relation Type

an array of merged types ([Details](dataset-definitions-enrichmentlinkage-properties-linked-datasets-items.md))

### qualified-relation Constraints

**minimum number of items**: the minimum number of items for this array is: `0`

## derivation




> prov:Derivation
>

`derivation`

-   is optional
-   Type: an array of merged types ([Details](dataset-definitions-enrichmentlinkage-properties-derivations-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-enrichmentlinkage-properties-derivations.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/enrichmentLinkage/properties/derivation")

### derivation Type

an array of merged types ([Details](dataset-definitions-enrichmentlinkage-properties-derivations-items.md))

### derivation Constraints

**minimum number of items**: the minimum number of items for this array is: `0`

## tools




> No standard identified. We encourage users to adopt a model along the lines of <https://www.ga4gh.org/news/tool-registry-service-api-enabling-an-interoperable-library-of-genomics-analysis-tools/>
>

`tools`

-   is optional
-   Type: `url[]`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-enrichmentlinkage-properties-tools.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/enrichmentLinkage/properties/tools")

### tools Type

`url[]`

### tools Constraints

**minimum number of items**: the minimum number of items for this array is: `0`
