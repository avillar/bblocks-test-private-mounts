
# My Schema (Schema)

`ogc.avillar.tests.mounts.mySchema` *v0.1*

An example schema defining the set of properties of any type of object.

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Example 1
#### json
```json
{
  "avillar": {
    "fake": "test"
  }
}
```

#### jsonld
```jsonld
{
  "@context": "https://avillar.github.io/bblocks-test-private-mounts/build/annotated/avillar/tests/mounts/mySchema/context.jsonld",
  "avillar": {
    "fake": "test"
  }
}
```

#### ttl
```ttl
@prefix ns1: <https://example.com/> .
@prefix ns2: <https://example.net/> .

[] ns2:avillar [ ns1:fake "test" ] .


```

## Schema

```yaml
$schema: https://json-schema.org/draft/2020-12/schema
description: My example schema
type: object
properties:
  avillar:
    $ref: https://avillar.github.io/ogcapi-sosa/build/annotated/sosa/properties/avillar/schema.yaml
    x-jsonld-id: https://example.net/avillar

```

Links to the schema:

* YAML version: [schema.yaml](https://avillar.github.io/bblocks-test-private-mounts/build/annotated/avillar/tests/mounts/mySchema/schema.json)
* JSON version: [schema.json](https://avillar.github.io/bblocks-test-private-mounts/build/annotated/avillar/tests/mounts/mySchema/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "avillar": {
      "@context": {
        "fake": "https://example.com/fake"
      },
      "@id": "https://example.net/avillar"
    },
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](https://avillar.github.io/bblocks-test-private-mounts/build/annotated/avillar/tests/mounts/mySchema/context.jsonld)

## Sources

* [Sample source document](https://example.com/sources/1)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/avillar/bblocks-test-private-mounts](https://github.com/avillar/bblocks-test-private-mounts)
* Path: `_sources/mySchema`

