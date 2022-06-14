# Understanding "Data and Information"

## Classification of Data

Following classifications of [data](../../glossary/README.md#data): [`Meta Data`](#meta-data)
, [`Infrastructure Data`](#infrastructure-data) and
[`Payload Data`](#payload-data) are explaind as follows.

### Meta Data

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

...etc. On the other hand it is aligned to well known application protocols, like 'http'.

```http request
GET 

```

```#meta-data```

---

### Infrastructure Data

All [data](../../glossary/README.md#data) used and provided by _Eco System_ relevant Infrastructure Services.

```#infrastructure-data```

---

### Payload Data

```#payload-data```

---