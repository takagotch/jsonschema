### jsonschema
---
https://github.com/Julian/jsonschema

```py
from jsonschema import validate
schema = {
  "type": "object",
  "properties": {
    "properties": {
      "price" : {"type": "number"},
      "name" : {"type": "string"},
    },
  }
}

validate(instance={"name": "Eggs", "price": 34.99}, schema=schema)
validate(
  instance={"name" : "Eggs", "price" : "Invalid"}, schema=schema,
)

```

```sh
jsonschema -i sample.json sample.schema
pip install jsonschema
```

```
```


