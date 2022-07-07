# `fua` DataVerse

The DataVerse ([**DAVE**](../../glossary/shortcut.md#dave)) is an Eco System.

The DataVerse is an Eco Systems of Eco Systems.

## Table of Content

- [Introduction](#introduction)
- [Authority](#authority)
- [Eco System](#eco-system)
- [Operating Agent](#operating-agent)
- [Domain](#domain)
    - [Domain Monitoring](#domain-monitoring)
- [Registry](#registry)
- [Logging Service](#logging-service)
- [Clearing House](#clearing-house)
- [Identity Provider](#identity-provider)
    - [Certification Body](#certification-body)
    - [Notarisation](#notarisation)
    - [Certificate Authority](#certificate-authority)
    - [Identity Providing Services](#identity-providing-services)
        - [Authentication Service](#authentication-service)
        - [Authorization Service](#authorization-service)
- [DataSpace](#dataspace)
- [Trust](#trust)
    - [Domain Trust](#domain-trust)
        - [Intra-Domain Trust](#intra-domain-trust)
        - [Extra-Domain Trust](#extra-domain-trust)
    - [Trust Policy](#trust-policy)
        - [Trust Request Policy](#trust-request-policy)
        - [Trust Offer Policy](#trust-offer-policy)
        - [Trust Agreement Policy](#trust-agreement-policy)

*Table of Content "DataVerse"*.

---

## Introduction

The "DataVerse" ([**DAVE**](../../glossary/shortcut.md#dave)), a collection of [Eco System](#eco-system),
[Domains](#domain) and [Data Spaces](#dataspace).

It is populated by [Infrastructure Services](../../glossary/README.md#infrastructure-service) (depending on
given [Eco System](#eco-system)),
like [Authentication Services](#authentication-service) and [Authorization Services](#authorization-service), or
Catalogues, Brokers (to be understood as _something_
like ["Yellow Pages", Wikipedia](https://en.wikipedia.org/wiki/Yellow_pages)). And - completing the roundel - Logging
Services and Clearing Houses.

Other Services, bring one [Eco System](#eco-system) or [DataSpace](#dataspace) to life, are those (evolving the main
topic ["Data Exchange"](../glossary/README.md#data-exchange) on
the ["Payload Data"](../glossary/README.md#payload-data) Layer) acting
under well known [roles](../glossary/README.md#role) ["Data Provider"](../glossary/README.md#data-provider)
and/or ["Data Consumer"](../glossary/README.md#data-consumer).

The namespace prefix of "DataVerse" is `dave`.

```turtle
@prefix dave: <https://www.nicos-rd.com/fua/dataverse#> .
@prefix tuni: <https://www.nicos-rd.com/data/theuniverse/> .

tuni:
    ## tuni stated to be an Universe
    a                univ:Universe ;
    ## tuni stated to be a DataVerse
    a                dave:DataVerse ;
    ## tuni stated to be a DataVerse Eco System
    a                dave:EcoSystem ;
    rdfs:label       "The Universe"@en ;
    univ:galaxy      tuni:MilkyWay ;
    ## region DataVerse
    dave:dataVerse   tuni: ;
    ## endregion DataVerse
    ## region EcoSystem
    dave:ecoSystem   tuni: ;
    ## endregion EcoSystem
    rdfs:isDefinedBy tuni: ;
.

```

*The Universe stated to be a DataVerse and a Eco System*.

For more elaborated tweaks see [this](../../example/dataversetuni/README.md).

---

## Authority

```#authority```

---

## Eco System

Eco System ([**EC**](../../glossary/shortcut.md#ec)).

```#eco-system```

---

### Operating Agent

Operating Agent ([**OA**](../../glossary/shortcut.md#oa)).

```#operating-agent, #agent```

---

### Domain

A Domain holds none, one, or many [Registries](#registry) (as a service instances)
for [authentication](#authentication-service) and/or [authorization](#authorization-service).

The sum of all given [Registries](#registry) expresses *a* Domain.

A given Domain exposes a Federation (a collaboration), containing all [Agents](../../glossary/README.md#agent) (like
participants, [Service Instances](../../glossary/README.md#service-instance), etc.).

```#domain```

---

#### Domain Monitoring

```#domain-monitoring, #domain```

---

### Registry

Registry [(**REG**)](../../glossary/shortcut.md#reg).

```#registry, #reg```

---

### Logging Service

Logging Service [(**LS**)](../../glossary/shortcut.md#ls).

```#logging-service, #ls```

---

### Clearing House

Clearing House [(**CH**)](../../glossary/shortcut.md#ch).

```#clearing-house, #ch```

---

### Identity Provider

The Identity Provider ([**IdP**](../../glossary/shortcut.md#idp)) **MAY** consist of two
Authorities ([Certification Body](#certification-body) and
[Certificate Authority](#certificate-authority)) and [identity providing services](#identity-providing-services),
tailored in [Authentication Service](#authentication-service) and [Authorization Service](#authorization-service).

```#identity-provider, #idp```

---

#### Certification Body

A Certification Body (**CB**) is an [authority](#Authority).

See also (same as): [Notarisation](#notarisation).

```#certification-body, #cb, #authority, #notarisation, #nota```

---

#### Notarisation

A Notarisation ([**NOTA**](../../glossary/shortcut.md#nota)) is an [Authority](#authority).

See also (same as): [Certification Body](#certification-body).

```#notarisation, #nota, #authority, #certification-body, #cb```

---

#### Certificate Authority

A Certificate Authority [(**CA**)](../../glossary/shortcut.md#ca) is an [authority](#authority).

```#certificate-authority, #ca, #authority```

---

#### Identity Providing Services

##### Authentication Service

An Authentication Service [(**ATS**)](../../glossary/shortcut.md#ats) is a [Service](../../glossary/README.md#service)
and acts being
a [Service Instance](../../glossary/README.md#service-instance). Working correctly the Authentication Service (instance)
verifies that given [Agent](../../glossary/README.md#agent) is what it claims to be.

```#authentication-service, #ats, #authentication, #service```

---

##### Authorization Service

An Authorization Service [(**AOS**)](../../glossary/shortcut.md#aos) is a [Service](../../glossary/README.md#service)
and acts being a [Service Instance](../../glossary/README.md#service-instance). Working
correctly the Authorization Service (instance) presents credentials related to
given [Agent](../../glossary/README.md#agent).

```#authorization-service, #aos, #authorization, service```

---

## DataSpace

A DataSpace [(**DS**)](../../glossary/shortcut.md#ds) (_the_ DataSpace) is brought to life by a dynamic landscape
of [data](../glossary/README.md#data).

A DataSpace is a ***Trusted DataSpace*** if it acts on top of underlying [Domain(s)](#domain), onboarding-mechanisms,
infrastructure components, providing services, etc. - by given [Eco System](#eco-system) and those normative
rules, models, schemata and basic mechanisms stated by *this* Eco System with the help of
*this* Eco Systems [Identity Provider](#identity-provider).

So, all this done well acting Agents [(Data Exchange)](../../glossary/README.md#data-exchange) will be provided
with given certainty everything is safe, maybe down to handling data correctly: a Data Provider, confer rights
to given Data Consumer using those data - *the* Data Provider trusts *the* Data Consumer to use data, formulated
in given [the terms of use](../../glossary/README.md#terms-of-use): *the* Data Provider keeps its
[Data Sovereignty](../../glossary/README.md#data-sovereignty) and the [***Intra-Domain***](#intra-domain)-Trust is
established.

A DataSpace **MAY** overstretch two or more [Eco Systems](#eco-system). If this arrives, there **MAY** be
*a* [trust](#trust) between those [Domains](#domain) or at least between two [Agents](../../glossary/README.md#agent)
hosted by (those ***two***) different domains, understanding the mechanisms and rules of each other. If this happens
this way the [***Extra-Domain***](#extra-domain)-Trust is established - hopefully based on
a [Trust Policy](#trust-policy)...

```#dataspace, #data```

---

## Trust

```#trust```

### Domain Trust

```#domain-trust, #trust```

#### Intra-Domain Trust

```#intra-domain-trust, #domain-trust, #trust```

---

#### Extra-Domain Trust

```#extra-domain-trust, #domain-trust, #trust```

---

### Trust Policy

```#trust-policy, #trust```

#### Trust Request Policy

A "Trust Request Policy" is a [Trust Policy](#trust-policy).

The requesting Agent generates *the* Trust Request from the perspective of given requested Party (Agent).
Doing so, requesting Agent is formulated ind *the* Trust Request being *the* "assignee" (role) - as given Party
receiving the
desired credentials at the end of the workflow.

*The* issuing Party is formulated in *this* Trust Request as *the* "assigner" (role), publishing the desired credentials
at the end of the workflow.

```#trust-request-policy, #trust-policy, #trust```

---

#### Trust Offer Policy

A "Trust Offer Policy" is a [Trust Policy](#trust-policy).

The *assigner* formulates a Trust Offer. This Offer ***MAY*** be based on a
preceding [Trust Request](#trust-request)). The *assigner* passes *the* Trust Offer to given *assignee*,

```#trust-offer-policy, #trust-policy, #trust```

---

#### Trust Agreement Policy

A "Trust Agreement Policy" is a [Trust Policy](#trust-policy).

A Trust Agreement is a contract between given *assigner* and *assignee*, expressing under wich circumstance aimed
trust will be won.

From the perspective of an up-and-running [Data Exchange](../../glossary/README.md#data-exchange) given trust might be
unidirectional: the *assingee* (or better, the Service Instances acting on the *assignee*-side)
as [Data Consumer](../../glossary/README.md#data-consumer) is able to consume *assigners*
[Data Providers](../../glossary/README.md#data-provider), but **NOT** (unidirectional!) the other way around.

A Trust Agreement can be *bidirectional*.

> ***TBC***: A Trust Agreement can be *multi-directional*?

```#trust-agreement-policy, #trust-policy, #trust```

---

```#dataverse, #dave```

---