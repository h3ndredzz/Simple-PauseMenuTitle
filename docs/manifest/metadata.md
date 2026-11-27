## `metadata`

optional for creditals, uh licenses and tools

* **`authors`** (`string[]`), creators of the pack. required using `format_version: 3`
* **`license`** (`string`), distrubition license (such as `"MIT"` or `"All Rights Reserved"`)
* **`url`** (`string`), any existing url, usually credit pages like github
* **`product_type`** (`string`), context flag, only `"addon"` is valid
* **`generated_with`** (`object`), tool names `[google-ai]`, max 32 characters

```json
"metadata": {
  "authors": ["Alex", "Steve"],
  "license": "MIT",
  "url": "https://github.com",
  "product_type": "addon",
  "generated_with": {
    "blockbench": ["4.10.0"]
  }
}
```
