# Untitled object in HDR UK Dataset Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/accessibility/properties/usage/allOf/0
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## 0 Type

`object` ([Details](dataset-definitions-usage.md))

# undefined Properties

| Property                                        | Type    | Required | Nullable       | Defined by                                                                                                                                                                                  |
| :---------------------------------------------- | ------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [data-use-limitation](#data-use-limitation)     | Merged  | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-usage-properties-data-use-limitation.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/usage/properties/data-use-limitation")     |
| [data-use-requirements](#data-use-requirements) | `array` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-usage-properties-data-use-requirements.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/usage/properties/data-use-requirements") |
| [resource-creator](#resource-creator)           | `array` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-usage-properties-citation-requirements.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/usage/properties/resource-creator")      |
| [investigations](#investigations)               | `array` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-usage-properties-investigations.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/usage/properties/investigations")               |
| [is-referenced-by](#is-referenced-by)           | `array` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-usage-properties-citations.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/usage/properties/is-referenced-by")                  |

## data-use-limitation

Please provide an indication of consent permissions for datasets and/or materials, and relates to the purposes for which datasets and/or material might be removed, stored or used. NOTE: we have extended the DUO to include a value for NO LINKAGE


> <https://www.ebi.ac.uk/ols/ontologies/duo/terms?iri=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FDUO_0000001>
>

`data-use-limitation`

-   is optional
-   Type: merged type ([Data Use Limitation](dataset-definitions-usage-properties-data-use-limitation.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-usage-properties-data-use-limitation.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/usage/properties/data-use-limitation")

### data-use-limitation Type

merged type ([Data Use Limitation](dataset-definitions-usage-properties-data-use-limitation.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-datauselimitation.md "check type definition")

## data-use-requirements




> <https://www.ebi.ac.uk/ols/ontologies/duo/terms?iri=http%3A%2F%2Fpurl.obolibrary.org%2Fobo%2FDUO_0000001>
>

`data-use-requirements`

-   is optional
-   Type: an array of merged types ([Details](dataset-definitions-usage-properties-data-use-requirements-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-usage-properties-data-use-requirements.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/usage/properties/data-use-requirements")

### data-use-requirements Type

an array of merged types ([Details](dataset-definitions-usage-properties-data-use-requirements-items.md))

### data-use-requirements Constraints

**minimum number of items**: the minimum number of items for this array is: `0`

## resource-creator




> dct:creator
>

`resource-creator`

-   is optional
-   Type: `string[]`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-usage-properties-citation-requirements.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/usage/properties/resource-creator")

### resource-creator Type

`string[]`

### resource-creator Constraints

**minimum number of items**: the minimum number of items for this array is: `0`

## investigations




> No standard identified
>

`investigations`

-   is optional
-   Type: `url[]`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-usage-properties-investigations.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/usage/properties/investigations")

### investigations Type

`url[]`

### investigations Constraints

**minimum number of items**: the minimum number of items for this array is: `0`

## is-referenced-by




> dct:isReferencedBy 
>

`is-referenced-by`

-   is optional
-   Type: an array of merged types ([Details](dataset-definitions-usage-properties-citations-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-usage-properties-citations.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/usage/properties/is-referenced-by")

### is-referenced-by Type

an array of merged types ([Details](dataset-definitions-usage-properties-citations-items.md))

### is-referenced-by Constraints

**minimum number of items**: the minimum number of items for this array is: `0`
