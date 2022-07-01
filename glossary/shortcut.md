# Shortcut

Shortcuts, abbreviations and acronyms used in `fua`.

| shortcut        | Long                                                         | Comment                                     |
|-----------------|:-------------------------------------------------------------|---------------------------------------------|
| [ACL](#acl)     | [Access Control List](./README.md#acl)                       |                                             |
| [ATS](#ats)     | [Authentication Service](./README.md#authentication-service) |                                             |
| [AOS](#aos)     | [Authorization Service](./README.md#authorization-service)   |                                             |
| [AU](#au)       | [Authority](./README.md#authority)                           |                                             |
| [CA](#ca)       | [Certificate Authority](./README.md#certificate-authority)   |                                             |
| [CB](#cb)       | [Certification Body](./README.md#certification-body)         | same as: [NOTA](#nota)                      |
| [CH](#ch)       | [Clearing House](./README.md#clearing-house)                 |                                             |
| [DACL](#dacl)   | [Dynamic Access Control Language](./README.md#dacl)          |                                             |
| [DAVE](#dave)   | [DataVerse](./README.md#dataverse)                           |                                             |
| [DS](#ds)       | [Data Space](./README.md#data-space)                         |                                             |
| [EC](#ec)       | [Eco System](./README.md#eco-system)                         | Data.                                       |
| [FTIME](#ftime) | `fua` time                                                   | [ODRL](../glossary/README.md#odrl) profile. |
| [IA](#ia)       | Information, Anthropocentric                                 |                                             |
| [ID](#id)       | Identifier                                                   |                                             |
| [IDE](#ide)     | Integrated Development Environment                           |                                             |
| [IdP](#idp)     | Identity Provider                                            |                                             |
| [LS](#ls)       | Logging Service                                              |                                             |
| [NLP](#nlp)     | Natural Language Policy                                      |                                             |
| [NOTA](#nota)   | Notarization                                                 | same as: [CB](#cb)                          |
| [OA](#oa)       | Operating Agent                                              |                                             |
| [OC](#oc)       | Operating Company                                            |                                             |
| [OP](#op)       | Operating Person                                             |                                             |
| [ORDL](#odrl)   | Open Digital Rights Language                                 |                                             |
| [REG](#reg)     | Registry                                                     |                                             |
| [REL](#rel)     | Rights Expression Language                                   |                                             |
| [REM](#rem)     | Remark                                                       |                                             |
| [TAG](#tag)     | Tag                                                          |                                             |
| [TBC](#tbc)     | To Be Clarified!                                             |                                             |
| [TBD](#tbd)     | To Be Discussed!                                             |                                             |
| [TODO](#todo)   | To Do!                                                       |                                             |
| [TLDR](#tldr)   | Too Long, Didn't Read!                                       |                                             |
| [TRACL](#tracl) | Transformation Control Language                              |                                             |
| [UCON](#ucon)   | [Usage Control](./README.md#usage-control)                   |                                             |
| [WAC](#wac)     | Web Access Control                                           |                                             |

*Table of `fua` shortcuts*.

## ACL

"**A**ccess **C**ontrol **L**ist".

[ACL](./README.md#acl).

```#acl, #acces-control-list```

## ATS

[**A**u**t**hentication **S**ervice](./README.md#authentication-service).

```#ats, #authentication-service```

## AOS

[**A**uth**o**rization **S**ervice](./README.md#authorization-service).

```#aos, #autherization-service```

## AU

[**Au**thority](../glossary/README.md#authority).

```#au, #authority```

## CA

[**C**ertificate **A**uthority](./README.md#certificate-authority).

```#ca, #certificate-authority, #authority, #au```

## CB

[**C**ertification **B**ody](./README.md#certification-body).

same as:

- [Notarisation (**NOTA**)](#nota)

```#cb, #certification-body```

## CH

[**C**learing **H**ouse](./README.md#clearing-house).

```#ch, #clearing-house```

## DACL

"**D**ynamic **A**access **C**ontrol **L**anguage"

### see

- [`dacl` (Decide, profile)](../extension/decide/profile/dacl/).

```#dacl, #dynamic-acces-control-language```

## DAVE

[**Da**ta**Ve**rse](./README.md#dataverse).

Preferred namespace prefix: `dave`

#### Example

##### turtle

```turtle
@prefix dave: <https://www.nicos-rd.com/fua/dataverse#> .
```

*A turtle example of using 'dave' as a prefix*.

##### json

```json
{
    "@context": [
        { "dave": "https://www.nicos-rd.com/fua/dataverse#" }
    ]
}
```

*A json (json+ld) example of using 'dave' as a prefix*.

The uppercase presentation ([**DAVE**](#dave)) is often used to expose the _concept_
of [DataVerse](./README.md#dataverse).

```#dave, #dataverse```

## DS

[**D**ata **S**pace](./README.md#data-space).

```#ds, #data-space```

## FTIME

"**F**ua **TIME**"

**FTIME** is an [**ODRL**](../glossary/README.md#odrl) profile.

Preferred namespace prefix: `ftime`

### see

- [`ftime` (Decide, profile)](../extension/decide/profile/ftime/).

```#ftime```

## IA

[**I**nformation, **A**nthropocentric](./README.md#ia).

```#ia, #information```

## ID

[**Id**entifier](./README.md#identifier).

```#id, #identifier```

## IDE

"**I**ntegrated **D**evelopment **E**nvironment"

```#ide, #integrated-development-environment```

## IdP

[**Id**entity **P**rovider](./README.md#identity-provider).

```#idp, #identity-provider```

## EC

[**E**co **S**ystem](./README.md#eco-system).

```#ec, #eco-system```

## LS

[**L**ogging **S**ervice](./README.md#logging-service).

```#ls, #logging-service```

## NLP

[**N**atural **L**anguage **P**olicy](./README.md#nlp).

```#nlp, #natural-language-policy```

## NOTA

["**Nota**risation"](./README.md#notarization).

same as:

- [Certification Body (**CB**)](#cb)

```#nota, #notarization```

## OA

[**O**perating **A**gent](./README.md#operating-agent).

A role of given [Agent](./README.md#agent), so doing something.

```#oa, #operating-agent```

## OC

[**O**perating **C**ompany](./README.md#operating-company).

Sub Class of [Operating Agent (OA)](#oa).
Sub Class of [`org:Organization`](https://www.w3.org/TR/vocab-org/#class-organization).

```#oc, #operating-company```

## OP

[**O**perating **P**erson](./README.md#operating-person).

Sub Class of ['Operating Agent' (OA)](#oa).
Sub Class of ['foaf:Person'](http://xmlns.com/foaf/0.1/).

```#op, #operating-person```

## ODRL

[**O**pen **D**igital **R**ights **L**anguage](./README.md#odrl).

```#odrl```

## REG

[**Re**gistry](./README.md#registry)

```#reg, #registry```

## REL

[*R*ights *E*xpression *L*anguage](./README.md#rel).

```#rel, #rights-expression-language, #rights```

## REM

**Rem**ark.

### Example

#### turtle

```turtle
## REM: this is it!
```

*A remark (**REM**) shown in `turtle`*.

```#rem, #remark```

## TAG

```#tag```

## TBC

**T**o **B**e **C**larified!

### Description

Something has to be clarified.

### Comment

One or more [agents](./README.md#agent) - maybe some [persons](./README.md#person) collaborate - have to clarify a
topic.

### Example

> TBC: is it really what it seems?

#### Agents

> TBC@JLA: could be that it's not ok?

```#tbc```

## TBD

**T**o **B**e **D**iscussed!

Something has to be discussed.

### Comment

Two or more [agents](./README.md#agent) - maybe some [persons](./README.md#person) - have to discuss a topic.

### Example

> TBD: **MAY**be we have to come closer to the problem!

#### Agents

> TBD@JLA,SPE: what is going on here?

```#tbd```

## TODO

**T**o **D**o!

Something has to be done.

### Example

> TODO: get it up an' running!

#### turtle

```turtle
## TODO: fix this immediatly!!!
```

*A To Do (**TODO**) shown in `turtle`*.

#### Agents

> TODO@JLA: it's your job!

```#todo```

## TLDR

**T**oo **L**ong, **D**idn't **R**ead!

### turtle

```turtle
## TLDR: A very, very long story (very boring, indeed!).
```

*Example of a very long text in `turtle`*.

### markdown

```markdown
## TLDR

A very, very long story (very boring, indeed.
 And it gets **NOT** better written in `markdown`!!!).

---
```

*Example of a very long text in `markdown`*.

```#tldr```

## TRACL

"**T**ransformation, **T**ranslation, **T**ransmutation and **C**onversion **C**ontrolling **L**anguage"

**TRACL** is an [**ODRL**](../glossary/README.md#odrl) profile.

Preferred namespace prefix: `tracl`

### see

- [tracl (Decide, profile)](../extension/decide/profile/tracl/).

```#tracl```

## UCON

"**U**sage **Co**ntrol"

```#ucon, #usage, #control```

## WAC

"**W**eb **A**eccess**C**ontrol"

```#wac, #web-access-control, #access, #control```

---