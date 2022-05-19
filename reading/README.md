# Reading [`fua`](../README.md)

Reading the given documentation of [`fua`](../README.md) follows the explanations:

## Signify the Requirements

Those words, like **MUST**, **MUST NOT**, **REQUIRED**, **SHALL**, **SHALL NOT**, **SHOULD**, **SHOULD NOT**,
**RECOMMENDED**,  **MAY**, and **OPTIONAL**, used in `fua` documentation, examples, code-fragments and there very
meaning are the explained [here, RFC2119](https://datatracker.ietf.org/doc/html/rfc2119).

---

## Pseudocode

`fua` revealed in this repository is pure ontology. But sometimes it helps to understand the path to its implementation
and exposed services, the "layer of usage". The pseudocode is shown in a programming language, that doesn't exist and is
assembled from all those programming languages hitting the matter best: what is going on?

### Example:

_If `43` is larger than `42`, than execute function `getit()` and put its result in `that`._

```pseudocode
if (43 > 42) {
    that = getit();
}
```

---

## json

The "JavaScript Object Notation", `json` do **NOT** allow comments, like `//` used by JavaScript itself. But
given documentation of `fua` uses this to characters `//` to express inline comments.

### Example:

_That artefact shown here and expressed in `json`, is the result of given function `getit()` and contains a comment
tagged as en remark (`REM`)_

```json
{
    "@context": [
        "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
        "https://www.nicos-rd.com/fua#"
    ],
    "@type":        "fua:ThatResult",
    // REM : it seems to be a constant result!
    "rdf:value":    "Hey dude, do you really think that <43> can be greater than <42> at some time or another?!?" 
}
```

---
