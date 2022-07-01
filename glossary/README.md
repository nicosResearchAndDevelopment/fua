# Glossary

Glossary and index for the "Framework Univer Architecture" (**FUA**).

## Introduction

`fua`s [glossary](./README.md) is used **NOT** only for **fua** itself, but also used for [`GAIAboX (GBX)`](#gaiabox)
and so for [`this repository`](../gbx/README.md) bringing **fua`s** ideas, concepts and mechanics to life.

## Summary

The [glossary](./README.md) acts as a gate to further [information](#information) and more detailed explanations.

---

## A

### Access Control

[Controlling](#control) access to targeted and underlying resources (assets).

#### see also

- [Access Control, Wikipedia](https://en.wikipedia.org/wiki/Access_control)

```#access-control, #control```

---

### Access Control List

"Access Control List" [(**ACL**)](./shortcut.md#acl).

#### see

- [ACL](#acl)

```#access-control-list, #acl, #access-control, #control```

---

### ACL

[(**ACL**, shortcut)](./shortcut.md#acl), "Access Control List".

#### see

- [`dacl` (Dynamic Access Control Language)](../extension/decide/profile/dacl/README.md)

#### see also

- [Web Access Control, latest version, solidproject](https://solidproject.org/TR/wac)

```#acl, #access-control-list, #access-control, #control, #solid```

---

### Action

An "Action" is **NOT** interruptible and **MAY** contain a [timestamp](#timestamp).

A given Action triggers [Activities](#activity).

#### see

- [`Activity`](#activity)
- [`Process`](#process)

```#action```

---

### Activity

An "Activity" has a beginning, a duration and an end.

An Activity **MAY** generate something (a product, a resource, an entity) using other resources (etc.)

An "Activity" is interruptible.

#### see

- [`Action`](#action)
- [`Process`](#process)

```#activity```

---

### Agent

A resource featured doing something.

```#agent```

---

### Alice

"Alice" embodies a [Service Instance](#service-instance) and sometimes a person (but always an [Agent](#agent)), also -
usually acting with [role](#role) ["Data Provider"](#data-provider) and as a [Controller](#controller), sending commands
directed to given [Agent](#agent). The recipient she likes most is [Bob](#bob).

#### see

- [`Bob` as a "Data Consumer"](#bob)

```#alice, #agent```

---

### Anthropocentric Information

#### see

- [`IA`](#ia)

---

### Application

```#application```

---

### Application Layer

The "Application Layer" is populated with given [application](#application).

[**OSI**](https://en.wikipedia.org/wiki/OSI_protocols) attributes it with numerical position "7",

#### see also

- [Open Systems Interconnection protocols (OSI), Layer 7, Application Layer, Wikipedia](https://en.wikipedia.org/wiki/OSI_protocols#Layer_7:_application_layer)
- [Open Systems Interconnection protocols (OSI), Wikipedia](https://en.wikipedia.org/wiki/OSI_protocols)

```#application-layer```

---

### Authentication Service

```#authentication-service, #ats```

---

### Authorization Service

```#authorization-service, #ats```

---

### Authority

An "Authority" ([**AU**](./shortcut.md#au)) is an [agent](#agent) generating
data (like [identifiers](#internal-identifier)) and information attached to given identifiable resource.

`fua` uses it by those (sub-classed) concepts:

- Certificate Authority, [DataVerse (**DAVE**)](../extension/dataverse/README.md#certificate-authority)
- Notarisation, [DataVerse (**DAVE**)](../extension/dataverse/README.md#notarisation)
- Certification Body, [DataVerse (**DAVE**)](../extension/dataverse/README.md#certification-body)

#### see

#### see also

- [authority, Wikidata](https://www.wikidata.org/wiki/Q174834)
- [Authority (disambiguation), Wikipedia](https://en.wikipedia.org/wiki/Authority_(disambiguation))

```#authority, #agent```

---

## B

### Base Twin

```#base-twin, #digital-twin, #physical-twin, #twin```

---

### Bob

"Bob" embodies a [Service Instance](#service-instance) and sometimes a person (but always an [Agent](#agent)),
usually acting with [role](#role) ["Data Consumer"](#data-consumer) and so populates the
[Problem Layer](#problem-layer) while consuming data, made available by given
[Service Instance](#service-instance) acting in [role](#role) ["Data Provider"](#data-provider).

Bob has to execute commands, being [controlled](#controller) by [Alice](#alice).

#### see

- [`Alice` as a "Data Provider"](#alice)

```#bob, #agent```

---

## C

### Certificate Authority

```#certificate-authority```

---

### Certification Body

```#certification-body```

---

### Clearing House

#### see

- [Clearing House (**DAVE**)](../extension/dataverse/README.md#clearing-house).

```#clearing-house```

---

### Constraint

A "Constraint" is to be understood as an _auxiliary condition_ to be evaluated in a given [rule](#rule).

Constraints are typically hosted in [rules](#rule).

#### see

- [`Rule`](#rule)

```#constraint```

---

### Command

A "Command" is an _instruction_, wrapped by a [control](#control) and send by a [controller](#controller)
targeted to receiving [agent](#agent).

```#command```

---

### Computing Data

#### see also

- [Data (computing), Wikipedia](https://en.wikipedia.org/wiki/Data_(computing))

```#computing-data```

---

### Consumer

"Consumer" is a [role](#role).

An [agent](#agent), consuming resources, act in its role [Consumer](#consumer).

#### see

- [`Data Consumer`](#data-consumer)

```#consumer```

---

### Control

A "Control" is a piece of [information](#information) send by a [controller](#controller) to targeted [agent](#agent).
The main content of given information are values and [commands](#command), those the receiving agent has to work with.  
The controlled agent is `controlledBy` by _the_ [Controller](#controller).

```#control```

---

### Controller

An [agent](#agent), acting as a "Controller", [controls](#control) a given resource ([agent](#agent)) by
sending commands. The controlled agent is `controlledBy` by _the_ Controller.

```#controller, #control```

---

### Control Language

A language to express [control](#control) over given asset.

`fua` is focused on a machine-readable control languages, aligned to ["Open Digital Rights Language (**ODRL**)](#odrl).

#### see

- [Decide](../extension/decide/README.md)

```#control-language, #control```

---

### Control, Access

#### see

- [`Access Control`](#access-control)

---

### Control, Remote

#### see

- [`Remote Control`](#remote-control)

---

### Control, Usage

#### see

- [`Usage Control`](#usage-control)

---

## D

### DACL

The "Dynamic Access Control Language" (**DACL**) as an **ODRL**-profile defined
by `fua`.

**DACL** enables ["Access Control"](#access-control).

#### see

- [Decide Profile DACL](../extension/decide/profile/dacl/README.md)
- [`ODRL ("Open Digital Rights Language")`](#odrl)

```#dacl, #access-control, #control-language, #control```

---

### Data

Value, achieved by observation or measurement and basis of [Information](#information).

#### see

- [`Information`](#information)

#### see also

- [Data, Wikidata](https://www.wikidata.org/wiki/Q42848)
- [Data (computing), Wikidata](https://en.wikipedia.org/wiki/Data_(computing))

```#data```

---

### Data Consumer

"Data Consumer" is a [role](#role).

Given [agent](#agent) requesting [data](#data) has membership to [role](#role) _Data Consumer_.

`fua` often uses "Data Consumer", _simplifying only_ and covering the fact, that it is an [agent](#agent) attributed
with [role](#role) [Data Consumer](#data-consumer).

In the end it is this: [Data Consumer](#data-consumer).

#### see

- [`Data Provider`](#data-provider)

```#data-consumer, #role, #data```

---

### Data Exchange

"Data Exchange" could be understood as generic [activity](#activity) of _exchanging data_:

A [Data consumer](#data-consumer) requests (and _this_ request contains data itself: [information](#information)
regarding requesters identification and/or authorization as [Infrastructure Data](#infrastructure-data) and
the _resource of interest_ as [Payload Data](#payload-data)) [data](#data) from a [Data Provider](#data-provider).

The [Data Provider](#data-provider) responses with the _resource of interest_ as [Payload Data](#payload-data),
decorated with some  [Meta Data](#meta-data), etc.

### see

- [Understanding "Data Exchange"](../understanding/dataexchange/README.md)

#### see also

- [`Data`](#data)
- [`Infrastructure Data`](#infrastructure-data)
- [`Payload Data`](#payload-data)
- [`Data Provider`](#data-provider)
- [`Data consumer`](#data-consumer)

```#data-exchange, #data-consumer, #data-provider```

---

### Data Exchange, Trusted

#### see

- [Trusted Data Exchange](#trusted-data-exchange)

---

### Data, Computing

#### see

- [`Computing Data`](#Computing-data)

---

### Data, Infrastructure

#### see

- [`Infrastructure Data`](#infrastructure-data)

```#infrastructure-data```

---

### Data, Meta

#### see

- [`Meta Data`](#meta-data)

---

### Data, Payload

#### see

- [`Payload Data`](#payload-data)

---

### Data Layer

The "Data Layer" is an overarching [Layer](#layer), so it can be stated

```#data-layer, #data```

---

### Data Linkage

#### see

- [`Linked Data](#linked-data)

---

### Data Domain

---

#### see

- [`DataDomain`, DataVerse](../extension/dataverse/README.md#data-domain)
- [`Data Verse`](#dataverse)

```#data-domain, #dataverse```

---

### Data Owner

```#data-owner```

---

### Data Provider

"Data Provider" is a [role](#role).

Given [agent](#agent) called by a request (send by a [Data Consumer](#data-consumer)), providing [data](#data) asked
for, has membership to [role](#role) _"Data Provider"_.

`fua` often uses "Data Provider", _simplifying only_ and covering the fact, that it is an [agent](#agent) attributed
with [role](#role) [Data Provider](#data-provider).

In the end it is this: [Data Provider](#data-provider).

#### see

- [`Data Consumer`](#data-consumer)
- [`Role`](#role)

```#data-provider, #role```

---

### Data Lineage

"Data Lineage" (**DL**).

> Data lineage includes the data origin, what happens to it and where it moves over time.

_taken from [Data lineage, Wikipedia](https://en.wikipedia.org/wiki/Data_lineage)_.

Another, often used _chatchphrase_ is "Data Provenance". But `fua` is focused on "Data Linage".

#### see also

- [Data lineage, Wikipedia](https://en.wikipedia.org/wiki/Data_lineage)

```#data-lineage, #dl, #data-provenance```

---

### Data Provenance

#### see

- [`Data Lineage`](#data-lineage)

```#data-provenance, #data-lineage```

---

### Data Sovereignty

```#data-sovereignty```

---

### Data Space

A "Data Space" is a dynamic collaboration of given [Data Domains](#data-domain). It can be also understood as an
isolated [Data Domain](#data-domain), populated by [Service Instances](#service.instance) (acting as
a [Data Provider](#data-provider) or [Data Consumer](#data-consumer)), so putting up a "Data Space".

A "Data Space" _comes to life_ when [data](#data) or, to be more
accurate, [Payload Data](#payload-data) is [exchanged](#data-exchange).

A [Data Domain](#data-domain) even exists _without_ exchanging [data](#data).

#### see

- [`Data Domain`](#data-domain)
- [`Data Provider`](#data-provider)
- [`Data Consumer`](#data-consumer)
- [`DataVerse`](#dataverse)
- [`Data`](#data)

```#data-space, #data-domain, #dataverse, #data```

---

### Data Type Property

```#datatypeproperty, #property```

---

### DataVerse

["DataVerse" (fua-extension)](../extension/dataverse/README.md) ([**DAVE**](./shortcut.md#dave)) is a collection
of [Data Domains](#data-domain), hovered
by [Data Spaces](#data-space).

#### see

- [`Data Domain`](#data-domain)
- [`Data Space`](#data-space)

```#dataverse, #data```

---

### Domain

A "Domain" expresses a collection of users, groups, [roles](#role) and credentials.

Domains are often equipped with [Services](#service), so those are [instantiated](#service-instance), _identifying_,
_authenticating_ and/or _authorizing_ [users](#problem-layer).

#### see

- [`Data Domain`](#data-domain)

#### see also

- [Active Directory, Services, Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/active-directory-domain-services)
- [Active Directory, Wikipedia](https://en.wikipedia.org/wiki/Active_Directory)

```#domain, #data-domain```

---

### Digital Twin

#### see also

- [Digital twin, Wikipedia](https://en.wikipedia.org/wiki/Digital_twin)

```#digital-twin, #twin```

---

## E

### Example

[`fua`](#fua) works with following examples:

#### ["The Weather Station"](../example/theweatherstation/README.md)

#### ["The Elevator"](../example/theelevator/README.md)

#### ["The Universe"](../example/theuniverse/README.md)

#### [Dataverse "The Universe"](../example/dataversetuni/README.md)

```#example, #weatherstation, #elevator, #unidataverse```

---

### External Identifier

#### see

- [`IDEX`](#idex)

---

## F

### Framework Universe Architecture

#### see

- [`fua`](#fua)

---

### fua

Shortcut for "Framework Universe Architecture", also used as prefix or namespace.

```#fua```

---

## G

### GAIAboX

The representative of working
[service instances and underlying applications](../gbx/README.md).

Shortcut is [`gbx`](#gbx).

#### see

- [`gbx`](../gbx/README.md)

```#gaiabox, #gbx```

---

### gbx

Acronym, shortcut and prefix of [`GAIAboX`](#gaiabox), the representative for services and applications.

```#gbx, #gaiabox```

---

### Generator

"Generator" is a classification of an [agent](#agent).

A Generator (an [agent](#agent) classified as a [Generator](#generator)) generates resources.

[Producer](#producer) is a narrower classification.

```#generator```

---

### Glossary

This document, presented to index `fua`.

```#glossary```

---

## I

### IA

Anthropocentric Information (**IA**) is a classification of [information](#information) and is generated by humans and
targeted to humans, so it is _human readable_.

It **MAY** also be read by machines, but reasoning is sometimes hard to achive and sometimes **NOT** possible.
If given _IA_ is machine readable and the machine _understands_ given piece of [data](#data),
representing _the_ [information](#information) it makes sense in accordance with the wishes of a human [agent](#agent)
(like [Alice](#alice)).

#### see also

- [anthropocentrism , Wikidata](https://www.wikidata.org/wiki/Q191624)

```#ia, #information```

---

### ID

#### see

- [Understanding "Identifier"](../understanding/identifier/README.md)

```#id, #identifier```

---

### Identifier

"Identifier" ([**ID**](#id)).

#### see

- [`ID`](#id)

```#identifier, #id```

---

### Identifier, external

#### see

- [IDEX](#idex)

---

### Identity Provider

"Identity Provider" [(**IdP**)](./shortcut.md#idp).

---

### Identifier, internal

#### see

- [`Internal Identifier`](#internal-identifier)

---

### IDEX

An "External Identifier" (**IDEX**) is generated by a external [domain](#domain) (or registry) and is used
to identify (unambiguously) a given resource in this external domain (registry).

A given resource (also equipped by its [Internal Identifer](#internal-identifier)) hosts this
External Identifier (**IDEX**).

#### see

- [Understanding "Identifier"](../understanding/identifier/README.md)

```#idex, #id, #identifier```

---

### Internal Identifier

An "Internal Identifier" is generated by given domain (as an [authority](#authority) to do so) and is used
to identify (unambiguously) a given resource in this domain.

#### see

- [Understanding "Identifier"](../understanding/identifier/README.md)

```#internal-identifier, #id```

---

### Information

Something derived from [Data](#data).

#### see

- [`Data`](#data)

#### see also

- [`Information (Wikidata)`](https://www.wikidata.org/wiki/Q11028)

```#information, #data```

---

### Information, anthropocentric

#### see

- [`IA`](#ia)

---

### IMPL

"Implementation" (**IMPL**) act as a _hint_ for implementers.

#### turtle

```turtle
## IMPL : Stay calm and keep coding!
rdfs:comment """IMPL : Stay calm and keep coding!"""@en
```

#### json

[Keep in mind...](../reading/README.md#json)

```json
// IMPL : Stay calm and keep coding!
{
    "rdfs:comment": "IMPL : Stay calm and keep coding!"
}
```

#### markdown

```markdown
#### IMPL

Stay calm and keep coding!
```

```#impl```

---

### Implementation

Implementation ([`IMPL`](#impl)).

#### see

- [`IMPL`](#impl)

---

### Infrastructure Data

### see

- [Understanding "Data and Information](../understanding/data_and_information/README.md)

```#infrastructure-data```

---

### Infrastructure Service

```#infrastructure-service```

---

## L

### Layer

Layering concepts by "Layer".

```#layer```

---

### Layer, Application

#### see

- [`Application Layer`](#application-layer)

---

### Layer, Data

#### see

- [`Data Layer`](#data-layer)

---

### Layer, Persistence

#### see

- [`Persistance Layer`](#persistence-layer)
- [`Layer`](#layer)

---

### Layer, Problem

#### see

- [`Problem Layer`](#problem-layer)

---

### Linked Data

At least one piece of [data](#data) (subject) stated to be linked to another piece of data (object).

_This_ link itself contains some information (like ([IA](#ia)): "I know how to resolve this link to _the_ object!"),
so maybe it might be a better idea to say "Linked Information" - but `fua' is glued to common sense and
uses [`Linked Data`](#linked-data).

#### see

```#linked-data```

---

### Logging Service

#### see

- [Logging Service (**DAVE**)](../extension/dataverse/README.md#logging-service).

```#logging-service```

---

## M

### Machine Readable Policy

A "Machine Readable Policy" (`MRP`) is a [policy](#policy) or contract, readable and interpretable by machines.

`fua`s implementation (`#impl`) of [Policies](#policy) is based
on the [`"Open Digital Rights Language", ODRL`](#open-digital-rights-language).

#### see

- [`Policy`](#policy)
- [`Open Digital Rights Language`](#open-digital-rights-language)
- [`Natural Language Policy`](#natural-language-policy)

```#machine-readable-policy, #policy```

---

### Meta Data

Data decorating given [Payload Data](#payload-data), like "where does Payload Data comes from?" or "when was Payload
Data generated?".

#### see

- [Understanding "Data and Information](../understanding/data_and_information/README.md)

#### see also

- [Meta Data, Wikipedia](https://en.wikipedia.org/wiki/Metadata)

```#meta-data, #data```

---

## N

### NARR

A "Narration" (**NARR**), something telling a story.

```#narr, #narration```

---

### Narration

"Narration" [(**NARR**)](#narr).

#### see

- [`narr`](#narr)

```#narration, #narr```

---

### Natural Language Policy

"Natural Language Policy" [(**NLP**)](#nlp).

#### see

- [`NLP`](#nlp)

```#natural-language-policy, #nlp```

---

### NLP

A Natural Language Policy (**NLP**) behaves as a policy or contract to be readable - and hopefully understandable - for
humans. Typically, such a policy can be spoken, or to outlive, written down.

#### see

- [`Policy`](#policy)
- [`Machine Readable Policy`](#machine-readable-policy)

#### see also

- [Clay Tablet, Wikipedia](https://en.wikipedia.org/wiki/Clay_tablet)

```#nlp, #natural-language-policy, #policy```

---

## O

### Object Property

#### see

- [`PropertyProperty`](#property)
- [`Data Type Property`](#data-type-property)

```#object-property, #property```

---

### ODRL

"Open Digital Rights Language" [(**ODRL**)](./shortcut.md#odrl)  is a
[Rights Expression Language (**REL**)](#rights-expression-language).

**ODRL** can be extended by [profiles](https://www.w3.org/TR/odrl-model/#profile). `fua` does so defining

- [`dacl`](../extension/decide/profile/dacl/README.md)
- [`tracl`](../extension/decide/profile/tracl/README.md)

### see also

- [ODRL Information Model 2.2, W3C](https://www.w3.org/TR/odrl-model/)
- [ODRL, Wikipedia](https://en.wikipedia.org/wiki/ODRL)
- [REL, Wikipedia](https://en.wikipedia.org/wiki/Rights_Expression_Language)

```#open-digital-rights-language, #odrl, #rights-expression-Language, #rel, #rights```

---

### Open Digital Rights Language

#### see

- [ODRL](#odrl)

#### see also

- [ODRL Information Model 2.2, W3C](https://www.w3.org/TR/odrl-model/)
- [ODRL, Wikipedia](https://en.wikipedia.org/wiki/ODRL)

---

## P

### Payload Data

"Payload Data" is a _classification_ of [data](#data) and expresses the main topic or [information](#information) of
given content. Accepting the definition this way, it can be seperated from [Meta Data](#meta-data), which carries
information _about_ the "Payload Data", like timestamping, type, provenance or ownership - to mention only some here.

"Payload Data" is allocated by an [agent](#agent) in its [role](#role) ["Data Provider"](#data-provider).

From the perspective of given data receiving [Data Consumer](#data-consumer): this (_the_ Payload Data) is what is
wanted (even the meta-data might be also interesting...).

Even Payload Data is sometimes _blended_ with Meta Data, it can be cleary devided
from [Infrastructure Data](#infrastructure-data).

#### see

- [`Meta Data`](#meta-data)
- [`Infrastructure Data`](#infrastructure-data)
- [Understanding "Data and Information"](../understanding/data_and_information/README.md)

#### see also

- [Payload Data, Wikipedia](https://en.wikipedia.org/wiki/Payload_(computing))

```#payload-data, #data```

---

### Persistence Layer

#### see also

- [Persistence (computer science), Wikipedia](https://en.wikipedia.org/wiki/Persistence_(computer_science))

```#persitance-layer, #layer```

---

### Physical Twin

#### see

- [`Base Twin`](#base-twin)
- [`Digital Twin`](#digital-twin)

```#physical-twin, #twin```

---

### Policy

A Policy behaves as contract or instruction, containing [rules](#rule) that **MAY**, **SHOULD** or **MUST** be
fulfilled.

#### see

- [`Natural Language Policy`](#natural-language-policy)
- [`Machine Readable Policy`](#machine-readable-policy)
- [`Rule`](#rule)

```#policy```

---

### Policy, Machine Readable

#### see

- [`Machine Readable Policy`](#machine-readable-policy)

---

### Policy, Natural Language

#### see

- [`Natural Language Policy`](#natural-language-policy)

---

### Problem Layer

The "Problem Layer", sometimes exposed with its numerical position "8", populated by [agents](#agent)
holding [role](#role) ["Data Consumer"](#data-consumer), also mentioned as [service](#service) or application user.

#### see

- [`Problem Layer`](#problem-layer)

```#problem-layer, #layer```

---

### Producer

"Producer" is a classification of an [agent](#agent).

A Producer (an [agent](#agent) classified as a [Producer](#producer)) produces [Products](#product).

[Generator](#generator) is a broader classification.

A Manufacturer (an [agent](#agent) classified as a [Producer](#producer)) produces physical [Products](#product).

#### see

- [`Product`](#product)
- [`Generator`](#generator)

```#producer, #product```

---

### Process

A "Process" has a beginning, a duration and an end.

A Process is interruptible.

#### see

- [`Action`](#action)
- [`Activity`](#activity)

```#process```

---

### Product

"Product" is a classification of a resource.

#### see

- [`Producer`](#producer)
- [`Data`](#data)

```#product, #producer```

---

### Property

#### see

- [`Data Type Property`](#data-type-property)
- [`Object Property`](#object-property)

```#property```

---

### Provider

"Provider" is a [role](#role).

An [agent](#agent), providing resources, act in its [role](#role) [Provider](#Provider).

#### see

- [`Data Provider`](#data-provider)

```#provider, #role```

---

## R

### Rights

```#rights```

---

### REL

"Rights Expression Language" ([**REL**](./shortcut.md#rel)) is a language to express [rights](#rights).

### see

- [ODRL](#odrl)

#### see also

- [REL (Rights Expression Language), Wikipedia](https://en.wikipedia.org/wiki/Rights_Expression_Language)
- [ODRL Information Model 2.2, W3C](https://www.w3.org/TR/odrl-model/)
- [ODRL (Open Digital Rights Language), Wikipedia](https://en.wikipedia.org/wiki/ODRL)

```#rel, #rights-expression-Language, #rights```

---

### Remote Control

[Controlling](#controller) a remote resource.

A "Remote Control" could also be understood as a [Service Instance](#service-instance) (designed under the paradigm
of acting as a [Digital Twin](#digital-twin)), proclaiming [commands](#command) directed to the [Base Twin](#base-twin)
by _pushing_ those.

```#remote-control, #control, #command```

---

### Rights Expression Language

"Rights Expression Language".

#### see

- [rel](#rel)

```#rights-expression-Language, #rel, #rights```

---

### Role

```#role```

---

### Rule

A "Rule" behaves as an _imperative_ that **MAY**, **SHOULD** or **MUST** be fulfilled. A Rule **MAY** contain
[constraints](#constraint), to clarify the topic handled and lead to a _(mandatory) action_ to be executed
by receiving assignee.

Rules are typically presented in [policies](#policy).

#### see

- [`Policy`](#policy)
- [`Natural Language Policy`](#natural-language-policy)
- [`Machine Readable Policy`](#machine-readable-policy)
- [`Open Digital Rights Language`](#open-digital-rights-language)

```#rule, #constraint, #policy```

---

## S

### Service

A "Service" is described by its [model](#service-model) and gets up-and-running
being [instantiated](#service-instance).

#### see

- [`Service Model`](#service-instance)
- [`Service Instance`](#service-model)
- [GAIAboX (GBX)](../gbx/README.md)

#### see also

- [Service (systems architecture), Wikipedia](https://en.wikipedia.org/wiki/Service_(systems_architecture))

```#service```

---

### Service, Web

#### see

- [`Web Service`](#web-service)
- [GAIAboX (GBX)](../gbx/README.md)

---

### Service Instance

A "Service Instance" is an up-and-running [Service](#service), hosted on a _server_.

#### see

- [GAIAboX (GBX)](../gbx/README.md)

```#service-instance```

---

### Service Layer

The "Service Layer" (as a sub-[layer](#layer) of [`Application Layer`](#application-layer)) behaves as the most
upfront layer of given [application](#application). The application is an instantiated [service](#service),
leading to an up-and-running [Service Instance](#service-instance) providing its attainment to .

#### see

- [GAIAboX (GBX)](../gbx/README.md)

```#service-layer```

---

### Service Model

A "Service Model" describes (and sometimes configures) a [Service](#service).

#### see

- [GAIAboX (GBX)](../gbx/README.md)

```#service-model```

---

### shacl

The Shape Constraint Language.

#### see

- [`turtle`](#turtle)

#### see also

- [Shapes Constraint Language (SHACL)](https://www.w3.org/TR/shacl/)

```#shacl```

---

### Shapes Constraint Language

The Shapes Constraint Language.

#### see

- [`shacl`](#shacl)

#### see also

- [Shapes Constraint Language (SHACL)](https://www.w3.org/TR/shacl/)

---

### Subject

```#subject```

---

### System

```#system```

---

## T

### tag

Property for tagging given subject.

```#tag```

---

### Terms Of Use

The Terms of using something. The Terms are formulated by an Agent, acting as a Provider and understood and fulfilled
by given Agent acting as a consumer.

#### see

- [`Usage Control`](#usage-control)

#### see also

- [termsOfUse, "Verifiable Credentials Data Model v1.1"](https://www.w3.org/TR/vc-data-model/#terms-of-use)

```#terms-of-use, #usage-control```

---

### Timestamp

fua uses "Timestamp" as a generic property. Its value is of
type [`xsd:dateTimestamp`](https://www.w3.org/TR/xmlschema11-2/#dateTimeStamp)

#### IMPL

"Timestamp" interpreted as a [time instant (Time Ontology in OWL)](https://www.w3.org/TR/owl-time/#time:Instant).

```#timestamp, #time-instant, #time```

---

### TRACL

The "Transformation, Translation, Transmutation and Conversion Language"
(**[TRACL](../extension/decide/profile/tracl/README.md)**) as an **[ODRL](#odrl)**-profile defined by `fua`.

#### see

- [`Decide Profile TRACL`](../extension/decide/profile/tracl/README.md)
- [`ODRL ("Open Digital Rights Language")`](#odrl)

```#tracl, #control-language, #control```

---


### Trust

```#trust```

---

### Trusted Data Exchange

A given [_Data Owner_](#data-owner) (and a [agent](#agent), [providing data](#data-provider) acting on behalf of given
Data Owner) hands over [data](#data) to an agent, acting as a [Data Consumer](#data-consumer), assuming that
the consumer handles _the_ data in a way that is **NOT** contrary to Data Owners interest.

```#trusted-data-exchange, #data-exchange```

---

### turtle

"Terse RDF Triple Language" (**turtle**).

Ontology `fua`, extensions, profiles and examples are written in `turtle`.

#### see

- [`shacl`](#shacl)

#### see also

- [turtle](https://www.w3.org/TR/turtle/)
- [Turtle (syntax), Wikipedia](https://en.wikipedia.org/wiki/Turtle_(syntax))

```#turtle, #ttl```

---

### Twin

```#twin, #base-twin, #digital-twin, #physical-twin```

---

### Twin, Digital

#### see

- [`Digital Twin`](#digital-twin)

---

### Twin, Base

#### see

- [`Base Twin`](#base-twin)

---

### Twin, Physical

#### see

- [`Physical Twin`](#physical-twin)

---

## U

### Usage Control

[Controlling](#controller) usage of given resource ([data](#data)) to accomplish **and**
preserve [_Data Sovereignty_](#data-sovereignty).

#### see also (W3C)

- [termsOfUse, "Verifiable Credentials Data Model v1.1"](https://www.w3.org/TR/vc-data-model/#terms-of-use)

##### see also (International Data Spaces, IDS)

- ["Data Sovereignty: Updated Position Paper on Data Usage Control in the IDS" (Eitel)](https://internationaldataspaces.org/data-sovereignty-updated-position-paper-on-data-usage-control-in-the-ids/)
- ["IDS Usage Control Policies" (Data Space Connector)](https://international-data-spaces-association.github.io/DataspaceConnector/Documentation/v5/UsageControl)
- ["Usage Control" (IDS Trusted Connector)](https://industrial-data-space.github.io/trusted-connector-documentation/docs/usage_control/)

```#usage-control, #terms-of-use, #control-language, #control, #ids```

---

## W

### Web Service

#### see also

- [`Web Service`, Wikipedia](https://en.wikipedia.org/wiki/Web_service)

```#web-service, #ws```

---