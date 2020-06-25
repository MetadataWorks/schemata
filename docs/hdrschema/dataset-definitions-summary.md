# Summary Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/descriptive-metadata/properties/summary
```

Summary metadata must be completed by Data Custodians onboarding metadata into the Innovation Gateway MVP.


| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## summary Type

`object` ([Summary](dataset-definitions-summary.md))

# Summary Properties

| Property                        | Type    | Required | Nullable       | Defined by                                                                                                                                                                            |
| :------------------------------ | ------- | -------- | -------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [title](#title)                 | Merged  | Required | cannot be null | [HDR UK Dataset](dataset-definitions-summary-properties-title.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/title")                       |
| [abstract](#abstract)           | Merged  | Required | cannot be null | [HDR UK Dataset](dataset-definitions-summary-properties-abstract.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/abstract")                 |
| [publisher](#publisher)         | Merged  | Required | cannot be null | [HDR UK Dataset](dataset-definitions-summary-properties-publisher.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/publisher")               |
| [contact-point](#contact-point) | Merged  | Required | cannot be null | [HDR UK Dataset](dataset-definitions-summary-properties-contact-point.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/contact-point")       |
| [keywords](#keywords)           | `array` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-summary-properties-keywords.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/keywords")                 |
| [doiname](#doiname)             | Merged  | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-summary-properties-digital-object-identifier.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/doiname") |
| [identifier](#identifier)       | `array` | Required | cannot be null | [HDR UK Dataset](dataset-definitions-summary-properties-identifier.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/identifier")             |

## title

Name of the dataset limited to 80 characters. It should provide a short description of the dataset and be unique across the gateway. If your title is not unique, please add a prefix with your organisation name or identifier to differentiate it from other datasets within the Gateway. Please avoid acronyms wherever possible. Good titles should summarise the content of the dataset and if relevant, the region the dataset covers. Notes: if the dataset is a “linked dataset”, please indicate this using the prefix “Linked”.


> dct:title
>

`title`

-   is required
-   Type: merged type ([Title](dataset-definitions-summary-properties-title.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-summary-properties-title.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/title")

### title Type

merged type ([Title](dataset-definitions-summary-properties-title.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-eightycharacters.md "check type definition")

### title Examples

```json
"North West London COVID-19 Patient Level Situation Report"
```

## abstract

Provide a clear and brief descriptive signpost for researchers who are searching for data that may be relevant to their research. The abstract should allow the reader to determine the scope of the data collection and accurately summarise its content. The optimal length is one paragraph (limited to 255 characters) and effective abstracts should avoid long sentences and abbreviations where possible. Note: Researchers will view Titles and Abstracts when searching for datasets and choosing whether to explore their content further. Abstracts must be different from the full description for a dataset.


> dct:abstract
>

`abstract`

-   is required
-   Type: merged type ([Abstract](dataset-definitions-summary-properties-abstract.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-summary-properties-abstract.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/abstract")

### abstract Type

merged type ([Abstract](dataset-definitions-summary-properties-abstract.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-abstract.md "check type definition")

### abstract Examples

```json
"CPRD Aurum contains primary care data contributed by General Practitioner (GP) practices using EMIS Web® including patient registration information and all care events that GPs have chosen to record as part of their usual medical practice."
```

## publisher

Completion Notes: This is the organisation responsible for running or supporting the data access request process, as well as publishing and maintaining the metadata. In most this will be the same as the HDR UK Organisation (Hub or Alliance Member). However, in some cases this will be different i.e. Tissue Directory are an HDR UK Gateway organisation but coordinate activities across a number of data publishers i.e. Cambridge Blood and Stem Cell Biobank.


> dct:publisher
>

`publisher`

-   is required
-   Type: merged type ([Publisher](dataset-definitions-summary-properties-publisher.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-summary-properties-publisher.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/publisher")

### publisher Type

merged type ([Publisher](dataset-definitions-summary-properties-publisher.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-eightycharacters.md "check type definition")

### publisher Default Value

The default value is:

```json
"Defaulted to the organisation registered the metadata in the catalogue"
```

### publisher Examples

```json
"Cambridge Blood and Stem Cell Biobank"
```

## contact-point

Please provide a valid email address that can be used to coordinate data access requests with the publisher. Organisations are expected to provide a dedicated email address associated with the data access request process. Notes: An employee’s email address can only be provided on a temporary basis and if one is provided an explicit consent must be obtained for this purpose.


> dcat:contactPoint
>

`contact-point`

-   is required
-   Type: merged type ([Contact Point](dataset-definitions-summary-properties-contact-point.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-summary-properties-contact-point.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/contact-point")

### contact-point Type

merged type ([Contact Point](dataset-definitions-summary-properties-contact-point.md))

all of

-   [Untitled email in HDR UK Dataset](dataset-definitions-email.md "check type definition")

### contact-point Examples

```json
"SAILDatabank@swansea.ac.uk"
```

## keywords

Please provide relevant and specific keywords that can improve the SEO of your dataset as a comma separated list. Notes: Onboarding portal will suggest keywords based on title, abstract and description. We are compiling a standardised list of keywords and synonyms across datasets to make filtering easier for users.


> dcat:keyword
>

`keywords`

-   is optional
-   Type: `array`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-summary-properties-keywords.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/keywords")

### keywords Type

`array`

### keywords Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

**unique items**: all items in this array must be unique. Duplicates are not allowed.

## doiname

Registered datasets should either have a Digital Object Identifier (DOI) or be working towards obtaining one. If a DOI is available, please provide the DOI. If a DOI has not been created for the dataset, please provide a default value: “In Progress” whilst you create your DOI. You can either use the HDR UK Onboarding Portal (HOP) to mint a DOI for your dataset or your chosen alternative means. Note: This is not the DOI of the publication(s) associated with the dataset.


> Vocabulary: DOI Data Dictionary 
>

`doiname`

-   is optional
-   Type: merged type ([Digital Object Identifier](dataset-definitions-summary-properties-digital-object-identifier.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-summary-properties-digital-object-identifier.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/doiname")

### doiname Type

merged type ([Digital Object Identifier](dataset-definitions-summary-properties-digital-object-identifier.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-doi.md "check type definition")

### doiname Examples

```json
"10.3399/bjgp17X692645"
```

## identifier




`identifier`

-   is required
-   Type: `string[]`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-summary-properties-identifier.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/summary/properties/identifier")

### identifier Type

`string[]`

### identifier Constraints

**minimum number of items**: the minimum number of items for this array is: `1`
