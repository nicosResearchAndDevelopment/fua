# `fua` DataVerse

The "DataVerse" ([**DAVE**](../../glossary/shortcut.md#dave)) model as a container for [Data Domains](#data-domain)
, [Data Spaces](#data-space),
and [Eco System](#eco-system).

The namespace prefix of "DataVerse" is `dave`.

```turtle
@prefix dave: <https://www.nicos-rd.com/fua/dataverse#> .
@prefix tuni: <https://www.nicos-rd.com/data/theuniverse/> .

tuni:
    a                univ:Universe ;
    rdfs:label       "The Universe"@en ;
    univ:galaxy      tuni:MilkyWay ;
    dave:dataVerse   tuni:dataverse ;
    rdfs:isDefinedBy tuni: ;
.

tuni:dataverse
    a dave:DataVerse ;
.
```

*The Universe stated holding a DataVerse*

```#dataverse, #dave```

---

## Introduction

The "DataVerse", a collection of [Eco System](#eco-system), [Domains](#data-domain) and [Data Spaces](#data-space).

It is populated by [Infrastructure Services](../../glossary/README.md#infrastructure-service) (depending on
given [Eco System](#eco-system)),
like [Authentication Services](#authentication-service) and [Authorization Services](#authorization-service), or
Catalogues, Brokers (to be understood as _something_
like ["Yellow Pages", Wikipedia](https://en.wikipedia.org/wiki/Yellow_pages)). And - completing the roundel - Logging
Services and Clearing Houses.

Other Services, bring one [Eco System](#eco-system) or [Data Space](#data-space) to life, are those (evolving the main
topic ["Data Exchange"](../glossary/README.md#data-exchange) on
the ["Payload Data"](../glossary/README.md#payload-data) Layer) acting
under well known [roles](../glossary/README.md#role) ["Data Provider"](../glossary/README.md#data-provider)
and/or ["Data Consumer"](../glossary/README.md#data-consumer).

---

## Authority

```#authority```

---

## Eco System

Eco System ([**EC**](../../glossary/shortcut.md#ec)).

```#eco-system```

---

### Operating Agent

Operating Agent ([**OA**](../../glossary/shortcut.md#oa).

```#operating-agent```

---

### Domain

A Domain holds none, one, or many [Registries](#registry) (as a service instances)
for [authentication](#authentication-service) and/or [authorization](#authorization-service).

The sum of all given [Registries](#registry) express the Domain.

A given Domain exposes a Federation (a collaboration) , containing all [Agents](../../glossary/README.md#agent) (like
participants, [service instances](../../glossary/README.md#service-instance), etc.).

```#domain```

---

### Registry

Logging Service [(**REG**)](../../glossary/shortcut.md#reg).

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

```#certification-body, #cb, #notarisation, #authority```

---

#### Notarisation

A Notarisation ([**NOTA**](../../glossary/shortcut.md#nota)) is an [authority](#authority).

```#notarisation, #nota, #authority```

---

#### Certificate Authority

A Certificate Authority [(**CA**)](../../glossary/shortcut.md#ca) is an [authority](#authority)(

```#certificate-authority, #ca, #authority```

---

#### Identity Providing Services

##### Authentication Service

A Authentication Service [(**ATS**)](../../glossary/shortcut.md#ats) is a [Service](../../glossary/README.md#service)
and acts being
a [Service Instance](../../glossary/README.md#service-instance). Working correctly the Authentication Service (instance)
verifies that given [Agent](../../glossary/README.md#agent) is what it claims to be.

```#authentication-service, #ats, #authentication, #service```

---

##### Authorization Service

An Authorization Service [(**AOS**)](../../glossary/shortcut.md#aos) is a [Service](../../glossary/README.md#service)
and acts being
a [Service Instance](../../glossary/README.md#service-instance) . Working
correctly the Authorization
Service (instance)
presents credentials related to given [Agent](../../glossary/README.md#agent).

```#authorization-service, #aos, #authorization, service```

---

## Data Space

A Data Space [(**DS**)](../../glossary/shortcut.md#ds) (_the_ Data Space) is brought to life by a dynamic landscape
of [data](../glossary/README.md#data)
and acts on top of underlying [Domain(s)](#domain), the infrastructure components, providing services boot
given [Eco System](#eco-system) and those normative rules, models, schemata and basic mechanics stated by _this_ Eco
System with the
help of the [Identity Provider](#identity-provider).

A Data Space **MAY** overstretch two or more [Eco Systems](#eco-system). If this arrives, there **MAY** be trusts
between those [Domains](#domain) or at least between two [Agents](../../glossary/README.md#agent) hosted by (those two)
different domains, understanding the authentication mechanisms, the verification of identities, the terms of using data
and - last but not least - the semantics...

```#data-space```

---

## Trust

```#trust```

---