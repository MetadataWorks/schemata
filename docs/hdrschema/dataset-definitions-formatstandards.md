# Untitled object in HDR UK Dataset Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/accessibility/properties/formatStandards/allOf/0
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## 0 Type

`object` ([Details](dataset-definitions-formatstandards.md))

# undefined Properties

| Property                                                  | Type    | Required | Nullable       | Defined by                                                                                                                                                                                                           |
| :-------------------------------------------------------- | ------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [conforms-to](#conforms-to)                               | Merged  | Required | cannot be null | [HDR UK Dataset](dataset-definitions-formatstandards-properties-conforms-to.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/formatStandards/properties/conforms-to")                          |
| [vocabulary-encoding-scheme](#vocabulary-encoding-scheme) | `array` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-formatstandards-properties-controlled-vocabulary.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/formatStandards/properties/vocabulary-encoding-scheme") |
| [language](#language)                                     | `array` | Required | cannot be null | [HDR UK Dataset](dataset-definitions-formatstandards-properties-language.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/formatStandards/properties/language")                                |
| [format](#format)                                         | `array` | Required | cannot be null | [HDR UK Dataset](dataset-definitions-formatstandards-properties-format.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/formatStandards/properties/format")                                    |

## conforms-to

List standardised data models that the dataset has been stored in or transformed to, such as OMOP or FHIR. If the data is only available in a local format, please make that explicit. If you are using a standard that has not been included in the list, please use “other” and contact support desk to ask for an addition.


> dct:conformsTo
>

`conforms-to`

-   is required
-   Type: merged type ([Conforms To](dataset-definitions-formatstandards-properties-conforms-to.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-formatstandards-properties-conforms-to.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/formatStandards/properties/conforms-to")

### conforms-to Type

merged type ([Conforms To](dataset-definitions-formatstandards-properties-conforms-to.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-standardiseddatamodels.md "check type definition")

### conforms-to Default Value

The default value is:

```json
"LOCAL"
```

## vocabulary-encoding-scheme




> <https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#http://purl.org/dc/dcam/VocabularyEncodingScheme>
>

`vocabulary-encoding-scheme`

-   is optional
-   Type: an array of merged types ([Details](dataset-definitions-formatstandards-properties-controlled-vocabulary-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-formatstandards-properties-controlled-vocabulary.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/formatStandards/properties/vocabulary-encoding-scheme")

### vocabulary-encoding-scheme Type

an array of merged types ([Details](dataset-definitions-formatstandards-properties-controlled-vocabulary-items.md))

### vocabulary-encoding-scheme Constraints

**minimum number of items**: the minimum number of items for this array is: `0`

### vocabulary-encoding-scheme Default Value

The default value is:

```json
"LOCAL"
```

## language




> dct:language
>

`language`

-   is required
-   Type: an array of merged types ([Details](dataset-definitions-formatstandards-properties-language-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-formatstandards-properties-language.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/formatStandards/properties/language")

### language Type

an array of merged types ([Details](dataset-definitions-formatstandards-properties-language-items.md))

### language Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

### language Default Value

The default value is:

```json
"en"
```

## format




> <http://purl.org/dc/terms/format> 
>

`format`

-   is required
-   Type: an array of merged types ([Details](dataset-definitions-formatstandards-properties-format-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-formatstandards-properties-format.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/formatStandards/properties/format")

### format Type

an array of merged types ([Details](dataset-definitions-formatstandards-properties-format-items.md))

### format Constraints

**minimum number of items**: the minimum number of items for this array is: `1`
