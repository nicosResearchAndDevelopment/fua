# Decide ODRL Profile "ftime"

- preferred namespace prefix `ftime`.

The following is the starting point to understand how `fua` brings some aspects of time related questions into
constraints (under rules, under policies).

- [Time Ontology in OWL](https://www.w3.org/TR/owl-time/).

```text
                      |     i     |        j
  Before(i, j)        |<.........>|   <--------->    After(j, i)
   Meets(i, j)        |           |<------------>    MetBy(j, i)
Overlaps(i, j)        |       <---|------------->    OverlappedBy(j, i)
  Starts(i, j)        |<----------|------------->    StartedBy(j, i)
  During(i, j)    <---|-----------|------------->    Contains(j, i)
Finishes(i, j)    <---|---------->|                  FinishedBy(j, i)
  Equals(i, j)        |<--------->|                  Equals(j, i)
```

*Thirteen elementary possible relations between time periods*.

> ["Actions and events in interval temporal logic In: Spatial and
Temporal Reasoning. O. Stock, ed., Kluwer, Dordrecht, Netherlands,
pp. 205-245.. J.F. Allen; G. Ferguson.1997."](http://dx.doi.org/10.1007/978-0-585-28322-7_7)

Two additional relations, `In` and `Disjoint`:

```pseudocode
      In(i, j) === (Starts(i, j) || During(i, j) || Finishes(i, j))
Disjoint(i, j) === (Before(i, j) || After(i, j))
```

## Convention to read Pseudocode Parameters

### Temporal Entity

Points in time and time intervals are temporal entities. A temporal entity
has a beginning and an end. For points in time beginning and end is the same.

### A Time Instant

So, it is a point in time and expressed in `xsd:dateTimeStamp`:

```text
"2019-04-01T00:00:00Z"
```

### Durations

Durations are expressed in [xsd:duration](https://www.w3.org/TR/xmlschema-2/#duration).

### Intervals

Intervals can be expressed in three different ways:

- time instant, time instant
- time instant, duration
- duration, time instant

Intervals are represented in given pseudocode as an array of two strings.

The following example expresses the identical interval (with
duration of one day) in three ways:

```text
[ "2019-04-01T00:00:00Z", "2019-04-02T00:00:00Z" ]
[ "2019-04-01T00:00:00Z", "P1D" ]
[ "P1D",                  "2019-04-02T00:00:00Z" ]
```

### An Interval

A period of time (here: one day)

```text
[ "2019-04-01T00:00:00Z", "2019-04-02T00:00:00Z" ]
```

The beginning of an interval **MUST** be placed before or equal to the end of it.

A period of time (here: 0 seconds)

```text
[ "2019-04-01T00:00:00Z", "2019-04-01T00:00:00Z" ]
```

### A Proper Interval

A period of time (here: one day)

```text
[ "2019-04-01T00:00:00Z", "2019-05-01T00:00:00Z" ]
```

The beginning of a proper interval **MUST** be placed before the end of it. So it can **NOT** take `0 seconds`!!!

---

## Binary Operators

### ftime:before

###### Example

A `time:Instant` is `ftime:before` a `time:Interval`.

###### pseudocode

```pseudocode
Before( "2019-01-05T00:00:00Z", [ "2019-02-01T00:00:00Z", "2019-03-01T00:00:00Z"]) ===== true
```

###### ODRL

```json
{
  "@context": [
    "http://www.w3.org/ns/odrl.jsonld",
      {
        "odrl": "http://www.w3.org/ns/odrl.jsonld",
        "time": "http://www.w3.org/2006/time#"
      }
    ],
    "constraint": [{
               "leftOperand": {
                    "@type": "time:Instant",
                    "time:hasBeginning": {
                        "@type": "time:Instant",
                        "time:inXSDDateTimeStamp": {
                            "@type": "xsd:dateTimeStamp",
                            "@value": "2019-01-05T00:00:00Z"
                        }
                    }
               },
               "operator": "ftime:before",
               "rightOperand":  {
                    "@type": "time:Interval",
                    "time:hasBeginning": {
                        "@type": "time:Instant",
                        "time:inXSDDateTimeStamp": {
                            "@type": "xsd:dateTimeStamp",
                            "@value": "2019-02-01T00:00:00Z"
                        }
                    },
                    "time:hasEnd": {
                        "@type": "time:Instant",
                        "time:inXSDDateTimeStamp": {
                            "@type": "xsd:dateTimeStamp",
                            "@value": "2019-03-01T00:00:00Z"
                        }
                    }
               }
           }]
}
```

---

### ftime:after

###### Example

A `time:Instant` is `ftime:after` a `time:Interval`.

###### pseudocode

```pseudocode
After( "2019-04-01T00:00:00Z", [ "2019-02-01T00:00:00Z", "2019-03-01T00:00:00Z" ]) === true
```

| time:TemporalEntity  |               | time:TemporalEntity               | is    |
|:---|---------------|:----------------------------------|:------|
| "2019-04-01T00:00:00Z" | `ftime:after` | [ "2019-02-01T00:00:00Z", "P1M" ] | true  |

### ftime:Meets

###### Example

A `time:Interval` `meets` a `time:Interval`.

###### pseudocode

```pseudocode
Meets( [ "2019-01-01T00:00:00Z", "2019-02-01T00:00:00Z" ], [ "2019-02-01T00:00:00Z", "2019-03-01T00:00:00Z" ]) === true
```

### ftime:MetBy

###### Example

A `time:Interval` is `ftime:metBy` a `time:Interval`.

###### pseudocode

```pseudocode
MetBy( [ "2019-02-01T00:00:00Z", "2019-03-01T00:00:00Z" ], [ "2019-01-01T00:00:00Z", "2019-02-01T00:00:00Z" ]) === true
```

### ftime:overlaps

###### Example

A `time:Interval` `ftime:overlaps` a `time:Interval`.

###### pseudocode

```pseudocode
Overlaps( [ "2019-01-01T00:00:00Z", "2019-03-01T00:00:00Z" ], [ "2019-02-01T00:00:00Z", "2019-04-01T00:00:00Z" ]) === true
```

### ftime:overlappedBy

###### Example

A `time:Interval` is `ftime:overlappedBy` a `time:Interval`.

###### pseudocode

```pseudocode
Overlaps([ "2019-02-01T00:00:00Z", "2019-04-01T00:00:00Z" ], [ "2019-01-01T00:00:00Z", "2019-03-01T00:00:00Z" ]) === true
```

### ftime:starts

###### Example

A `time:Instant` `ftime:starts` a `time:Interval`.

###### pseudocode

```pseudocode
Starts( "2019-01-01T00:00:00Z", [ "2019-01-01T00:00:00Z", "2019-02-01T00:00:00Z" ]) === true
```

### ftime:startedBy

###### Example

A `time:Interval` is `ftime:startedBy` a `time:Instant`.

###### pseudocode

```pseudocode
Starts([ "2019-01-01T00:00:00Z", "2019-02-01T00:00:00Z" ], "2019-01-01T00:00:00Z" ) === true
```

### ftime:during

###### Example

A `time:Interval` is `ftime:during` a `time:Interval`.

###### pseudocode

```pseudocode
During( [ "2019-02-01T00:00:00Z", "2019-03-01T00:00:00Z" ], [ "2019-01-01T00:00:00Z", "2019-04-01T00:00:00Z" ] ) === true
```

### ftime:contains

###### Example

A `time:Interval` `fcontains` a `time:Instant`.

###### pseudocode

```pseudocode
Contains( [ "2019-01-01T00:00:00Z", "2019-03-01T00:00:00Z" ], "2019-02-01T00:00:00Z" ) === true
```

### ftime:finishes

###### Example

A `time:Instant` `ftime:finishes` a `time:Interval`.

###### pseudocode

```pseudocode
Finishes( "2019-02-01T00:00:00Z", [ "2019-01-01T00:00:00Z", "2019-02-01T00:00:00Z" ]) === true
```

### ftime:finishedBy

###### Example

A `time:Interval` is `ftime:finishedBy` a `time:Instant`.

###### pseudocode

```pseudocode
Finishes([ "2019-01-01T00:00:00Z", "2019-02-01T00:00:00Z" ], "2019-02-01T00:00:00Z" ) === true
```

### ftime:equals

##### Example

A `time:Instant` `ftime:equals` a `time:Instant`.

###### pseudocode

```pseudocode
Equals("2019-04-01T00:00:00Z", "2019-04-01T00:00:00Z") === true
```

| time:TemporalEntity  |   | time:TemporalEntity | is |  
|:---|---|:---|:---|
| "2019-04-01T00:00:00Z" | `Equals`     | "2019-04-01T00:00:00Z" | true   |

### ftime:in

###### Example

A `time:Interval` is `ftime:in` a `time:Interval`.

###### pseudocode

```pseudocode
Finishes( [ "2019-01-01T00:00:00Z", "2019-02-01T00:00:00Z" ], [ "2019-01-01T00:00:00Z", "2019-03-01T00:00:00Z" ]) === true
```

### ftime:disjoint

###### Example

A `time:Interval` is `ftime:disjoint` with a `time:Interval`.

###### pseudocode

```pseudocode
Finishes( [ "2019-01-01T00:00:00Z", "2019-02-01T00:00:00Z" ], [ "2019-03-01T00:00:00Z", "2019-04-01T00:00:00Z" ]) === true
```

---

```#ftime, #time, #control-language, #control```

---
