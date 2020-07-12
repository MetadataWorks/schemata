 


1       Scope
=============

Initially this metadata specification is intended to be used to enhance search
capability on datasets held by Health Data Research UK (HDRUK) members and Hubs.
It is intended that the specification be developed and extended, in time, to
serve UK National Health Service and Healthcare organisations globally.

Much of the work has been built on attempts to build a technical metadata
meta-model in order to automate much of the mapping, curation and relationship
work which is carried out manually on datasets, in order to integrate data in a
machine-friendly fashion.  The work builds on work expressed in ISO11179, which
is a 6-part standard specifying how to design and build a metadata registry.

Enabling automated data-matching by using metadata will not achieve semantic
interoperability on its own, however it will help to achieve data integration in
less time, and with less expert effort that is now commonplace. It can thus be
viewed as step towards the goal of semantic interoperability. The work carried
out to develop this metamodel is covered papers referenced in (8) and (9).

The purposes of the ISO 11179 standard are to promote the following:

¾    Standard description of data

¾    Common understanding of data across organizational elements and between
organizations

¾    Re-use and standardization of data over time, space, and applications

¾    Harmonization and standardization of data within an organization and across
organizations

¾    Management of the components of data

¾    Re-use of the components of data

2.1       Key Decisions
-----------------------

This document is intended to be an initial discussion document. The principles
of the specification need to be defined in general terms, before we can move to
implementation details and specification of technologies. Currently once we have
agreed basic principles, in particular those related to versioning we can then
move to security principles and an MVP implementation.

 

*Key theoretical stages:

To build a federation we need to agree on identifiers and versioning as the core
of the registry system.

1.     Unique Identifiers

We need to agree how to uniquely identify datasets within the registry.  This is
linked to the idea of versioning and publishing, and currently a system based on
the ideas within ISO11179 is suggested as a way forward. This means that every
item in the catalogue will be given a unique identifier.  All items will be
grouped into Data Models (effectively a template for a dataset), and this will
be given a unique identifier based around the current internet domain name
system – an IRI. The suggested form is:

**\<domain name\>\<data model unique identifier – version\>**

For example we may have a reference dataset called “Pathology Codes” this can be
given the IRI:

<https://www.hdruk.ac.uk/>198992/

Data elements within a data model can also use this IRI format, so that another
element within the Data Model will be accessed using an extension of this
scheme, so for a data element “Aldosterone” within a reference Data Model we may
use the IRI as follows:

<https://www.hdruk.ac.uk/188998/dataElement/189056>

or even:

“<https://www.hdruk.ac.uk/188998/189056>”

 

Having an IRI means that registries in the federation can look up the “Cancer”
dataset in registry A without confusing it with the “Cancer” dataset in registry
B.


*As a user of registry A, I will be able to look up all datasets registered in
the whole federation using an IRI, and can be confident that
“https://RegistryA/CancerDataset“ is not going to be confused with
“https://RegistryB.com/CancerDataset”.*

*As a user if I want to use a data standard, which is simply identified by a
name, and whose version keeps changing, then I need to keep a copy of that whole
data standard locally, and have the ability to update my local copy, so that I
am not out of sync with this data standard.  Otherwise the dataset I build
referencing the standard today may be out of step tomorrow as the standard has
been updated.*

*As a user I may need to import a copy of Data Model (or standard) into my
registry, in order to build a new (conformant) data model, I need to keep the
trace of where the Data Model originated in order to maintain the provenance of
my dataset.*

*As a researcher in organisation A, with registry A as my local registry. I want
to build a set of forms to capture data based on a standard published by
registry B (because they have done some up to date work on say influenza vaccine
side effects) and I have located a Data Model (X version 1.0.0) in registry B,
which has all the specifications I need for my research forms. I will import
that into my registry, so that the Data Model(*<https://registryB/X-1.0.0>*)
will now be given a new local identifier of* <https://registryA/X-1.0.0/I-01>
*where the last part of the identifier identifies it as an imported model, with
an arbitrary letter ‘l’ for local and a unique number of the import – this
enables details of the import, including the original IRI, to be kept.  This can
be thought of as akin to a library storing their copy of the “Encyclopaedia
Brittanica” with a local index which will help the librarian find the book when
it is asked for.*

Having an IRI means that a resource is unique everywhere, and if I need to
impose security constraints on that particular dataset or Data Model I can do so
easily, by relating that IRI to a user or group identifier.

*As a data owner I want to ensure that the consent details surrounding a
particular dataset are adhered to.  I want to control who can see the details
relating to which datasets I am willing to share, and what are the conditions
that I intend to impose on these datasets.  I may want to store datasets that
are private to my organisation, but I may want to share some of these datasets
with other organizations.*

 

 