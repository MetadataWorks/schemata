# Untitled object in HDR UK Dataset Schema

```txt
http://healthdatagateway.org/schema/dataset.json#/definitions/accessibility/properties/access/allOf/0
```




| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | ---------- | -------------- | ------------ | :---------------- | --------------------- | ------------------- | -------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Allowed               | none                | [dataset.schema.json\*](../out/dataset.schema.json "open original schema") |

## 0 Type

`object` ([Details](dataset-definitions-access.md))

# undefined Properties

| Property                                  | Type      | Required | Nullable       | Defined by                                                                                                                                                                                             |
| :---------------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [access-rights](#access-rights)           | `array`   | Required | cannot be null | [HDR UK Dataset](dataset-definitions-access-properties-access-rights.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/access-rights")                          |
| [access-service](#access-service)         | Merged    | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-access-properties-access-service.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/access-service")                        |
| [delivery-lead-time](#delivery-lead-time) | Merged    | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-access-properties-access-request-duration.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/delivery-lead-time")           |
| [access-requests](#access-requests)       | `integer` | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-access-properties-number-of-access-requests-received-1.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/access-requests") |
| [jurisdiction](#jurisdiction)             | `array`   | Required | cannot be null | [HDR UK Dataset](dataset-definitions-access-properties-number-of-access-requests-received.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/jurisdiction")      |
| [data-controller](#data-controller)       | Merged    | Required | cannot be null | [HDR UK Dataset](dataset-definitions-access-properties-data-controller.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/data-controller")                      |
| [data-processor](#data-processor)         | Merged    | Optional | cannot be null | [HDR UK Dataset](dataset-definitions-access-properties-data-processor.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/data-processor")                        |

## access-rights




> dct:access_rights 
>

`access-rights`

-   is required
-   Type: `url[]`
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-access-properties-access-rights.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/access-rights")

### access-rights Type

`url[]`

### access-rights Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

## access-service

Please provide a brief description of the environment where data can be accessed by researchers. If no environment is currently available, please indicate the current plans and timelines when the data will be made available through an access environment or process. Note: This value will be used as default access environment for all datasets submitted by the organisation. However, there will be the opportunity to overwrite his value for each dataset.


> dcat:accessService 
>

`access-service`

-   is optional
-   Type: merged type ([Access Service](dataset-definitions-access-properties-access-service.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-access-properties-access-service.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/access-service")

### access-service Type

merged type ([Access Service](dataset-definitions-access-properties-access-service.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-longdescription.md "check type definition")

### access-service Examples

```json
"https://cnfl.extge.co.uk/display/GERE/Research+Environment+User+Guide"
```

## delivery-lead-time

Please provide an indication of the typical processing times based on the types of requests typically received.


> <https://schema.org/deliveryLeadTime>
>

`delivery-lead-time`

-   is optional
-   Type: merged type ([Access Request Duration](dataset-definitions-access-properties-access-request-duration.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-access-properties-access-request-duration.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/delivery-lead-time")

### delivery-lead-time Type

merged type ([Access Request Duration](dataset-definitions-access-properties-access-request-duration.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-accessrequestduration.md "check type definition")

## access-requests

Please indicate the number of data access requests that have been received for the dataset. Note: please do not include data access requests received through the innovation gateway


> No standard identified
>

`access-requests`

-   is optional
-   Type: `integer` ([Number of Access Requests Received](dataset-definitions-access-properties-number-of-access-requests-received-1.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-access-properties-number-of-access-requests-received-1.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/access-requests")

### access-requests Type

`integer` ([Number of Access Requests Received](dataset-definitions-access-properties-number-of-access-requests-received-1.md))

## jurisdiction




> <http://purl.org/dc/terms/Jurisdiction>
>

`jurisdiction`

-   is required
-   Type: an array of merged types ([Details](dataset-definitions-access-properties-number-of-access-requests-received-items.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-access-properties-number-of-access-requests-received.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/jurisdiction")

### jurisdiction Type

an array of merged types ([Details](dataset-definitions-access-properties-number-of-access-requests-received-items.md))

### jurisdiction Constraints

**minimum number of items**: the minimum number of items for this array is: `1`

### jurisdiction Default Value

The default value is:

```json
"GB-ENG"
```

## data-controller

Data Controller means a person/entity who (either alone or jointly or in common with other persons/entities) determines the purposes for which and the way any Data Subject data, specifically personal data or are to be processed. Notes: For most organisations this will be the same as the publisher of the dataset. If this is not the case, please indicate that there is a different controller. If there is a different controller please complete the Data Processor attribute to indicate that the publisher is a Processor rather than the data controller.


>  dpv:DataController
>

`data-controller`

-   is required
-   Type: merged type ([Data Controller](dataset-definitions-access-properties-data-controller.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-access-properties-data-controller.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/data-controller")

### data-controller Type

merged type ([Data Controller](dataset-definitions-access-properties-data-controller.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-longdescription.md "check type definition")

## data-processor

A Data Processor, in relation to any Data Subject data, specifically personal data, means any person/entity (other than an employee of the data controller) who processes the data on behalf of the data controller. Notes: Required to complete if the Publisher is the Data Processor rather than the data controller.


> dpv:DataProcessor
>

`data-processor`

-   is optional
-   Type: merged type ([Data Processor](dataset-definitions-access-properties-data-processor.md))
-   cannot be null
-   defined in: [HDR UK Dataset](dataset-definitions-access-properties-data-processor.md "http&#x3A;//healthdatagateway.org/schema/dataset.json#/definitions/access/properties/data-processor")

### data-processor Type

merged type ([Data Processor](dataset-definitions-access-properties-data-processor.md))

all of

-   [Untitled string in HDR UK Dataset](dataset-definitions-longdescription.md "check type definition")
