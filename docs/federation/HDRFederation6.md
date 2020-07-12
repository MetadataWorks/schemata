
6       Metamodel Specification
===============================

This section is informative at present, much depends on answers given in the
previous sections.

A metamodel is required for management of the technical metadata. Meta-models in
the database world are called  *schemas* and if all the datasets were based on
SQL data structures then it would be possible to call this section the
*schema*.  However, in order to differentiate relational-database-schemas, XML
Schemas, UML models and other structures we are using the term *Metamodel* to
denote the structure of a dataset.

Currently 2 metamodels are being used in the registries used by HDR, one for the
onboarding (Metadataworks or MDW), and one as the core metadata registry
(Oxford). These models are very close and are derived from the ISO11179
metamodel during research carried out for the most part at Oxford University.
Both models are designed to capture the structure of the data efficiently and
provide a means of managing the publication and versioning of datasets, however
they are totally focused on technical metadata. Both models can handle
extensible metadata, meaning that whatever summary, business and operational
metadata is chosen it can be managed. However, because of the way it is stored,
as unstructured key-value pairs, it is not necessarily the most efficient way of
handling the summary, business and operational metadata.

It is conceivable that we can extend the metamodel to allow for any kind of
structured metadata, but using the technical metamodel to manage the summary,
business and operational metadata.  The drawback of this is that the metadata
registry would need to be re-engineered, perhaps using RDF or RDFa as the core
technical binding instead of XML/UML as it currently is. The advantage would be
a much more flexible structure metadata registry in the long term.

6.1      The Current ISO11179 Metamodel
---------------------------------------

![](file:///?????clip_image009.jpg)

Figure 1 - Consolidated metamodel from ISO11179-3

6.2      ISO11179 Artefact Details
----------------------------------

The standard defines a number of terms which used to build up the description of
the core metamodel in Part 3, and these will be examined in the light of how one
can build a model using the standard from an existing database. By taking some
of the key terms and redefining them using a formal and a semi-formal system we
can arrive at a set of definitions which can define a metamodel sufficient to
capture context from any existing database or data-store.

The central artefact in the model is that of *Data Element*, defined in the
standard as shown in Table 1. The definition states that it is the result of
assigning a Data Element Concept to a Value Domain, and thus it is arguably a
relation between a Data Element Concept and a Value Domain.

*Data Type* - A Datatype is designated by a data type name and described by a
datatype description. The datatype name is usually drawn from some external
source, which is designated by a datatype scheme reference. Additional
information may optionally be provided using the datatype annotation

*Value Domain* - An example of a Conceptual Domain and a set of Value Domains is
ISO 3166, Codes for the representation of names of countries. For instance, ISO
3166 describes the set of seven Value Do- mains: short name in English, official
name in English, short name in French, official name in French, alpha-2 code,
alpha-3 code, and numeric code.

The idea of a Value Domain is not in widespread usage in data management or
computer science texts, in fact it doesn’t appear in a Wikipedia search other
than in the context of ISO11179. Thus, standard representations of ISO 3166 in
database tables do not include any reference to Value Domains, and it would
therefore entirely feasible to represent the context in which an aspect of
ISO3166 is used, say 2-character country codes, without any need to identify the
Value Domain concerned.

Data Types are associated with Value Domains, and a definition is provided in
Table 2, however it may be relevant at this stage to look at the general usage
of the term as well some other definitions. Parnas (Parnas et al., 1976)
identified 5 different ways in which the word *Data Type* is defined:

·      Syntactic.

·      Value Space. A type is defined by a set of possible values. 

·      Behaviour.   A type is defined by a value space and a set of operations
on elements of that space

·      Representation and Behaviour. A type is defined as its representation and
a set of operators manipulating that representation

·      Value Space and Behaviour. A type is a set of values which a variable can
possess, and a set of functions applied to those values.

Data Types are used in programming languages for the most part to detect errors,
by having a statically and strongly typed language errors can be detected by the
compiler before the program is run. Cardelli and Wegner (Cardelli and Wegner,
1985) provide the following explanation:

A type system has as its major purpose to avoid embarrassing questions about
representations, and to forbid situations where these questions might come up. 
In mathematics as in programming, types impose constraints which help to enforce
correctness. Some untyped universes, like naive set theory, were found to be
logically inconsistent, and typed versions were proposed to eliminate
inconsistencies. Typed versions of set theory, just like typed programming
languages, impose constraints on object interaction which prevent objects (in
this case sets) from inconsistent interaction with other objects. A type may be
viewed as a set of clothes (or a suit of armour) that protects an underlying
untyped representation from arbitrary or unintended use. It provides a
protective covering that hides the underlying representation and constrains the
way objects may interact with other objects. In an untyped system untyped
objects are naked in that the underlying representation is exposed for all to
see. Violating the type system involves removing the protective set of clothing
and operating directly on the naked representation.

Generally both programming languages and databases will have fixed datatypes,
and there is a widespread degree of overlap between the data types used by the
many languages and databases in service, Appendix 3 details the many data types
in common use in C, C++, Java, Python, MySQL, SQL Server and MS Access. From
this we can build up a set of artefacts which can model all these datatypes from
within a metadata registry, and by defining a direct mapping we can build this
part of the metadata model automatically.

Table 1 - Metamodel Domain Constructs 1

**ISO 11179 Structural Artefacts**

**Definition**

Conceptual Domain

a set of valid Value Meanings expressed as a description or via a set of
enumerations

Object Class

a set of ideas, abstractions, or things in the real world that are identified
with explicit boundaries and meaning and whose properties and behaviour follow
the same rules

Property

a characteristic common to all members of an Object Class

Data Element Concept

A Data Element Concept is a concept that can be represented in the form of a
data element, described independently of any particular representation. A Data
Element Concept may have zero or one Object Class and zero or one Property. The
union of a Property and an Object Class provides significance beyond either that
of the Property or the Object Class. A Data Element Concept thus has a
Definition independent from the Definition of the Object Class or the Property.

Data Element

A Data Element is considered to be a basic unit of data of interest to an
organization. It is a unit of data for which the definition, identification,
representation, and permissible values are specified by means of a set of
attributes. A Data Element is formed when a Data Element Concept is assigned a
representation. One of the key components of a representation is the Value
Domain, i.e., restricted valid values.

DataType

A Value Domain is associated with a Datatype a set of distinct values,
characterized by properties of those values and by operations on those values,
for example the category used for the collection of letters, digits, and/or
symbols to depict values of a Data Element determined by the operations that may
be performed on the Data Element.

Value Domain

(3.3.140) a set of Permissible Values. One of the key components of a
representation is the Value Domain. A Value Domain is associated with a
Conceptual Domain. A Value Domain provides a representation for the Conceptual
Domain.

Described or Non-enumerated Value Domain

A Value Domain may be expressed via a description or specification, such as a
rule, a procedure, or a range (i.e., interval), rather than as an explicit set
of Permissible Values. Such a Value Domain is called a Non-enumerated Value
Domain. As a sub-type of Value Domain, a Non-enumerated Value Domain inherits
the attributes and relationships of the former.

Enumerated Value Domain

An Enumerated Value Domain is one where the Value Domain is expressed as an
explicit set of two or more Permissible Values. As a sub-type of Value Domain,
an Enumerated Value Domain inherits the attributes and relationships of the
former

Permissible Value

A Permissible Value is an expression of a Value Meaning within an Enumerated
Value Domain. It is one of a set of such values that comprises an Enumerated
Value Domain. Each Permissible Value is associated with a Value Meaning.

Enumerated Conceptual Domain

a Conceptual Domain that is specified by a list of all its Value Meanings

 

Table 2 - Metamodel Domain Constructs 2

**ISO 11179 Relational Artefacts**

**Definition**

Relation

A Relation is a class each instance of which models a relation (3.2.119), a
sense in which concepts (3.2.18) may be connected via constituent relation roles
(

Relationship

(metamodel) a connection among model elements

Generalization

relationship (3.1.15) between a more general class (the parent) and a more
specific class (the child) that is fully consistent with the general class and
that adds additional information. A generalization is a type of relationship
(3.1.15); (Adapted from ISO/IEC 19505-2:2012, 7.3.20.)

Classification

A metadata item is classified if it has one or more Classification (9.2.3.1)
association classes, each with a Concept (9.1.2.1) class in a Concept System
(9.1.2.2).

classification scheme

descriptive information for an arrangement or division of objects (3.2.87) into
groups based on criteria such as characteristics (3.2.14), which the objects
have in com- mon

classifiable item

metadata item (3.2.75) of a type for which classification is supported in a
given metadata registry (3.2.78)

Concept System

Concept Systems may be used as classification schemes to classify Classifiable
Items within a registry, but some classification schemes will be more applicable
to classifying objects in the real world than items in a registry. If the
objects to be classified are not in the registry, the classification scheme may
still be recorded using the Concept System structures. A classification scheme
may be a taxonomy, a network, an ontology, or any other terminological system.
The classification may also be just a list of controlled vocabulary of property
words (or terms). The list might be taken from the ”leaf level” of a taxonomy.
Examples include SKOS, UML, OWL.

Concept

(3.2.18 )unit of knowledge created by a unique combination of characteristics

Unit of measure

value domain actual units in which the associated values are measured

Dimensionality

set of equivalent units of measure

6.3      Revised Metamodel Overview
-----------------------------------

tbd

6.4      FMDR Metamodel
-----------------------

The goal of the FMD registry is to build a metamodel of a dataset based on
access to a database table, series of tables or spreadsheet.

The language defines data elements, ways to group data elements, and ways to
handle relationships between different elements, within the same domain or
collection, and with data elements in other collections. It also is able to
define rules for typing and thus verifying data items, and also to define rules
or constraints, which in turn operate on groups of data elements. By defining
groups of data elements as data classes, a basic data structure, corresponding
to the structure used in almost all object-oriented computer languages and
databases storage mechanism can be built up.

Groups of classes are termed models, a model corresponding to a dataset, or as
in the case of health constraint information within one group, that information
then has the possibility to be transferred with the data during data transfer
operations, or due to the reference mechanisms in place to be referred to at a
later point in time.

![A screenshot of a cell phone Description automatically generated](file:////Users/davidmilward/Library/Group Containers/UBF8T346G9.Office/TemporaryItems/msohtmlclip/clip_image011.jpg)

Figure 2; FMDR Core Metamodel (subject to change)

The key artefacts of the new metamodel are:

Data Model

This artefact captures an overall group of data items which belong together, it
can be thought similar to a conceptual domain which groups a number of concepts
around a set of core idea. A terminology or dataset could be grouped as a Data
Model, and then versioning and publication is for simplicity grouped together.
For instance, one may wish to collect all the data elements pertaining to a
particular type of disease or illness, and curate them as a single Data Model.
One also may wish to import all the Data Elements from a particular system which
handles a particular disease or clinical grouping such as “haematology”, or
“lung cancer”

Data Class

This is a way of grouping or classifying collections of different data elements,
some of the containment relationships are borrowed from Object modelling
languages to handle hierarchical inheritance. However, inheritance here can be
configured for multiple or single inheritance as a policy. This can then be
adjusted using the import mechanisms to handle table linking as appropriate.

Data Element

This is the core element, and in many ways is similar to the current Data
Element, essentially this is an atomic data unit, which is related to a single
concept or idea, captured either by way of a link or in the name and description
of the Data Element.

Data Type

Every Data Element will have a single Data Type – which may be descriptive,
primitive (value based as given by the data source) or reference.

Relationship

These can be configured as appropriate and allow different Data Elements to be
linked together.

ExtensionItem (MetadataItem)

The Metadata Item can be added to any other Registered Element as appropriate
and will consist of a key-value pair.

RegisteredItem  (CatalogueElement)

The basis of all other registry element (i.e. Data Models, Data Classes, Data
Elements, ExtensionItems and Data Types are all RegistryItems, with a unique IRI
and a version.

 

6.5      FMDR Grammar
---------------------

To be defined

6.6       Metamodel Comparison
------------------------------

The following comparison is made by comparing the core Metadata Works codebase
with the model described on the Oxford Metadata Catalogue Wiki site, however it
must be pointed out that without sight of the source code it is possible that
the Oxford Data Catalogue has not been fully documented here.

Any amendments from the Oxford team would be most welcome.

Table 3: Metamodel Comparison

Notes

MDW

Oxford

ISO11179

Some properties differ

DataModel(Physical & Logical)

DataModel

\-

 

DataClass

DataClass

Object Class

 

Term

Term

Concept

 

DataElement

DataElement (Attribute?)

Data Element

 

DataType

DataType

Data Type

 

EnumeratedType

EnumerationValue

Enumerated Value Domain

 

PrimitiveType

\-

\-

 

ReferenceType

\-

\-

 

Relationship

\-

Relation

 

RelationshipType

\-

\-

 

RelationshipMetadata

\-

\-

 

ExtensionValue(MetadataItem)

Metadata

\-

 

Tag

Classifier

Classification

 

ValidationRule

\-

 

 

Asset

Attachment

 

 

AssetFile

 

 

 

\-

Comment

 

 

DataModel(Conceptual)

Terminology

 

 

Relationship (in Conceptual DataModel)

Term Relationship

 

 

Measurement Unit

 

Measurement Unit

 

 