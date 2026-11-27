## `header`

required, defines the pack's name, ID, version, and engine compatibility

* **`name`** (`string`, required), display name shown in the pack menu
* **`description`** (`string`, required), summary shown under the pack name in-game
* **`uuid`** (`string`, required), unique UUIDv4 for the pack. Must be unique across all packs and different from `modules[].uuid`
* **`version`** (`int[3]`, required), `[major, minor, patch]`. Bump this on updates so Minecraft registers the changes.
* **`min_engine_version`** (`int[3]`, required), `[major, minor, patch]` of the oldest Minecraft version the pack supports
* **`pack_scope`** (`string`, optional), Controls where the pack can be used: `"any"` (default), `"global"`, or `"world"`

```json
"header": {
  "name": "pack.name",
  "description": "pack.description",
  "uuid": "00000000-0000-0000-0000-000000000000",
  "version":[1, 0, 0],
  "min_engine_version":,
  "pack_scope": "any"
}
```
