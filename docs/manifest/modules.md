## `modules`

required, tells minecraft what contents the pack holds. Resource packs need at least one object with `"type"` set to `"resources"`

* **`type`** (`string`, required), must be `"resources"` for texture/resource packs
* **`uuid`** (`string`, required), unique UUIDv4 for this module. Must be different from `header.uuid`
* **`version`** (`int`, required) — `[major, minor, patch]`. Keep this synced with `header.version`
* **`description`** (`string`, optional),  Internal note describing the module.

```json
"modules": [
  {
    "type": "resources",
    "uuid": "11111111-1111-1111-1111-111111111111",
    "version":[1, 0, 0],
    "description": "mhm this is a resource pack for sure"
  }
]
```
