# Shortcut

Shortcuts, abbreviations and acronyms used in `fua`.

| shortcut        | Description                        | Comment                    |
|-----------------|:-----------------------------------|----------------------------|
| [ATS](#ats)     | Authentication Service             |                            |
| [AOS](#aos)     | Authorization Service              |                            |
| [AU](#au)       | Authority                          |                            |
| [CA](#ca)       | Certificate Authority              |                            |
| [CB](#cb)       | Certification Body                 | same as: [**NOTA**](#nota) |
| [CH](#ch)       | Clearing House                     |                            |
| [DACL](#dacl)   | Dynamic Access Control Language    |                            |
| [DAVE](#dave)   | DataVerse                          |                            |
| [DS](#ds)       | Data Space                         |                            |
| [EC](#ec)       | Eco System                         | Data.                      |
| [IA](#ia)       | Information, Anthropocentric       |                            |
| [ID](#id)       | Identifier                         |                            |
| [IDE](#ide)     | Integrated Development Environment |                            |
| [IdP](#idp)     | Identity Provider                  |                            |
| [LS](#ls)       | Logging Service                    |                            |
| [NLP](#nlp)     | Natural Language Policy            |                            |
| [NOTA](#nota)   | Notarization                       | same as: [**CB**](#cb)     |
| [OA](#oa)       | Operating Agent                    |                            |
| [OC](#oc)       | Operating Company                  |                            |
| [OP](#op)       | Operating Person                   |                            |
| [ORDL](#odrl)   | Open Digital Rights Language       |                            |
| [REG](#reg)     | Registry                           |                            |
| [REL](#rel)     | Rights Expression Language         |                            |
| [REM](#rem)     | Remark                             |                            |
| [TBC](#tbc)     | To Be Clarified!                   |                            |
| [TBD](#tbd)     | To Be Discussed!                   |                            |
| [TODO](#todo)   | To Do!                             |                            |
| [TLDR](#tldr)   | Too Long, Didn't Read!             |                            |
| [TRACL](#tracl) | Transformation Control Language    |                            |

_Table: `fua` shortcuts_.

## ATS

[Authentication Service](./README.md#authentication-service).

---

## AOS

[Authorization Service](./README.md#authorization-service).

---

## AU

Authority.

---

## CA

[Certificate Authority](./README.md#certificate-authority).

---

## CB

[Certification Body](./README.md#certification-body).

### Comment

same as:

- [Notarisation (**NOTA**)](#nota)

---

## CH

[Clearing House](./README.md#clearing-house).

---

## DACL

---

## DAVE

[DataVerse](./README.md#dataverse).

### Comment

`dave` is used as a (preferred) namespace prefix, like

#### Example

##### turtle

```turtle
@prefix dave: <https://www.nicos-rd.com/fua/dataverse#> .
```

_A turtle example of using 'dave' as a prefix._

##### json

```json
{
    "@context": [
        { "dave": "https://www.nicos-rd.com/fua/dataverse#" }
    ]
}
```

_A json (json+ld) example of using 'dave' as a prefix._

The uppercase presentation ([**DAVE**](#dave)) is often used to expose the _concept_
of [DataVerse](./README.md#dataverse).

---

## DS

[Data Space](./README.md#data-space).

---

## IA

[Information, Anthropocentric](./README.md#ia).

---

## ID

[Identifier](./README.md#identifier).

---

## IDE

Integrated Development Environment.

---

## IdP

[Identity Provider](./README.md#identity-provider).

---

## EC

### Description

Eco System.

---

## LS

[Logging Service](./README.md#logging-service).

---

## NLP

[Natural Language Policy](./README.md#nlp).

---

## NOTA

### Description

Notarisation.

### Comment

same as:

- [Certification Body (**CB**)](#cb)

---

## OA

Operating Agent.

### Description

A role of given [Agent](./README.md#agent), so doing something.

---

## OC

Operating Company.

Sub Class of ['Operating Agent' (**OA**)](#oa).
Sub Class of ['org:Organization'](https://www.w3.org/TR/vocab-org/#class-organization).

---

## OP

Operating Company.

Sub Class of ['Operating Agent' (**OA**)](#oa).
Sub Class of ['foaf:Person'](http://xmlns.com/foaf/0.1/).

---

## ODRL

[Open Digital Rights Language](./README.md#odrl).

---

## REG

Registry.

---

## REL

[Rights Expression Language](./README.md#rel).

---

## REM

Remark.

### Example

#### turtle

```turtle
## REM: this is it!
```

_A remark (**REM**) shown in `turtle`_.

---

## TBC

To Be Clarified!

### Description

Something has to be clarified.

### Comment

One or more agents have to clarify a topic.

### Example

> TBC: is it really what it seems?

#### Agents

> TBC@JLA: could be that it's not ok?

---

## TBD

To Be Discussed!

### Description

Something has to be discussed.

### Comment

Two or more agents have to discuss a topic.

It can be extended by agents.

### Example

> TBD: we have to get a little bit closer to the problem!

#### Agents

> TBD@JLA,SPE: what is going on here?

---

## TODO

To Do!

### Comment

Something has to be done.

### Example

> TODO: get it up an' running!

#### turtle

```turtle
## TODO: fix this immediatly!!!
```

_A To Do (**TODO**) shown in `turtle`_.

#### Agents

> TODO@JLA: it's your job!

---

## TLDR

Too Long, Didn't Read!

### Example

#### turtle

```turtle
## TLDR: A very, very long story (very boring, indeed!).
```

_Example in `turtle`_.

---

#### markdown

```markdown
## TLDR

A very, very long story (very boring, indeed.
 And it gets **NOT** better written in `markdown`!!!).

---
```

_Example in m`markdown`_.

---

## TRACL

---