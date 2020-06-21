# HDR UK Dataset Schema

```txt
http://healthdatagateway.org/schema/dataset.json
```

HDR UK Dataset Schema


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                  |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | --------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json](../schema/dataset.schema.json "open original schema") |

## HDR UK Dataset Type

`object` ([HDR UK Dataset](dataset.md))

# HDR UK Dataset Properties

| Property                                                  | Type     | Required | Nullable       | Defined by                                                                                                                                                      |
| :-------------------------------------------------------- | -------- | -------- | -------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [id](#id)                                                 | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-dataset-identifier.md "\#/properties/id#/properties/id")                                                                    |
| [identifier](#identifier)                                 | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-properties-local-dataset-identifier.md "\#/properties/identifier#/properties/identifier")                                              |
| [title](#title)                                           | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-dataset-title.md "\#/properties/title#/properties/title")                                                                   |
| [abstract](#abstract)                                     | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-dataset-abstract.md "\#/properties/abstract#/properties/abstract")                                                          |
| [publisher](#publisher)                                   | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-dataset-publisher.md "\#/properties/publisher#/properties/publisher")                                                       |
| [contactPoint](#contactPoint)                             | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-contactpoint-schema.md "\#/properties/contactPoint#/properties/contactPoint")                                           |
| [accessRights](#accessRights)                             | Merged   | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-accessrights-schema.md "\#/properties/accessRights#/properties/accessRights")                                           |
| [group](#group)                                           | `string` | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-group-schema.md "\#/properties/group#/properties/group")                                                                |
| [description](#description)                               | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-description-schema.md "\#/properties/description#/properties/description")                                              |
| [media](#media)                                           | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-media-schema.md "\#/properties/media#/properties/media")                                                                |
| [purpose](#purpose)                                       | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-purpose-schema.md "\#/properties/purpose#/properties/purpose")                                                          |
| [source](#source)                                         | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-source-schema.md "\#/properties/source#/properties/source")                                                             |
| [setting](#setting)                                       | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-setting-schema.md "\#/properties/setting#/properties/setting")                                                          |
| [releaseDate](#releaseDate)                               | `string` | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-releasedate-schema.md "\#/properties/releaseDate#/properties/releaseDate")                                              |
| [accessRequestCost](#accessRequestCost)                   | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-accessrequestcost-schema.md "\#/properties/accessRequestCost#/properties/accessRequestCost")                            |
| [accessRequestDuration](#accessRequestDuration)           | `string` | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-accessrequestduration-schema.md "\#/properties/accessRequestDuration#/properties/accessRequestDuration")                |
| [accessEnvironment](#accessEnvironment)                   | `string` | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-accessenvironment-schema.md "\#/properties/accessEnvironment#/properties/accessEnvironment")                            |
| [usageRestrictions](#usageRestrictions)                   | Merged   | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-usagerestrictions-schema.md "\#/properties/usageRestrictions#/properties/usageRestrictions")                            |
| [dataController](#dataController)                         | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-datacontroller-schema.md "\#/properties/dataController#/properties/dataController")                                     |
| [dataProcessor](#dataProcessor)                           | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-dataprocessor-schema.md "\#/properties/dataProcessor#/properties/dataProcessor")                                        |
| [license](#license)                                       | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-license-schema.md "\#/properties/license#/properties/license")                                                          |
| [derivedDatasets](#derivedDatasets)                       | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-deriveddatasets-schema.md "\#/properties/derivedDatasets#/properties/derivedDatasets")                                  |
| [linkedDataset](#linkedDataset)                           | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-linkeddataset-schema.md "\#/properties/linkedDataset#/properties/linkedDataset")                                        |
| [linkageOpportunity](#linkageOpportunity)                 | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-linkageopportunity-schema.md "\#/properties/linkageOpportunity#/properties/linkageOpportunity")                         |
| [geographicCoverage](#geographicCoverage)                 | `string` | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-geographiccoverage-schema.md "\#/properties/geographicCoverage#/properties/geographicCoverage")                         |
| [periodicity](#periodicity)                               | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-periodicity-schema.md "\#/properties/periodicity#/properties/periodicity")                                              |
| [datasetEndDate](#datasetEndDate)                         | `string` | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-datasetenddate-schema.md "\#/properties/datasetEndDate#/properties/datasetEndDate")                                     |
| [datasetStartDate](#datasetStartDate)                     | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-datasetstartdate-schema.md "\#/properties/datasetStartDate#/properties/datasetStartDate")                               |
| [jurisdiction](#jurisdiction)                             | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-jurisdiction-schema.md "\#/properties/jurisdiction#/properties/jurisdiction")                                           |
| [populationType](#populationType)                         | Merged   | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-populationtype-schema.md "\#/properties/populationType#/properties/populationType")                                     |
| [disabmiguatingDescription](#disabmiguatingDescription)   | `string` | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-disabmiguatingdescription-schema.md "\#/properties/disabmiguatingDescription#/properties/disabmiguatingDescription")    |
| [statisticalPopulation](#statisticalPopulation)           | Merged   | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-statisticalpopulation-schema.md "\#/properties/statisticalPopulation#/properties/statisticalPopulation")                |
| [ageBand](#ageBand)                                       | `string` | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-ageband-schema.md "\#/properties/ageBand#/properties/ageBand")                                                          |
| [physicalSampleAvailability](#physicalSampleAvailability) | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-physicalsampleavailability-schema.md "\#/properties/physicalSampleAvailability#/properties/physicalSampleAvailability") |
| [keywords](#keywords)                                     | Merged   | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-keywords-schema.md "\#/properties/keywords#/properties/keywords")                                                       |
| [conformsTo](#conformsTo)                                 | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-conformsto-schema.md "\#/properties/conformsTo#/properties/conformsTo")                                                 |
| [controlledVocabulary](#controlledVocabulary)             | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-controlledvocabulary-schema.md "\#/properties/controlledVocabulary#/properties/controlledVocabulary")                   |
| [language](#language)                                     | Merged   | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-language-schema.md "\#/properties/language#/properties/language")                                                       |
| [format](#format)                                         | Merged   | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-format-schema.md "\#/properties/format#/properties/format")                                                             |
| [fileSize](#fileSize)                                     | `string` | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-filesize-schema.md "\#/properties/fileSize#/properties/fileSize")                                                       |
| [creator](#creator)                                       | `string` | Required | cannot be null | [HDR UK Dataset](dataset-properties-the-creator-schema.md "\#/properties/creator#/properties/creator")                                                          |
| [citations](#citations)                                   | Merged   | Optional | cannot be null | [HDR UK Dataset](dataset-properties-the-citations-schema.md "\#/properties/citations#/properties/citations")                                                    |
| [doi](#doi)                                               | Merged   | Required | cannot be null | [HDR UK Dataset](dataset-properties-digital-object-identifier.md "\#/properties/doi#/properties/doi")                                                           |
| Additional Properties                                     | Any      | Optional | can be null    |                                                                                                                                                                 |

## id

Dataset identifier


`id`

-   is required
-   Type: `string` ([Dataset identifier](dataset-properties-dataset-identifier.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-dataset-identifier.md "\#/properties/id#/properties/id")

### id Type

`string` ([Dataset identifier](dataset-properties-dataset-identifier.md))

### id Constraints

**maximum length**: the maximum number of characters for this string is: `36`

**minimum length**: the minimum number of characters for this string is: `36`

**pattern**: the string must match the following regular expression: 

```regexp
^[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}$
```

[try pattern](https://regexr.com/?expression=%5E%5Ba-fA-F0-9%5D%7B8%7D-%5Ba-fA-F0-9%5D%7B4%7D-%5Ba-fA-F0-9%5D%7B4%7D-%5Ba-fA-F0-9%5D%7B4%7D-%5Ba-fA-F0-9%5D%7B12%7D%24 "try regular expression with regexr.com")

## identifier

Local dataset identifier


> FIX SPEC: Conforms to spec, but this MAY be an array of strings. FIXME: Rename to local identifier
>

`identifier`

-   is optional
-   Type: merged type ([Local dataset identifier](dataset-properties-local-dataset-identifier.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-local-dataset-identifier.md "\#/properties/identifier#/properties/identifier")

### identifier Type

merged type ([Local dataset identifier](dataset-properties-local-dataset-identifier.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-local-dataset-identifier-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-local-dataset-identifier-anyof-1.md "check type definition")

## title

Name of the dataset limited to 80 characters. It should provide a short description of the dataset and be unique across the gateway. If your title is not unique, please add a prefix with your organisation name or identifier to differentiate it from other datasets within the Gateway. Please avoid acronyms wherever possible. Good titles should summarise the content of the dataset and if relevant, the region the dataset covers.


`title`

-   is required
-   Type: `string` ([Dataset title](dataset-properties-dataset-title.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-dataset-title.md "\#/properties/title#/properties/title")

### title Type

`string` ([Dataset title](dataset-properties-dataset-title.md))

### title Constraints

**maximum length**: the maximum number of characters for this string is: `80`

**minimum length**: the minimum number of characters for this string is: `2`

## abstract

Provide a clear and brief descriptive signpost for researchers who are searching for data that may be relevant to their research. The abstract should allow the reader to determine the scope of the data collection and accurately summarise its content. The optimal length is one paragraph (limited to 255 characters) and effective abstracts should avoid long sentences and abbreviations where possible


`abstract`

-   is required
-   Type: `string` ([Dataset abstract](dataset-properties-dataset-abstract.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-dataset-abstract.md "\#/properties/abstract#/properties/abstract")

### abstract Type

`string` ([Dataset abstract](dataset-properties-dataset-abstract.md))

### abstract Constraints

**maximum length**: the maximum number of characters for this string is: `255`

**minimum length**: the minimum number of characters for this string is: `5`

## publisher

This is the organisation responsible for running or supporting the data access request process, as well as publishing and maintaining the metadata. In most this will be the same as the HDR UK Organisation (Hub or Alliance Member). However, in some cases this will be different i.e. Tissue Directory are an HDR UK Gateway organisation but coordinate activities across a number of data publishers i.e. Cambridge Blood and Stem Cell Biobank.


> Conforms to spec, but this MAY be an an object of organisation
>

`publisher`

-   is required
-   Type: `string` ([Dataset publisher](dataset-properties-dataset-publisher.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-dataset-publisher.md "\#/properties/publisher#/properties/publisher")

### publisher Type

`string` ([Dataset publisher](dataset-properties-dataset-publisher.md))

### publisher Constraints

**maximum length**: the maximum number of characters for this string is: `80`

**minimum length**: the minimum number of characters for this string is: `2`

## contactPoint

An explanation about the purpose of this instance.


`contactPoint`

-   is required
-   Type: `string` ([The contactPoint schema](dataset-properties-the-contactpoint-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-contactpoint-schema.md "\#/properties/contactPoint#/properties/contactPoint")

### contactPoint Type

`string` ([The contactPoint schema](dataset-properties-the-contactpoint-schema.md))

### contactPoint Constraints

**email**: the string must be an email address, according to [RFC 5322, section 3.4.1](https://tools.ietf.org/html/rfc5322 "check the specification")

## accessRights

The URL of a webpage where the data access request process and/or guidance is provided. If there is more than one access process i.e. industry vs academic please provide both. If such a resource or the underlying process doesn’t exist, please provide “In Progress”, until both the process and the documentation are ready.


> FIXME: Conforms to spec, but this SHOULD be an array or URIs as cardinality is 1:\*
>

`accessRights`

-   is required
-   Type: merged type ([The accessRights schema](dataset-properties-the-accessrights-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-accessrights-schema.md "\#/properties/accessRights#/properties/accessRights")

### accessRights Type

merged type ([The accessRights schema](dataset-properties-the-accessrights-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-accessrights-schema-anyof-0.md "check type definition")
-   [Untitled string in HDR UK Dataset](dataset-properties-the-accessrights-schema-anyof-1.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-accessrights-schema-anyof-2.md "check type definition")

## group

An explanation about the purpose of this instance.


> Conforms to spec, but this MAY be an array of groups
>

`group`

-   is optional
-   Type: `string` ([The group schema](dataset-properties-the-group-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-group-schema.md "\#/properties/group#/properties/group")

### group Type

`string` ([The group schema](dataset-properties-the-group-schema.md))

## description

A free-text account of the record. An html account of the data that provides context and scope of the data (limited to 50,000 characters) and/or a resolvable URL that describes the dataset.


`description`

-   is optional
-   Type: merged type ([The description schema](dataset-properties-the-description-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-description-schema.md "\#/properties/description#/properties/description")

### description Type

merged type ([The description schema](dataset-properties-the-description-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-description-schema-anyof-0.md "check type definition")
-   [Untitled string in HDR UK Dataset](dataset-properties-the-description-schema-anyof-1.md "check type definition")

## media

Please provide any media associated with the Gateway Organisation using a valid URI. This is an opportunity to provide additional context that could be useful for researchers wanting to undestand more about the dataset and its relevance to their research question. The following formats will be accepted .jpg, .png or .svg, .pdf, .xslx or .docx.


> FIXME: Conforms to spec, but this SHOULD to be an array of URIs as cardinality 0:\*
>

`media`

-   is optional
-   Type: merged type ([The media schema](dataset-properties-the-media-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-media-schema.md "\#/properties/media#/properties/media")

### media Type

merged type ([The media schema](dataset-properties-the-media-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-media-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-media-schema-anyof-1.md "check type definition")

## purpose

Pleases indicate the purpose(s) that the dataset was collected. Multiple purposes may be provided


> FIXME: Mandatory, but cardinality 0:\* Possibly deprecate.
>

`purpose`

-   is optional
-   Type: merged type ([The purpose schema](dataset-properties-the-purpose-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-purpose-schema.md "\#/properties/purpose#/properties/purpose")

### purpose Type

merged type ([The purpose schema](dataset-properties-the-purpose-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-purpose-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-purpose-schema-anyof-1.md "check type definition")

## source

Pleases indicate the source(s) that the dataset was collected. Multiple source(s) may be provided


> FIXME: Mandatory, but cardinality 0:\* Possibly deprecate.
>

`source`

-   is optional
-   Type: merged type ([The source schema](dataset-properties-the-source-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-source-schema.md "\#/properties/source#/properties/source")

### source Type

merged type ([The source schema](dataset-properties-the-source-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-source-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-source-schema-anyof-1.md "check type definition")

## setting

Pleases indicate the setting(s) where data was collected. Multiple settings may be provided.


> FIXME: Mandatory, but cardinality 0:\*. Possibly deprecate.
>

`setting`

-   is optional
-   Type: merged type ([The setting schema](dataset-properties-the-setting-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-setting-schema.md "\#/properties/setting#/properties/setting")

### setting Type

merged type ([The setting schema](dataset-properties-the-setting-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-setting-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-setting-schema-anyof-1.md "check type definition")

## releaseDate

An explanation about the purpose of this instance.


`releaseDate`

-   is optional
-   Type: `string` ([The releaseDate schema](dataset-properties-the-releasedate-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-releasedate-schema.md "\#/properties/releaseDate#/properties/releaseDate")

### releaseDate Type

`string` ([The releaseDate schema](dataset-properties-the-releasedate-schema.md))

### releaseDate Constraints

**date time**: the string must be a date time string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## accessRequestCost

An explanation about the purpose of this instance.


`accessRequestCost`

-   is required
-   Type: `string` ([The accessRequestCost schema](dataset-properties-the-accessrequestcost-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-accessrequestcost-schema.md "\#/properties/accessRequestCost#/properties/accessRequestCost")

### accessRequestCost Type

`string` ([The accessRequestCost schema](dataset-properties-the-accessrequestcost-schema.md))

## accessRequestDuration

Please provide an indication of the typical processing times based on the types of requests typically received.


`accessRequestDuration`

-   is optional
-   Type: `string` ([The accessRequestDuration schema](dataset-properties-the-accessrequestduration-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-accessrequestduration-schema.md "\#/properties/accessRequestDuration#/properties/accessRequestDuration")

### accessRequestDuration Type

`string` ([The accessRequestDuration schema](dataset-properties-the-accessrequestduration-schema.md))

### accessRequestDuration Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | ----------- |
| `"<1 Week"`    |             |
| `"1-2 Weeks"`  |             |
| `"2-4 Weeks"`  |             |
| `"1-2 Months"` |             |
| `"2-6 Months"` |             |
| `">6 Months"`  |             |
| `"Other"`      |             |

## accessEnvironment

Please provide a brief description of the data access environment that is currently available to researchers.


`accessEnvironment`

-   is optional
-   Type: `string` ([The accessEnvironment schema](dataset-properties-the-accessenvironment-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-accessenvironment-schema.md "\#/properties/accessEnvironment#/properties/accessEnvironment")

### accessEnvironment Type

`string` ([The accessEnvironment schema](dataset-properties-the-accessenvironment-schema.md))

### accessEnvironment Constraints

**maximum length**: the maximum number of characters for this string is: `5000`

**minimum length**: the minimum number of characters for this string is: `5`

## usageRestrictions

Please provide a description of any usage restrictions of key terms and conditions under which access to the dataset is provided.


> FIXME: Missing from Onboarding tool, so not captured
>

`usageRestrictions`

-   is required
-   Type: merged type ([The usageRestrictions schema](dataset-properties-the-usagerestrictions-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-usagerestrictions-schema.md "\#/properties/usageRestrictions#/properties/usageRestrictions")

### usageRestrictions Type

merged type ([The usageRestrictions schema](dataset-properties-the-usagerestrictions-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-usagerestrictions-schema-anyof-0.md "check type definition")
-   [Untitled string in HDR UK Dataset](dataset-properties-the-usagerestrictions-schema-anyof-1.md "check type definition")

## dataController

Data Controller means a person/entity who (either alone or jointly or in common with other persons/entities) determines the purposes for which and the way any Data Subject data, specifically personal data or are to be processed.


`dataController`

-   is required
-   Type: `string` ([The dataController schema](dataset-properties-the-datacontroller-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-datacontroller-schema.md "\#/properties/dataController#/properties/dataController")

### dataController Type

`string` ([The dataController schema](dataset-properties-the-datacontroller-schema.md))

### dataController Constraints

**maximum length**: the maximum number of characters for this string is: `5000`

**minimum length**: the minimum number of characters for this string is: `5`

## dataProcessor

A Data Processor, in relation to any Data Subject data, specifically personal data, means any person/entity (other than an employee of the data controller) who processes the data on behalf of the data controller.


`dataProcessor`

-   is optional
-   Type: merged type ([The dataProcessor schema](dataset-properties-the-dataprocessor-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-dataprocessor-schema.md "\#/properties/dataProcessor#/properties/dataProcessor")

### dataProcessor Type

merged type ([The dataProcessor schema](dataset-properties-the-dataprocessor-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-dataprocessor-schema-anyof-0.md "check type definition")
-   [Untitled string in HDR UK Dataset](dataset-properties-the-dataprocessor-schema-anyof-1.md "check type definition")

## license

An explanation about the purpose of this instance.


`license`

-   is required
-   Type: `string` ([The license schema](dataset-properties-the-license-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-license-schema.md "\#/properties/license#/properties/license")

### license Type

`string` ([The license schema](dataset-properties-the-license-schema.md))

## derivedDatasets

Indicate if derived datasets or predefined extracts are available and the type of derivation available.


> FIXME: Conforms to spec, but this SHOULD to be an array of datasets as cardinality 0:\*
>

`derivedDatasets`

-   is optional
-   Type: merged type ([The derivedDatasets schema](dataset-properties-the-deriveddatasets-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-deriveddatasets-schema.md "\#/properties/derivedDatasets#/properties/derivedDatasets")

### derivedDatasets Type

merged type ([The derivedDatasets schema](dataset-properties-the-deriveddatasets-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-deriveddatasets-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-deriveddatasets-schema-anyof-1.md "check type definition")
-   [Untitled string in HDR UK Dataset](dataset-properties-the-deriveddatasets-schema-anyof-2.md "check type definition")

## linkedDataset

If applicable, please provide the DOI of other datasets that have previously been linked to this dataset and their availability. If no DOI is available, please provide the title of the datasets that can be linked, where possible using the same title of a dataset previously onboarded.


> FIXME: If linked $title must start with 'Linked'. FIXME: Conforms to spec, but this SHOULD to be an array of datasets as cardinality 0:\*
>

`linkedDataset`

-   is optional
-   Type: merged type ([The linkedDataset schema](dataset-properties-the-linkeddataset-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-linkeddataset-schema.md "\#/properties/linkedDataset#/properties/linkedDataset")

### linkedDataset Type

merged type ([The linkedDataset schema](dataset-properties-the-linkeddataset-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-linkeddataset-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-linkeddataset-schema-anyof-1.md "check type definition")
-   [Untitled string in HDR UK Dataset](dataset-properties-the-linkeddataset-schema-anyof-2.md "check type definition")

## linkageOpportunity

If applicable, please indicate if there is the opportunity to link this dataset to additional data sources. If possible, please describe the data elements that could be used to link to external data sources i.e. region or postcode could be used to link to open datasets such as air pollution or deprivation indices. In addition, please describe the restricted data elements that cannot be used to link to other datasets.


`linkageOpportunity`

-   is optional
-   Type: `string` ([The linkageOpportunity schema](dataset-properties-the-linkageopportunity-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-linkageopportunity-schema.md "\#/properties/linkageOpportunity#/properties/linkageOpportunity")

### linkageOpportunity Type

`string` ([The linkageOpportunity schema](dataset-properties-the-linkageopportunity-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-linkageopportunity-schema-anyof-0.md "check type definition")
-   [Untitled string in HDR UK Dataset](dataset-properties-the-linkageopportunity-schema-anyof-1.md "check type definition")

## geographicCoverage

The geographical area covered by the dataset.


> FIXME: Update to geoname pattern
>

`geographicCoverage`

-   is optional
-   Type: `string` ([The geographicCoverage schema](dataset-properties-the-geographiccoverage-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-geographiccoverage-schema.md "\#/properties/geographicCoverage#/properties/geographicCoverage")

### geographicCoverage Type

`string` ([The geographicCoverage schema](dataset-properties-the-geographiccoverage-schema.md))

### geographicCoverage Constraints

**URI**: the string must be a URI, according to [RFC 3986](https://tools.ietf.org/html/rfc4291 "check the specification")

### geographicCoverage Examples

```json
"GB"
```

## periodicity

The frequency at which dataset is published.


`periodicity`

-   is required
-   Type: `string` ([The periodicity schema](dataset-properties-the-periodicity-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-periodicity-schema.md "\#/properties/periodicity#/properties/periodicity")

### periodicity Type

`string` ([The periodicity schema](dataset-properties-the-periodicity-schema.md))

### periodicity Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | ----------- |
| `"Static"`     |             |
| `"Annual"`     |             |
| `"Biennial"`   |             |
| `"Quaterly"`   |             |
| `"Bimonthly"`  |             |
| `"Monthly"`    |             |
| `"Biweekly"`   |             |
| `"Daily"`      |             |
| `"Irregular"`  |             |
| `"Continious"` |             |

## datasetEndDate

The end of the time period that the dataset provides coverage for.


`datasetEndDate`

-   is optional
-   Type: `string` ([The datasetEndDate schema](dataset-properties-the-datasetenddate-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-datasetenddate-schema.md "\#/properties/datasetEndDate#/properties/datasetEndDate")

### datasetEndDate Type

`string` ([The datasetEndDate schema](dataset-properties-the-datasetenddate-schema.md))

### datasetEndDate Constraints

**date**: the string must be a date string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## datasetStartDate

The start of the time period that the dataset provides coverage for.


`datasetStartDate`

-   is required
-   Type: `string` ([The datasetStartDate schema](dataset-properties-the-datasetstartdate-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-datasetstartdate-schema.md "\#/properties/datasetStartDate#/properties/datasetStartDate")

### datasetStartDate Type

`string` ([The datasetStartDate schema](dataset-properties-the-datasetstartdate-schema.md))

### datasetStartDate Constraints

**date**: the string must be a date string, according to [RFC 3339, section 5.6](https://tools.ietf.org/html/rfc3339 "check the specification")

## jurisdiction

Please use country code from ISO 3166-1 country codes and the associated ISO 3166-2 for regions, cities, states etc. for the country/state under whose laws the data subjects’ data is collected, processed and stored.


> FIXME: Add ISO 3166-2 Subdivision code pattern
>

`jurisdiction`

-   is required
-   Type: `string` ([The jurisdiction schema](dataset-properties-the-jurisdiction-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-jurisdiction-schema.md "\#/properties/jurisdiction#/properties/jurisdiction")

### jurisdiction Type

`string` ([The jurisdiction schema](dataset-properties-the-jurisdiction-schema.md))

### jurisdiction Constraints

**pattern**: the string must match the following regular expression: 

```regexp
^[A-Z]{2}(-[A-Z]{2,3})?$
```

[try pattern](https://regexr.com/?expression=%5E%5BA-Z%5D%7B2%7D(-%5BA-Z%5D%7B2%2C3%7D)%3F%24 "try regular expression with regexr.com")

## populationType

Please provide a valid SNOMED CT concept that describes the measure within the dataset i.e. participants in a study, modality, or images with certain characteristics.


> FIXME: Check against SNOMED-CT TERMS. Conforms to spec but MAY be array of strings
>

`populationType`

-   is required
-   Type: merged type ([The populationType schema](dataset-properties-the-populationtype-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-populationtype-schema.md "\#/properties/populationType#/properties/populationType")

### populationType Type

merged type ([The populationType schema](dataset-properties-the-populationtype-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-populationtype-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-populationtype-schema-anyof-1.md "check type definition")

## disabmiguatingDescription

If SNOMED CT term does not provide sufficient detail, please provide a description that disambiguates the population type.


> FIXME: Rename MDC response to ageRange according to spec
>

`disabmiguatingDescription`

-   is optional
-   Type: `string` ([The disabmiguatingDescription schema](dataset-properties-the-disabmiguatingdescription-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-disabmiguatingdescription-schema.md "\#/properties/disabmiguatingDescription#/properties/disabmiguatingDescription")

### disabmiguatingDescription Type

`string` ([The disabmiguatingDescription schema](dataset-properties-the-disabmiguatingdescription-schema.md))

### disabmiguatingDescription Constraints

**pattern**: the string must match the following regular expression: 

```regexp
\d{1,3}-\d{1,3}
```

[try pattern](https://regexr.com/?expression=%5Cd%7B1%2C3%7D-%5Cd%7B1%2C3%7D "try regular expression with regexr.com")

## statisticalPopulation

An explanation about the purpose of this instance.


> FIXME: Spec calls this Measured Value
>

`statisticalPopulation`

-   is required
-   Type: merged type ([The statisticalPopulation schema](dataset-properties-the-statisticalpopulation-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-statisticalpopulation-schema.md "\#/properties/statisticalPopulation#/properties/statisticalPopulation")

### statisticalPopulation Type

merged type ([The statisticalPopulation schema](dataset-properties-the-statisticalpopulation-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-statisticalpopulation-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-statisticalpopulation-schema-anyof-1.md "check type definition")

## ageBand

Please indicate the age range in whole years of participants in the dataset. Please provide range in the following format ‘[min age] – [max age]’ where both the minimum and maximum are whole numbers (integers).


> FIXME: Rename MDC response to ageRange according to spec
>

`ageBand`

-   is optional
-   Type: `string` ([The ageBand schema](dataset-properties-the-ageband-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-ageband-schema.md "\#/properties/ageBand#/properties/ageBand")

### ageBand Type

`string` ([The ageBand schema](dataset-properties-the-ageband-schema.md))

### ageBand Constraints

**pattern**: the string must match the following regular expression: 

```regexp
\d{1,3}-\d{1,3}
```

[try pattern](https://regexr.com/?expression=%5Cd%7B1%2C3%7D-%5Cd%7B1%2C3%7D "try regular expression with regexr.com")

## physicalSampleAvailability

Availability of physical samples associated with the dataset. If samples are available, please indicate the types of samples that are available.


`physicalSampleAvailability`

-   is required
-   Type: `string` ([The physicalSampleAvailability schema](dataset-properties-the-physicalsampleavailability-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-physicalsampleavailability-schema.md "\#/properties/physicalSampleAvailability#/properties/physicalSampleAvailability")

### physicalSampleAvailability Type

`string` ([The physicalSampleAvailability schema](dataset-properties-the-physicalsampleavailability-schema.md))

### physicalSampleAvailability Constraints

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

### physicalSampleAvailability Examples

```json
"Not Available"
```

## keywords

An explanation about the purpose of this instance.


> Conforms to spec, but this MAY be an array of strings
>

`keywords`

-   is required
-   Type: `string` ([The keywords schema](dataset-properties-the-keywords-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-keywords-schema.md "\#/properties/keywords#/properties/keywords")

### keywords Type

`string` ([The keywords schema](dataset-properties-the-keywords-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-keywords-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-keywords-schema-anyof-1.md "check type definition")

### keywords Constraints

**pattern**: the string must match the following regular expression: 

```regexp
[0-9a-zA-Z._\-]+(,[0-9a-zA-Z.\-_]+)*
```

[try pattern](https://regexr.com/?expression=%5B0-9a-zA-Z._%5C-%5D%2B(%2C%5B0-9a-zA-Z.%5C-_%5D%2B)* "try regular expression with regexr.com")

## conformsTo

An explanation about the purpose of this instance.


`conformsTo`

-   is required
-   Type: `string` ([The conformsTo schema](dataset-properties-the-conformsto-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-conformsto-schema.md "\#/properties/conformsTo#/properties/conformsTo")

### conformsTo Type

`string` ([The conformsTo schema](dataset-properties-the-conformsto-schema.md))

### conformsTo Constraints

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
| `"LOCAL"`    |             |
| `"OTHER"`    |             |

## controlledVocabulary

List any relevant terminologies / ontologies / controlled vocabularies, such as ICD 10 Codes, NHS Data Dictionary National Codes or SNOMED CT International, that are being used by the dataset.


> FIXME: Confroms to spec, but MAY be a list of strings
>

`controlledVocabulary`

-   is optional
-   Type: merged type ([The controlledVocabulary schema](dataset-properties-the-controlledvocabulary-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-controlledvocabulary-schema.md "\#/properties/controlledVocabulary#/properties/controlledVocabulary")

### controlledVocabulary Type

merged type ([The controlledVocabulary schema](dataset-properties-the-controlledvocabulary-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-controlledvocabulary-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-controlledvocabulary-schema-anyof-1.md "check type definition")

### controlledVocabulary Examples

```json
"See ConformsTo"
```

## language

This should list all the languages in which the dataset metadata and underlying data is made available.


> FIXME: Conforms to spec, but may be a list of strings given cardinality 1:\*. Validate against external list of languages. Resources defined by the Library of Congress (ISO 639-1, ISO 639-2) SHOULD be used.
>

`language`

-   is required
-   Type: merged type ([The language schema](dataset-properties-the-language-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-language-schema.md "\#/properties/language#/properties/language")

### language Type

merged type ([The language schema](dataset-properties-the-language-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-language-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-language-schema-anyof-1.md "check type definition")

## format

If multiple formats are available please specify.


> FIXME: Conforms to spec, but may be a list of strings given cardinality 1:\*. Validate against external list of formats, e.g. <https://www.iana.org/assignments/media-types/media-types.xhtml>
>

`format`

-   is required
-   Type: merged type ([The format schema](dataset-properties-the-format-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-format-schema.md "\#/properties/format#/properties/format")

### format Type

merged type ([The format schema](dataset-properties-the-format-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-format-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-format-schema-anyof-1.md "check type definition")

## fileSize

An explanation about the purpose of this instance.


`fileSize`

-   is optional
-   Type: `string` ([The fileSize schema](dataset-properties-the-filesize-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-filesize-schema.md "\#/properties/fileSize#/properties/fileSize")

### fileSize Type

`string` ([The fileSize schema](dataset-properties-the-filesize-schema.md))

### fileSize Examples

```json
"301MB"
```

## creator

Please provide the text that you would like included as part of any citation that credits this dataset. This is typically just the name of the publisher. No employee details should be provided.


`creator`

-   is required
-   Type: `string` ([The creator schema](dataset-properties-the-creator-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-creator-schema.md "\#/properties/creator#/properties/creator")

### creator Type

`string` ([The creator schema](dataset-properties-the-creator-schema.md))

## citations

Please provide the keystone paper associated with the dataset. Also include a list of known citations, if available and should be links to existing resources where the dataset has been used or referenced.


> FIXME: Conforms to spec, but may be a list of citation strings
>

`citations`

-   is optional
-   Type: merged type ([The citations schema](dataset-properties-the-citations-schema.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-the-citations-schema.md "\#/properties/citations#/properties/citations")

### citations Type

merged type ([The citations schema](dataset-properties-the-citations-schema.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-the-citations-schema-anyof-0.md "check type definition")
-   [Untitled array in HDR UK Dataset](dataset-properties-the-citations-schema-anyof-1.md "check type definition")

## doi

All HDR UK registered datasets should either have a Digital Object Identifier (DOI) or be working towards obtaining one. If a DOI is available, please provide the DOI.


`doi`

-   is required
-   Type: merged type ([Digital Object Identifier](dataset-properties-digital-object-identifier.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-properties-digital-object-identifier.md "\#/properties/doi#/properties/doi")

### doi Type

merged type ([Digital Object Identifier](dataset-properties-digital-object-identifier.md))

any of

-   [Untitled string in HDR UK Dataset](dataset-properties-digital-object-identifier-anyof-0.md "check type definition")
-   [Untitled string in HDR UK Dataset](dataset-properties-digital-object-identifier-anyof-1.md "check type definition")

## Additional Properties

Additional properties are allowed and do not have to follow a specific schema
