# Understanding [`fua`](../README.md)

Some thoughts on **fua**-underlying concepts and interpretations.

## Internal View

[`fua`](../README.md) - as presented here - aims the _internal_ view on expressing data and its structure,
implementing solutions, done by nicos Research & Development (nrd), based on
[GAIAboX (gbx)](https://github.com/nicosResearchAndDevelopment/gbx/README.md) and brought to service by.

## The Mechanics

Understanding it this way, service users (consumers) do **NOT** have to implement **fua**!
Reading the docs here, means to get a deeper understanding of _the mechanics_ and offers
(and that seems to be the most significant impact) and to foster creativity of those intended
to work with given concepts.

## The Presentation Layer is Somewhere Else

**fua** does **NOT** express information offered on the Presentation Layer, the information of interest send to given
data-consumer. The Presentation Layer is _seated_ somewhere else: [gbx](https://github.com/nicosResearchAndDevelopment/gbx/README.md) - whatever **THE** presentation looks like...

## Do **NOT** Cover

**fua** aims **NOT** to cover well know concepts, ontologies and schemas, like (in alphabetical order):

- [dct (DCMI Metadata Terms)](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/)
- [foaf (Friend Of A Friend)](http://xmlns.com/foaf/spec/)
- [odrl (ODRL Information Model 2.2)](https://www.w3.org/TR/odrl-model/)
- [org (The Organization Ontology)](https://www.w3.org/TR/vocab-org/)
- [prov (PROV Model Primer)](https://www.w3.org/TR/prov-primer/)
- [skos (SKOS Simple Knowledge Organization System)](https://www.w3.org/TR/skos-reference/)
- [time (Time Ontology in OWL)](https://www.w3.org/TR/owl-time/)
- [vc (Verifiable Credentials Data Model v1.1)](https://www.w3.org/TR/vc-data-model/)
- [xsd (W3C XML Schema Definition Language (XSD) 1.1 Part 2: Datatypes)](https://www.w3.org/TR/xmlschema11-2/)

...to list some of those **fua** has a strong relation to.

## turtle and Linked Data

**fua** shows itself and its examples, all its citations (mostly) in [turtle](https://www.w3.org/TR/turtle/). For some
readers this seems _natural_. For others not. A lot of us don't like this turtle-stuff. For this reason (?!?) there are
some concepts (like [odrl](https://www.w3.org/TR/odrl-model/) or [vc](https://www.w3.org/TR/vc-data-model/)) in
the field showing there topics in [JSON-LD](https://www.w3.org/TR/json-ld11/). "LD" = [Linked Data](https://en.wikipedia.org/wiki/Linked_data).
Some of us are feeling more comfortable with JSON-LD, because it looks like [_JSON_](https://en.wikipedia.org/wiki/JSON)
("Yes", JSON-LD **is** JSON!!!) and **fua** itself will present some concepts in JSON-LD (see [fua "Decide Pofiles"](../decide/profile/README.md), these are on top on odrl and so it seems to be "natural" to do so...), also - and/or in turtle. But **fua** focusses on turtle and it is worth to learn it reading. Authors of **fua** thought that it is the
better way...

## Dirty Hands

To get hands dirty, **fua** works with [examples](../èxample/README.md) to get in touch with
_"aha" moments_ - at best. And to strength the intention of being the _solution_ and **NOT** the _problem_...

- [Weather Station](../èxample/weatherstation/README.md)
- [Elevator](../èxample/elevator/README.md)
- [The Universe Dataverse](../èxample/dataverseuni/README.md)

Sometimes some of those scopes look a little nerdy, but they only demonstrate and explain
underlying concepts of **fua** - and try to trigger creativity of kind reader. 

## You are Welcome

So, if someone is interested in implementing its own solutions using **fua** - you're welcome! For all others it will
(hopefully) be a manual to explore the potentials.

---