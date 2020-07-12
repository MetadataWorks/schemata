# Documentation Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/documentation
```

Documentation can include a rich text description of the dataset or links to media such as documents, images, presentations, videos or links to data dictionaries, profiles or dashboards. Organisations are required to confirm that they have permission to distribute any additional media.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## documentation Type

`object` ([Documentation](dataset-definitions-documentation.md))

# Documentation Properties

| Property                              | Type     | Required | Nullable       | Defined by                                                                                                                                                                                        |
| :------------------------------------ | -------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [description](#description)           | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-documentation-properties-description.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/documentation/properties/description")           |
| [associated-media](#associated-media) | `array`  | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-documentation-properties-associated-media.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/documentation/properties/associated-media") |
| [documentation](#documentation)       | `url`    | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-documentation-properties-documentation.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/documentation/properties/documentation")       |
| [is-part-of](#is-part-of)             | `string` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-documentation-properties-group.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/documentation/properties/is-part-of")                  |

## description

An HTML account of the data that provides context and scope of the data, limited to 3000 characters (1 Page), and/or a resolvable URL that describes the dataset. Additional information can be recorded and included using media. Notes: A WYSIWYG editor will be available through the onboarding portal.


> dc:description
>

`description`

-   is optional
-   Type: merged type ([Description](dataset-definitions-documentation-properties-description.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-documentation-properties-description.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/documentation/properties/description")

### description Type

merged type ([Description](dataset-definitions-documentation-properties-description.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-description.md "check type definition")

## associated-media




> <https://schema.org/associatedMedia>
>

`associated-media`

-   is optional
-   Type: `url[]`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-documentation-properties-associated-media.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/documentation/properties/associated-media")

### associated-media Type

`url[]`

### associated-media Examples

```json
"PDF Document that describes study protocol"
```

## documentation

Please provide a link to any additional technical documentation, such as data dictionaries, data catalogues, data profiles, summary dashboards or other technical assets that describe the dataset.


> <https://schema.org/documentation>
>

`documentation`

-   is optional
-   Type: `url` ([Documentation](dataset-definitions-documentation-properties-documentation.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-documentation-properties-documentation.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/documentation/properties/documentation")

### documentation Type

`url` ([Documentation](dataset-definitions-documentation-properties-documentation.md))

### documentation Examples

```json
""
```

## is-part-of

Please complete only if the dataset is part of a group or family of datasets i.e. Hospital Episode Statistics has several constituents.


>     https://schema.org/isPartOf NOTE: we may make Groups first class citizens so the are navigable
>

`is-part-of`

-   is optional
-   Type: `string` ([Group](dataset-definitions-documentation-properties-group.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-documentation-properties-group.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/documentation/properties/is-part-of")

### is-part-of Type

`string` ([Group](dataset-definitions-documentation-properties-group.md))

### is-part-of Default Value

The default value is:

```json
"Not Applicable"
```

### is-part-of Examples

```json
"Hospital Episodes Statistics datasets (A&E, APC, OP, AC MSDS)."
```
