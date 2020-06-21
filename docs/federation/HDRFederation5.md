

5      Proposal Background
===========================

5.1      Background
-------------------

Health Data Research UK (HDR UK) has launched the Minimum Viable Product (MVP)
solution for the Innovation Gateway that allows for a rich set of level
information that describes the datasets that are available for research and
innovation across members of the UK Health Data Research Alliance and the seven
health data research hubs. This information is stored in the form of Metadata in
a central repository, which can be used directly by these organisations.
Additionally, there is also an easy to use Metadata Onboarding Portal for
non-technical users to provide their metadata, which is stored in the Onboarding
Metadata Repository.

This arrangement as well as plans by more technically advanced hubs and alliance
members to create and operate their own metadata repositories means that HDR UK
has identified a need for a federated mechanism for maintaining, storing and
accessing metadata. This mechanism must be fully automated beyond the initial
setup of the gateway membership to allow the Gateway and members of the
federation to index the information to return any search results from any of the
members without having to explicitly find the member that the information
originates from.

HDR UK’s initial requirements have been used as a baseline specification and
iterated based on feedback and suggestions from NHS Digital and Oxford
University (providing the Metadata catalogue) HDR UK, its alliance members and
the hubs.

The following principles have governed the work and decisions made:

·      Specification that will be distributed in first iteration will be “good
enough MVP” rather than perfect

·      Metadata Federation should use open standards whenever possible and only
if no standard can be found should we create a new mechanism.

The specification is split into the following sections:

·      Summary Metadata, giving overview and search terms for indexing purposes.

·      Descriptive Metadata i.e. metadata required to manage data catalogues and
is descriptive in content.

·      Technical Metadata, i.e. a formal (or mathematical) metamodel of data
structure and other technical aspects of the data.

·      Operational Metadata, including quality, profile, volume, lineage and
other aspects of the data relating to processing of underlying data to the
resulting data present in the dataset.

·      A peer-to-peer Metadata Federation that covers

o   Data catalogues that can be published and linked to specifications for its
data elements

o   Universally Unique identifiers for every item in all data catalogues in the
federation (and beyond???)

o   Structured metadata for items in the catalogue

o   Linking data terms to each other within the original catalogue as well as
others elsewhere in the federation network

o   Data Dictionary that defines enterprise data (not “Standards”) in which a
name, definition, datatype and enumeration if present, need to be made available
in machine readable and human readable format for Data sharing, semi-automated
customization of data collection tools and other uses

o   Machine readable format for metadata specifications to support data mapping
and transformation

o   Replicated data set address indexes across the federation network

o   Persistent Access control across the federation network

o   Federation API endpoints and descriptions


5       Requirements
====================

5.1       Primary Requirements
------------------------------

We expect that the key requirement for a researcher will be to find out all
possible information about a subject X.  How this information is stored and what
is needed to do to be able to access that data is the job that a metadata
federation should do. From this basis we look at how this can be split into
detailed requirements, some of which we express as user stories.

### 5.1.1      As a researcher I want to understand all the data available on subject of interest.

Data is held in datasets. Datasets can be excel files, csv files, RDF files, XML
Files, RDMS or even text files. So all of the data in these heterogeneous
formats need to be converted to the same format in order to work with it, so the
way in which the data is stored needs to be recorded.

 

Data in one dataset can be linked to data in another dataset. For example, very
often datasets are built to conform with a version of a reference data standard
such as SNOMED CT, FHIR or LOINC for example. This means that if a data element
in dataset A is described using SNOMED CT code XY, it can be linked to every
other data element which is described using the same code XY.  This kind of
linking will allow a researcher to expand the datasets that are of interest, or
even the set of data elements of interest, despite the fact that they reside in
many different data repositories.

 

Linking on an open data can enable vast amounts of data stored in multiple
repositories to be linked, enabling the researcher to navigate the data directly
and build up a knowledge graph of all the data they need.  This works when all
the data is either stored in RDF/OWL, or served up as JSON-LD or RDF,  and where
minimal security is attached to the data.  Whilst many of the ideas behind
linked open data can be used in building a federated metadata registry system,
the fact that not all local repositories and registries are able, or willing, to
publish data in an open-data format must be accounted for. The federated system
needs to function for heterogeneous datasets, i.e. those stored as excel, csv,
in XML files, in various relational and NOSQL databases, RDF, graph databases,
where the formatting and structuring is specified in multiple different ways.

 

 

### 5.1.2      As a researcher I want to know where relevant data resides so that I can find out how to access it.

This comes from the previous requirement and states that as a researcher my goal
is to access as many datasets that have data related to my subject X as
possible.  If I run a search on one part of the network, I want to be able to
find all the datasets that reside in both my local organization or network
section but also which reside in other network sections or organisations located
elsewhere.

 

### 5.1.3      As a researcher once I understand where a dataset is located, I want to satisfy all the requirements to download it and use it in my research.

Once I have enough metadata to determine that a dataset is of interest to me, I
need to find out who to contact to obtain that dataset (or subset thereof). I
need to know what the constraints on that dataset are, whether I can take a copy
of the data to keep locally, or if I can get updates of the dataset should it be
updated. I need to know how good the data is, and how the data is structured. 

 

### 5.1.4      As a researcher I want to be able to map my analysis dataset to the source datasets that are available.

This is a key requirement, the data may reside in many different datasets
described by different schema types, and so some kind of estimation of how to
source the data needs to be carried out. Data may already be passed from one
system to another using ETL techniques, and some of this data may already have
been assessed and moved using transformations.

 

As an example, suppose I need the following very simple table of data:

 

 

 

And I suspect I may need data from Cancer Registry A, and Cancer Registry B, the
schemas are given for Cancer Registry A in an XSD document, and for Cancer
Registry B in a relational database schema. These are shown in Figure A and B
below.

 

**Figure A: Cancer Registry Model A**

![A screenshot of a social media post Description automatically generated](file:////Users/davidmilward/Library/Group Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image005.jpg)

 

 

**Figure B: Cancer Registry Model B**

![A screenshot of a social media post Description automatically generated](file:////Users/davidmilward/Library/Group Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image007.jpg)

 

There are problems here with naming, structure and versioning which conspire to
make it difficult to just take a file of data conforming to Cancer Model A and
add it to data conforming to Cancer Model B.

 

 

 

 

5.2       Secondary Requirements
--------------------------------

The key requirements are to be able to search a group of federated metadata
registries as if they were a single store of datasets. The first issue is how to
identify different datasets.

### 5.2.1      Naming and Versioning

Globally unique identifiers will enable different datasets and even component
data elements to be identified. A system which allows an organisation’s name, or
the name of a particular metadata registry to be included in the naming system
will help location.

 

As a researcher I may obtain access to several datasets, A, B, and C for a
particular research subject, these may be located in different places, so if we
assume that each organisation has it’s own name as part of the naming system, we
can uniquely identify each dataset with the following unique identity:

 

**\<Organisation\>\<DatasetID\>**

 

This assumes that each organisation has a unique name or identifier such as a
domain name as given by the global internet domain name system. If that is the
case then assuming all the datasets for an organisation are registered in one
metadata registry, with all the appropriate metadata, then as a researcher I
will be able to guarantee that my datasets A, B and C can always be correctly
identified.

 

In addition if my metadata registry is able to uniquely identify data elements
and other artefacts, I will be able to append an artefact identifier, to build
up a hierarchical naming system for all the technical metadata as follows:

 

**https://\<Organisation-domain-name\>/\<DatasetID\>/\<DataArtefactID\>.**

 

 

 

### 5.2.2      Versioning

The NHS data dictionary has a website and a download area for its key datasets,
and people can use the website to look up data formats, and ensure that the
codes they are using for a clinical trial record align, for reporting purposes,
with the current datasets on the website.  However, there have been at least 15
updates to the NHS Data dictionary.

 

#### 5.2.2.1      **As a researcher if I record that I am using a data element from the NHS data dictionary today, and reference that same URL and named element in 12 months there is a chance that it will have changed.** If this happens then the data I am collecting will no longer align with the reporting system, and I may have to manually convert the data.

 

To avoid this problem the version needs to be part of the name, and we need to
ensure that the contents of the dataset once given a version doesn’t change.

 

### 5.2.3      Linking

As a researcher I may need to link to another dataset, or dataset specification
without downloading the whole content of the specification. As with the previous
example, I may build my own dataset, but I want some key elements in common with
common dataset specifications such as SNOMED CT or LOINC.

 

A mechanism to link a data element, a group of data elements or even a whole
dataset to the newly curated dataset will allow that information to be brought
into the new dataset. We may define different types of linking relationships, so
that in some case data elements I use locally can be forced to align with a
particular dataset standard.

 

This indicates that we need the means to define the link itself, and possibly
add some information about how the link will be used, in other words define a
relationship with the other dataset or group of elements.

 

### 5.2.4      Import Mechanism

As a researcher I may need to import all the data in a dataset into my own
research environment in order to work on it and make it available to co-workers
in my team. In this case it makes sense to be able to copy the original dataset,
together with the meta-dataset, and install it locally, whilst registering it
with the metadata registry. That way other people with access to my local
metadata registry can also see that it is available, and see under what
conditions I am making it available locally.

 

#### **5.2.4.1      As a researcher I want to import the source metadata into my local metadata registry**

This is important for the reasons identified in 4.1.4, but also it is useful to
have a record of where data is stored, and to have it locally without needing to
make global searches. It makes sense to be able to import the data directly to a
local metadata instance.

*For example if I am building a new dataset specification Y, and I am taking
some definitions X (from another organisation), I will also want to see where
these definitions originate: are they part of a reference dataset (SNOMED CT for
instance) which is residing in registry D? or did they originate somewhere else
– reference R for instance. I may want to import some other definitions X2 from
registry D instead, or go to registry R for the original definitions.*

 

#### **4.2.4.2      As a researcher I want to import the source data into my local data repository.**

As a researcher, having made a request for a dataset, ideally I would expect to
receive a copy of that dataset which I can then store locally in my working data
repository. It may be possible for the source data repository guardian to simply
provide the appropriate security credentials, which when received can be used to
access the data directly for a specific time period.

 

### 4.2.5      As a Data Publisher I want many experts from many organisations to contribute to my new data model, in order to get it widely endorsed and used.

As a data publisher I want to put a model together which covers my expertise,
but I also want other experts to contribute so that other areas that I am not so
strong in can be well defined. This means that if I put together a model of a
dataset, name, version and publish it then other people in other organisations
should be able to modify it.

For this to happen the original version needs to be fixed in structure, and each
separate modification needs to be versioned in a new “copy”, or “draft” version
of the dataset specification. Lets suppose there is a model A in registry Z, I
take a copy (A1) and modify it. I then send it back to registry Z as model A1.
Registry Z needs to be able to access model A and create a new model based on
the incoming model A1. Now someone else may have started working on a new
version of model A in registry Z, therefore I need a naming system which will be
able to:

1)    Relate the incoming draft model A1 to the original fixed model A.

2)    Differentiate the incoming model A1 from the other model A1 already in
registry Z.

 

 

 

 

 

 

5.3      
---------

 

In summary we can view the requirements as being:

1.     Search to see what datasets are available for research

2.     Search to obtain details and access to datasets of interest

3.     Search to see alignment of data elements used in different datasets.

4.     Build new datasets re-using good common definitions.

5.     Build fused datasets where datasets are compatible and linkable.

6.     Relate datasets to core dataset specifications (e.g. SNOMED CT) and to
standard references datasets (e.g. NHS Data Dictionary).

 

5       Basic Principles
========================

 

This section looks at how the requirements in the previous section can be
implemented in practise, and explores some of the issues in a bit more depth.

5.1       Unique Identifiers and Version Control
------------------------------------------------

 

 

5.2       Descriptive Metadata
------------------------------

 

 

5.3       Technical Metadata
----------------------------

 

 

5.4       Security (Concerns)
-----------------------------

It is anticipated that organizations will each have their own metadata registry,
and that the security will be managed on a peer-to-peer basis. In essence,
datasets are resources, and metadata about resources is also a resource which is
owned, and therefore needs to be managed.

To meet the requirements of federated access to these resources

·      Each metadata registry would manage its own users, and each registry
would trust users from all the other metadata registries.

·      A user in one registry would be able to read objects in a remote registry
but would be unable to update them, unless specifically permitted.

We suggest 2 authorisation mechanisms, the first is a more simplistic role-base
mechanism, the second is a fully fledged authorization system which can be as
fine-grained as the metadata registry owner wishes. This is augmented by the
ability to enable Federated Single Sign on across the registry network.

### 5.4.1      Authentication

Authentication can be done locally in a metadata registry, using simple username
and passwords.

Alternatively, a web-based scheme such as OpenID can be used, or indeed
Google/Microsoft/Facebook authentication application.

What kind of authentication is required?

### 5.4.2      Authorization

Authorization can be carried out using a web-based method, or using an
enterprise scheme, or it can be implemented locally on each metadata registry.
The main alternatives are Role-based access control, and Access Control List
authorization, the latter allowing a more fine-grained approach.

What kind of authorisation is required?

#### 5.4.2.1       Role-based access control security model

Under this model the federation will collectively define a set of roles, say
Administrator, Data-user, Data-reader, and assigned permissions to these roles
as follows:

**Role**

**Users**

**Local Objects**

**Remote Objects**

Administrator

Can add/update/delete local users

Can read/add/update/delete objects

No rights

Data-user

\-

Can read/add/update/delete objects

Can read objects

Data-reader

\-

Can read objects

Can read objects

The key concept here is that users would have very broad control allotted to
them, based on their assigned role for all objects stored in the metadata
registry. This would include all 4 different metadata categories. There would be
no capability to alter access based on the user and/or the object in question.

#### 5.4.2.2       Access Control List security model

This model gives the owner of each object in a metadata registry the ability to
control who can access each metadata object, this could be taken right down to
data elements in a dataset, however the more fine-grained the security the
greater the administrative burden for the data owner.

It is likely that some degree of role-based permissions would be needed for
implementing the basic search capability, so that a user in MDR A can make a
search and get results from MDR B,C and D.

However the amount of access that a user can obtain maybe constrained by their
rights to the datasets, and although they may be able to view the summary
metadata of all the data models being stored in the federation, they may have to
ask the data-owner for permission to get the business, technical and operational
metadata associated with that dataset.

#### 5.4.2.3      Federated Single Sign-On

The authorisation schemes above govern access to resources within a registry.

Let’s assume a Data-reader in MDR A makes a search for “cancer”, and a list of
datasets are returned from MDR A,B & C. For coarse grained security the list
will only list the URI of the dataset and on clicking that URL the user will be
taken to the web page associated with that catalogue item. However, they may not
have permission to access the dataset, in which case they will be re-directed to
make an (email) request to gain permissions to access the resources concerned.
For finer grained security at individual attribute or metadata item level, each
such resources would need to be addressable using URLs  in their own right and
accessing those would follow the same pattern.

This scenario assumes a federated authentication and authorization system, such
as SAML (<http://docs.oasis-open.org/security/saml/v2.0/>) or OpenID Connect
Federation (<https://openid.net/specs/openid-connect-federation-1_0.html> ) in
play. Each registry will be responsible for its users, and if a user wants to
gain full access to local resources, they will need to obtain a local account
with appropriate permission.

Both SAML and OpenID Connect Federation work based on assertions provided by the
owning authority of a resource including any required access rights or other
properties. OpenID Federation in particular builds on top of OpenID connect
authentication mechanism to enable a user authenticated y one member of the
federation to be reused dynamically to access resources of another member.

SAML is XML based and has advanced capabilities for federation, so it is
suitable for server to server communications, but browser based SAML exchanges
can become quite onerous because of large XML  request and response payloads.

OpenID Connect avoids some of these issues by using JSON as its payloads format
and provides a nice thin layer of authentication over OAuth 2 to satisfy the
core authentication and authorisation needs of modern-day web and API access.

The big identity providers like Google and Facebook etc., use this very
combination for authentication and authorisation.

The final piece of picture to fulfil the requirements of this specification is
provided by OpenID Connect Federation which provides mechanism for single sign
on across a federation as well as account linking i.e. ability to have multiple
local accounts in the federation and use them as appropriate in a single trust
chain or multiple overlapping ones

Google, Facebook etc. have some support for the Single Sign On aspects of OpenID
Connect Federation but the account linking is mostly proprietary still.

**Recommendation:  Use OpenID Connect for authentication OAuth2 for core
authorisation and OpenID Connect Federation, which are all open standards and
will allow for both coarse and  fine-grained access control.**

5.5       Current Metadata Requirements
---------------------------------------

The current version of the HDR metadata specification requires that an
organization provides the following metadata fields:

·      Name

·      Logo

·      About

·      Membership

·      Grid.ac identifier

·      Contact Point

·      Access Rights

·      Access Request Cost

·      Access Request Duration

·      Access Environment

·      Terms and Conditions

These would be automatically appended to all datasets being catalogued, and thus
would be searchable throughout the federation.

The specification lists the following items as summary metadata:

·      DOI

·      Title

·      Abstract

·      Publisher

·      Contact Point

·      Group

·      Local Identifier

The metadata items classed as ‘organisational’ and ‘summary’ are those which
will be visible by anyone who has access to the federated metadata registry
system. The search should go ahead using keywords, which are protected as
‘business’ metadata, however all these items above will be visible on a search
result.

