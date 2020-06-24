7       Minimum Viable Product (MVP) : Implementation 
======================================================

**Recommendation: We develop a simple example of a federated system using
current available metadata registries, and from there look at a more
implementation-independent specification.**

Much of the work here depends decisions made in the previous sections, so please
treat this is a starting point for discussion.

Both the MDW and Oxford MDR’s are built using XML transfer mechanism, so for any
test instance we will probably need to remain in the XML technical space. Both
metadata registries have basic API’s that can be used to test out the Federation
principles.

Essential features of any implementation are firstly to have a single URL for
each data-model(dataset), and ideally to include in that URL the status and
version of the data-model. Attached to this can be the key metadata payload,
which could then be used to de-reference the “full” data-model from its (home)
metadata registry.  The principle of making all data-models, and ideally all
data-elements, de-referenceable using a carefully constructed URL (or IRI) is
key to the operation of a federated registry system.

7.1       Core Messaging
------------------------

The requirements identified in section 5.2 are repeated here and form the basis
of any core messaging required.

1.     Search to see what datasets are available for research

2.     Search to obtain details and access to datasets of interest

3.     Search to see alignment of data elements used in different datasets.

4.     Build new datasets re-using good common definitions.

5.     Build fused datasets where datasets are compatible and linkable.

6.     Relate datasets to core dataset specifications (e.g. SNOMED CT) and to
standard references datasets (e.g. NHS Data Dictionary).

For the minimum viable product exercise we consider only the first two
requirements, which we believe can be implemented relatively quickly using
existing registries.

### 7.1.1      Search

“*A user would like to find out what datasets are available across the
federation*”

There are a number of mechanisms to implement this, a master-slave relationship
is one, and a peer-to-peer discovery mechanism similar to the bonjour service is
another. The search could be carried out using a central index which all
registries have access to and use on shared basis.

Each registry needs to be able to give a list of all the datasets (or data
models) which are available. This can be accomplished an API which lists
available data models, the list should include a de-referenceable URI for each
data-model(dataset) in a registry, together with some core fields, ideally name,
description, see table below:

 

Metadata Item

Example

URI

https://\<Organisation registry URI\>/\<data model registry id\>/\<version
no\>/\<status\>

(Dataset) Name

100k Cancer Clinical Data

Description (keywords)

Cancer Clinical data from 100,000 patient records

Organisation

Genomics England

Contact Point

Joe Bloggs

Access Rights

URL of webpage showing access rights

 

 

 

MVP:  Basic federation can be implemented if each MDR has a REST interface
allowing the following calls:

 

### 7.1.2      API Details

The following is a skeleton set of methods for implementing a federated metadata
registry system, based on the metamodel and principles outlined earlier.
Currently an MVP based on this simple model can be implemented using the MDWs
metadata registry, and we believe it could also be implemented using the Oxford
metadata registry. Oxford to confirm.

 

REST

Example End-point

Notes

Get

https://derriford.hdrfederation.org/api/getAllDataModels

This will in effect be unsecured, and all registries will have this capability –
it will return the organization, a contact point, access details, and a list of
data models with URL (and embedded version/status) – each data-model will have a
contact point, a group or set of groups, abstract and publisher – (MVP: this
will be XML format conforming to the MDW Schema shown further on in this
section)

Get

https://derriford.hdrfederation.org/api/dataModel/\$Id

This will allow a client who has the URL of a specific data-model, obtained from
the previous call getAllDataModels.

The amount of details returned will depend on the user’s authorization level,
but it could be all the business, operational and technical metadata, returned
as XML (see MDW XSD examples)

Post

https://derriford.hdrfederation.org/users/requestAccess

Depending on the security model adopted this could be a request for
authorization for a particular data-model. The request could arguably also be
carried out by email.

 

7.2       Technical Spaces
--------------------------

### 7.2.1      Languages

#### 7.2.1.1      DSL

#### 7.2.1.2      XML

##### 7.2.1.2.1     Oxford XSD

 

 

![A screenshot of a social media post Description automatically generated](file:////Users/davidmilward/Library/Group Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image013.jpg)

 

 For full XSD details please see Appendix 3.

 

 

 

##### 7.2.1.2.2     MDW XSD

 

![A screenshot of a cell phone Description automatically generated](file:////Users/davidmilward/Library/Group Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image015.jpg)

![A screenshot of a cell phone Description automatically generated](file:////Users/davidmilward/Library/Group Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image017.jpg)

 

 

For full XSD details please see Appendix 4.

 

 

#### 7.2.1.3      RDF/OWL

 

 



 