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
  "name": "cool pack",
  "description": "this pack has chicken butt",
  "uuid": "00000000-0000-0000-0000-000000000000",
  "version":[1, 0, 0],
  "min_engine_version":[1, 26, 65],
  "pack_scope": "any"
}
```
I personally just put the min engine to the latest version. v26.25
version is just so minecraft can tell if you updated your pack's code or version 
so if you changed it to [1, 1, 0] this is the 10th version of your addon