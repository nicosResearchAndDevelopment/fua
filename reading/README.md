# Reading `fua`

Reading the given documentation of [`fua`](../README.md) follows the explanations:

## Signify the Requirements

Those words, like **MUST**, **MUST NOT**, **REQUIRED**, **SHALL**, **SHALL NOT**, **SHOULD**, **SHOULD NOT**,
**RECOMMENDED**,  **MAY**, and **OPTIONAL**, used in `fua` documentation, examples, code-fragments and there very
meaning are the explained [here, RFC2119](https://datatracker.ietf.org/doc/html/rfc2119).

---

## Pseudocode

`fua` revealed in this repository is pure ontology. But sometimes it helps to understand the path to its implementation
and exposed [services](../glossary/README.md#service), the "layer of usage". The pseudocode is shown in a programming
language, that doesn't exist and is assembled from all those programming languages hitting the matter
best: ([IA](../glossary/README.md#ia)) "What is going on here?".

### Example "43>42"

[IA](../glossary/README.md#ia) : "Is '43' larger than '42' and if "YES" get it and put it to 'that'".

```pseudocode
if (43 > 42) {
    that = getit();
}
```

[IA](../glossary/README.md#ia) : _If `43` is larger than `42`, than execute function `getit()` and put its result
in `that`_.

---

## JSON

The "JavaScript Object Notation", (**JSON**) do **NOT** allow inline comments {`//`} (like used by JavaScript itself).
But given documentation of `fua` uses this two characters `//` to express inline comments this way for easier
understanding, what it's all about...

### Example "illicit comment in JSON"

Using _illicit_ comment `//` in **JSON**.

```json
{
    "@context": [
        "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
        "https://www.nicos-rd.com/fua#"
    ],
    "@type":        "fua:ThatResult",
    // REM : it seems to be a constant result!
    "rdf:value":    "Hey dude!!! Do you really think that <43> can be greater than <42> at some time or another?!?" 
}
```

_That artefact shown here and expressed in **JSON**, is the result of given function [`getit()`](#example-4342) and
contains a malicious inline comment, tagged as a remark (`REM`)_.

## Tags

`fua` uses [tags](../glossary/README.md#tag) (down to code) for one reason: to foster [traceability](#traceability)
of related concepts, descriptions or _mentions_.

### Example

#### in markdown

This is often shown in `fuas` [glossary](../glossary/README.md) (focused on `#linked-data`):

```markdown
```#linked-data, #infrastructure-data, #infrastructure-layer, #layer```
```

#### in turtle

```turtle
### #linked-data, #infrastructure-data, #infrastructure-layer, #layer ###
```

#### in json

[Keep in mind!](#example-illicit-comment-in-json)

```json
/// #linked-data, #infrastructure-data, #infrastructure-layer, #layer ///
```

### Traceability

Take your **IDE**, clone `fua` and search for [`#linked-data`](../glossary/README.md#linked-data). While `fua` keeps
track
of focused use of a tag you will find the most relevant [information](../glossary/README.md#information) regarding
given topic.

Mostly the tags are _weighted_, means: if a topic is decorated with tags, the most relevant is in front followed by
less "important" ones (ordered, descending). And they are used to point (mostly) to a glossary-entry

```text
[#linked-data](../glossary/README.md#linked-data)
```

_...this leads to [#linked-data](../glossary/README.md#linked-data)_.

Hope that helps!

---

---

## Glossary

`fuas` [glossary](../glossary/README.md) is a good starting point itself, showing all those _well known_
buzz-words and how `fua` assimilates and paraphrases them.

The [glossary](../glossary/README.md) is something like a Gate Keeper (for `fuas` terminology) and not at least
as an _eye of a needle_: incoming links **SHOULD** land [here](../glossary/README.md#glossary) (**RECOMMENDED**).

---
