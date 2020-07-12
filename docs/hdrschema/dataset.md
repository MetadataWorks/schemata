---
title: HDR UK Dataset Schema
layout: home
---
 

```txt
http://healthdatagateway.org/schema/dataset.json
```

HDR UK Dataset Schema


| Abstract               | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                               |
| :--------------------- | ---------- | -------------- | ----------------------- | :---------------- | --------------------- | ------------------- | ------------------------------------------------------------------------ |
| Cannot be instantiated | Yes        | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [dataset.schema.json](../out/dataset.schema.json "open original schema") |

## HDR UK Dataset Type

`object` ([HDR UK Dataset](dataset.md))

all of

-   [Descriptive Metadata](dataset-definitions-descriptive-metadata.md "check type definition")

# HDR UK Dataset Definitions

## Definitions group physicalsampleavailability

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/physicalsampleavailability"}
```




`physicalsampleavailability`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-physicalsampleavailability.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/physicalsampleavailability")

### physicalsampleavailability Type

`string`

### physicalsampleavailability Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                            | Explanation |
| :------------------------------- | ----------- |
| `"NOT AVAILABLE"`                |             |
| `"BONE MARROW"`                  |             |
| `"CANCER CELL LINES"`            |             |
| `"CORE BIOPSY"`                  |             |
| `"CDNA/MRNA"`                    |             |
| `"DNA"`                          |             |
| `"FAECES"`                       |             |
| `"IMMORTALIZED CELL LINES"`      |             |
| `"MICRORNA"`                     |             |
| `"PERIPHERAL BLOOD CELLS"`       |             |
| `"PLASMA"`                       |             |
| `"PM TISSUE"`                    |             |
| `"PRIMARY CELLS"`                |             |
| `"RNA"`                          |             |
| `"SALIVA"`                       |             |
| `"SERUM"`                        |             |
| `"SWABS"`                        |             |
| `"TISSUE"`                       |             |
| `"URINE"`                        |             |
| `"WHOLE BLOOD"`                  |             |
| `"AVAILABILITY TO BE CONFIRMED"` |             |

## Definitions group followup

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/followup"}
```




`followup`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-followup.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/followup")

### followup Type

`string`

### followup Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value             | Explanation |
| :---------------- | ----------- |
| `"0 - 6 MONTHS"`  |             |
| `"6 - 12 MONTHS"` |             |
| `"1 - 10 YEARS"`  |             |
| `"> 10 YEARS"`    |             |
| `"UNKNOWN"`       |             |

## Definitions group purpose

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/purpose"}
```




`purpose`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-purpose.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/purpose")

### purpose Type

`string`

### purpose Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                | Explanation |
| :------------------- | ----------- |
| `"STUDY"`            |             |
| `"DISEASE REGISTRY"` |             |
| `"TRIAL"`            |             |
| `"CARE"`             |             |
| `"AUDIT"`            |             |
| `"ADMINISTRATIVE"`   |             |
| `"FINANCIAL"`        |             |
| `"OTHER"`            |             |

## Definitions group source

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/source"}
```




`source`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-source.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/source")

### source Type

`string`

### source Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                  | Explanation |
| :--------------------- | ----------- |
| `"EPR"`                |             |
| `"ELECTRONIC SURVEY"`  |             |
| `"LIMS"`               |             |
| `"PAPER BASED "`       |             |
| `"FREETEXT NLP"`       |             |
| `"MACHINE GENERATED "` |             |
| `"OTHER"`              |             |

## Definitions group setting

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/setting"}
```




`setting`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-setting.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/setting")

### setting Type

`string`

### setting Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                     | Explanation |
| :------------------------ | ----------- |
| `"CLINIC"`                |             |
| `"PRIMARY CARE"`          |             |
| `"ACCIDENT AN EMERGENCY"` |             |
| `"OUTPATIENTS"`           |             |
| `"IN-PATIENTS  "`         |             |
| `"SERVICES"`              |             |
| `"COMMUNITY "`            |             |
| `"HOME"`                  |             |
| `"PRIVATE"`               |             |
| `"PHARMACY"`              |             |
| `"OTHER"`                 |             |

## Definitions group periodicity

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/periodicity"}
```




`periodicity`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-periodicity.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/periodicity")

### periodicity Type

`string`

### periodicity Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | ----------- |
| `"STATIC"`     |             |
| `"ANNUAL"`     |             |
| `"BIENNIAL"`   |             |
| `"QUARTERLY"`  |             |
| `"BIMONTHLY"`  |             |
| `"MONTHLY"`    |             |
| `"BIWEEKLY"`   |             |
| `"WEEKLY"`     |             |
| `"SEMIWEEKLY"` |             |
| `"DAILY"`      |             |
| `"IRREGULAR"`  |             |
| `"CONTINUOUS"` |             |

## Definitions group timelag

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/timelag"}
```




`timelag`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-timelag.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/timelag")

### timelag Type

`string`

### timelag Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | ----------- |
| `">1 WEEK"`    |             |
| `"1-2 WEEKS"`  |             |
| `"2-4 WEEKS"`  |             |
| `"1-2 MONTHS"` |             |
| `"2-6 MONTHS"` |             |
| `">6 MONTHS"`  |             |
| `"VARIABLE"`   |             |
| `"NA"`         |             |

## Definitions group datauselimitation

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/datauselimitation"}
```




`datauselimitation`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-datauselimitation.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/datauselimitation")

### datauselimitation Type

`string`

### datauselimitation Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                              | Explanation |
| :--------------------------------- | ----------- |
| `"GENERAL RESEARCH USE"`           |             |
| `"GENETIC STUDIES ONLY"`           |             |
| `"NO GENERAL METHODS RESEARCH"`    |             |
| `"NO RESTRICTION"`                 |             |
| `"RESEARCH SPECIFIC RESTRICTIONS"` |             |
| `"RESEARCH USE ONLY"`              |             |
| `"NO LINKAGE"`                     |             |

## Definitions group datauserequirements

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/datauserequirements"}
```




`datauserequirements`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-datauserequirements.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/datauserequirements")

### datauserequirements Type

`string`

### datauserequirements Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                                 | Explanation |
| :------------------------------------ | ----------- |
| `"COLLABORATION REQUIRED"`            |             |
| `"ETHICS APPROVAL REQUIRED"`          |             |
| `"GEOGRAPHICAL RESTRICTIONS"`         |             |
| `"INSTITUTION SPECIFIC RESTRICTIONS"` |             |
| `"NOT FOR PROFIT USE"`                |             |
| `"PROJECT SPECIFIC RESTRICTIONS"`     |             |
| `"PUBLICATION MORATORIUM"`            |             |
| `"PUBLICATION REQUIRED"`              |             |
| `"RETURN TO DATABASE OR RESOURCE"`    |             |
| `"TIME LIMIT ON USE"`                 |             |
| `"USER SPECIFIC RESTRICTION"`         |             |

## Definitions group accessrequestduration

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/accessrequestduration"}
```




`accessrequestduration`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-accessrequestduration.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/accessrequestduration")

### accessrequestduration Type

`string`

### accessrequestduration Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | ----------- |
| `">1 WEEK"`    |             |
| `"1-2 WEEKS"`  |             |
| `"2-4 WEEKS"`  |             |
| `"1-2 MONTHS"` |             |
| `"2-6 MONTHS"` |             |
| `">6 MONTHS"`  |             |
| `"OTHER"`      |             |

## Definitions group standardiseddatamodels

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/standardiseddatamodels"}
```




`standardiseddatamodels`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-standardiseddatamodels.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/standardiseddatamodels")

### standardiseddatamodels Type

`string`

### standardiseddatamodels Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value         | Explanation |
| :------------ | ----------- |
| `"HL7 FHIR "` |             |
| `"HL7 V2"`    |             |
| `"HL7 CDA"`   |             |
| `"HL7 CCOW"`  |             |
| `"LOINC"`     |             |
| `"DICOM"`     |             |
| `"I2B2"`      |             |
| `"IHE"`       |             |
| `"OMOP"`      |             |
| `"OPENEHR"`   |             |
| `"SENTINEL"`  |             |
| `"PCORNET"`   |             |
| `"CDISC"`     |             |
| `"LOCAL"`     |             |
| `"OTHER"`     |             |

## Definitions group controlledvocabulary

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/controlledvocabulary"}
```




`controlledvocabulary`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-controlledvocabulary.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/controlledvocabulary")

### controlledvocabulary Type

`string`

### controlledvocabulary Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value                   | Explanation |
| :---------------------- | ----------- |
| `"LOCAL"`               |             |
| `"OPCS4"`               |             |
| `"READ "`               |             |
| `"SNOMED CT "`          |             |
| `"SNOMED RT "`          |             |
| `"DM+D"`                |             |
| `"NHS NATIONAL CODES "` |             |
| `"ODS "`                |             |
| `"LOINC "`              |             |
| `"ICD10 "`              |             |
| `"ICD10CM "`            |             |
| `"ICD10PCS "`           |             |
| `"ICD9CM "`             |             |
| `"ICD9"`                |             |
| `"ICDO3 "`              |             |
| `"AMT "`                |             |
| `"APC "`                |             |
| `"ATC "`                |             |
| `"CIEL "`               |             |
| `"HPO"`                 |             |
| `"CPT4 "`               |             |
| `"DPD "`                |             |
| `"DRG "`                |             |
| `"HEMONC"`              |             |
| `"JMDC "`               |             |
| `"KCD7 "`               |             |
| `"MULTUM"`              |             |
| `"NAACCR"`              |             |
| `"NDC"`                 |             |
| `"NDFRT "`              |             |
| `"OXMIS "`              |             |
| `"RXNORM"`              |             |
| `"RXNORM EXTENSION "`   |             |
| `"SPL "`                |             |
| `"OTHER "`              |             |

## Definitions group statisticalpopulationcontrained

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/statisticalpopulationcontrained"}
```




`statisticalpopulationcontrained`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-statisticalpopulationcontrained.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/statisticalpopulationcontrained")

### statisticalpopulationcontrained Type

`string`

### statisticalpopulationcontrained Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value        | Explanation |
| :----------- | ----------- |
| `"Persons"`  |             |
| `"Events"`   |             |
| `"Findings"` |             |

## Definitions group eightycharacters

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/eightycharacters"}
```




`eightycharacters`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-eightycharacters.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/eightycharacters")

### eightycharacters Type

`string`

### eightycharacters Constraints

**maximum length**: the maximum number of characters for this string is: `80`

**minimum length**: the minimum number of characters for this string is: `1`

## Definitions group abstract

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/abstract"}
```




`abstract`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-abstract.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/abstract")

### abstract Type

`string`

### abstract Constraints

**maximum length**: the maximum number of characters for this string is: `255`

**minimum length**: the minimum number of characters for this string is: `1`

## Definitions group email

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/email"}
```




`email`

-   is optional
-   Type: `email`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-email.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/email")

### email Type

`email`

## Definitions group commaseparatedlist

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/commaseparatedlist"}
```




`commaseparatedlist`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-commaseparatedlist.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/commaseparatedlist")

### commaseparatedlist Type

`string`

### commaseparatedlist Constraints

**pattern**: the string must match the following regular expression: 

```regexp
/[0-9a-zA-Z]+(,[0-9a-zA-Z]+)*/
```

[try pattern](https://regexr.com/?expression=%2F%5B0-9a-zA-Z%5D%2B(%2C%5B0-9a-zA-Z%5D%2B)*%2F "try regular expression with regexr.com")

## Definitions group doi

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/doi"}
```




`doi`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-doi.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/doi")

### doi Type

`string`

### doi Constraints

**pattern**: the string must match the following regular expression: 

```regexp
^10.\d{4,9}/[-._;()/:a-zA-Z0-9]+$
```

[try pattern](https://regexr.com/?expression=%5E10.%5Cd%7B4%2C9%7D%2F%5B-._%3B()%2F%3Aa-zA-Z0-9%5D%2B%24 "try regular expression with regexr.com")

## Definitions group description

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/description"}
```




`description`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-description.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/description")

### description Type

`string`

### description Constraints

**maximum length**: the maximum number of characters for this string is: `3000`

**minimum length**: the minimum number of characters for this string is: `5`

## Definitions group url

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/url"}
```




`url`

-   is optional
-   Type: `url`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-url.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/url")

### url Type

`url`

## Definitions group agerange

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/agerange"}
```




`agerange`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-agerange.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/agerange")

### agerange Type

`string`

### agerange Constraints

**pattern**: the string must match the following regular expression: 

```regexp
/(150|1[0-4][0-9]|[0-9]|[1-8][0-9]|9[0-9])-(150|1[0-4][0-9]|[0-9]|[1-8][0-9]|9[0-9])/
```

[try pattern](https://regexr.com/?expression=%2F(150%7C1%5B0-4%5D%5B0-9%5D%7C%5B0-9%5D%7C%5B1-8%5D%5B0-9%5D%7C9%5B0-9%5D)-(150%7C1%5B0-4%5D%5B0-9%5D%7C%5B0-9%5D%7C%5B1-8%5D%5B0-9%5D%7C9%5B0-9%5D)%2F "try regular expression with regexr.com")

## Definitions group longDescription

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/longDescription"}
```




`longDescription`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-longdescription.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/longDescription")

### longDescription Type

`string`

### longDescription Constraints

**maximum length**: the maximum number of characters for this string is: `5000`

**minimum length**: the minimum number of characters for this string is: `5`

## Definitions group isocountrycode

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/isocountrycode"}
```




> FIXME: Add ISO 3166-2 Subdivision code pattern
>

`isocountrycode`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-isocountrycode.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/isocountrycode")

### isocountrycode Type

`string`

### isocountrycode Constraints

**pattern**: the string must match the following regular expression: 

```regexp
^[A-Z]{2}(-[A-Z]{2,3})?$
```

[try pattern](https://regexr.com/?expression=%5E%5BA-Z%5D%7B2%7D(-%5BA-Z%5D%7B2%2C3%7D)%3F%24 "try regular expression with regexr.com")

## Definitions group linkeddatasets

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/linkeddatasets"}
```




`linkeddatasets`

-   is optional
-   Type: `url`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-linkeddatasets.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/linkeddatasets")

### linkeddatasets Type

`url`

## Definitions group format

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/format"}
```




> FIXME: Conforms to spec, but may be a list of strings given cardinality 1:\*. Validate against external list of formats, e.g. <https://www.iana.org/assignments/media-types/media-types.xhtml>
>

`format`

-   is optional
-   Type: `string`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-format.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/format")

### format Type

`string`

### format Constraints

**minimum length**: the minimum number of characters for this string is: `1`

## Definitions group descriptive-metadata

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata"}
```

Describes a resource for purposes of discovery and identification.


`descriptive-metadata`

-   is optional
-   Type: `object` ([Descriptive Metadata](dataset-definitions-descriptive-metadata.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-descriptive-metadata.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata")

### descriptive-metadata Type

`object` ([Descriptive Metadata](dataset-definitions-descriptive-metadata.md))

## Definitions group summary

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/summary"}
```




`summary`

-   is optional
-   Type: `object` ([Details](dataset-definitions-summary.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-summary.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary")

### summary Type

`object` ([Details](dataset-definitions-summary.md))

## Definitions group documentation

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/documentation"}
```




`documentation`

-   is optional
-   Type: `object` ([Details](dataset-definitions-documentation.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-documentation.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/documentation")

### documentation Type

`object` ([Details](dataset-definitions-documentation.md))

## Definitions group coverage

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/coverage"}
```




`coverage`

-   is optional
-   Type: `object` ([Details](dataset-definitions-coverage.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-coverage.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/coverage")

### coverage Type

`object` ([Details](dataset-definitions-coverage.md))

## Definitions group provenance

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/provenance"}
```




`provenance`

-   is optional
-   Type: `object` ([Details](dataset-definitions-provenance.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-provenance.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/provenance")

### provenance Type

`object` ([Details](dataset-definitions-provenance.md))

## Definitions group origin

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/origin"}
```




`origin`

-   is optional
-   Type: `object` ([Details](dataset-definitions-origin.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-origin.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/origin")

### origin Type

`object` ([Details](dataset-definitions-origin.md))

## Definitions group temporal

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/temporal"}
```




`temporal`

-   is optional
-   Type: `object` ([Details](dataset-definitions-temporal.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-temporal.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/temporal")

### temporal Type

`object` ([Details](dataset-definitions-temporal.md))

## Definitions group accessibility

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/accessibility"}
```




`accessibility`

-   is optional
-   Type: `object` ([Details](dataset-definitions-accessibility.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-accessibility.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/accessibility")

### accessibility Type

`object` ([Details](dataset-definitions-accessibility.md))

## Definitions group usage

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/usage"}
```




`usage`

-   is optional
-   Type: `object` ([Details](dataset-definitions-usage.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-usage.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/usage")

### usage Type

`object` ([Details](dataset-definitions-usage.md))

## Definitions group access

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/access"}
```




`access`

-   is optional
-   Type: `object` ([Details](dataset-definitions-access.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-access.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access")

### access Type

`object` ([Details](dataset-definitions-access.md))

## Definitions group formatStandards

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/formatStandards"}
```




`formatStandards`

-   is optional
-   Type: `object` ([Details](dataset-definitions-formatstandards.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-formatstandards.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/formatStandards")

### formatStandards Type

`object` ([Details](dataset-definitions-formatstandards.md))

## Definitions group enrichmentLinkage

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/enrichmentLinkage"}
```




`enrichmentLinkage`

-   is optional
-   Type: `object` ([Details](dataset-definitions-enrichmentlinkage.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-enrichmentlinkage.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/enrichmentLinkage")

### enrichmentLinkage Type

`object` ([Details](dataset-definitions-enrichmentlinkage.md))

## Definitions group observations

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/observations"}
```




`observations`

-   is optional
-   Type: `object` ([Details](dataset-definitions-observations.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-observations.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observations")

### observations Type

`object` ([Details](dataset-definitions-observations.md))

## Definitions group observation

Reference this group by using

```json
{"$ref":"http://healthdatagateway.org/schema/dataset.json#/definitions/observation"}
```




`observation`

-   is optional
-   Type: `object` ([Details](dataset-definitions-observation.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-observation.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/observation")

### observation Type

`object` ([Details](dataset-definitions-observation.md))
