# Data

The following classifications of data: [`Meta Data`](#meta-data), [`Infrastructure Data`](#infrastructure-data) and
 [`Payload Data`](#payload-data).

## Meta Data

Even `Payload Data` will reflect some portions of meta data, like any timestamping of given values,

Example:

```json
{
    'rdf:type': "xsd:nonNegativeInteger",
    'rdf:value': "43",
    'fua:timestamp': {
        '@type': "xsd:dateTimeStamp",
        '@value': ""
    }
}
```

...etc. On the other
 hand it is aligned to well known application protocols, like 'http', 'WebSockets', etc.  

## Infrastructure Data

All Data used and provided by Eco System relevant Infrastructure Services.

## Payload Data

---
