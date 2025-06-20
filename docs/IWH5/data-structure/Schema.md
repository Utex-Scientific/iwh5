# JSON Schema Documentation

## Schema
- **$schema**: [https://json-schema.org/draft/2020-12/schema](https://json-schema.org/draft/2020-12/schema)

??? info "View Schema JSON"
    ```json
      {
      "$schema": "https://json-schema.org/draft/2020-12/schema",
      "type": "object",
      "properties": {
        "version": {
          "type": "string"
        },
        "name": {
          "type": "string"
        },
        "commonAxes": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "points": {
                "type": "number"
              },
              "start": {
                "type": "number"
              },
              "resolution": {
                "type": "number"
              },
              "units": {
                "type": "string"
              },
              "type": {
                "type": "string"
              }
            },
            "required": [
              "points",
              "start",
              "resolution",
              "units",
              "type"
            ]
          }
        },
        "subsets": {
          "type": "array",
          "items": {
            "type": "object",
            "properties": {
              "name": {
                "type": "string"
              },
              "element": {
                "type": "array",
                "items": {
                  "type": "object",
                  "properties": {
                    "units": {
                      "type": "string"
                    },
                    "displayMin": {
                      "type": "number"
                    },
                    "displayMax": {
                      "type": "number"
                    },
                    "type": {
                      "type": "string"
                    },
                    "reservedLevels": {
                      "type": "array",
                      "items": {
                        "type": "object",
                        "properties": {
                          "name": {
                            "type": "string"
                          },
                          "level": {
                            "type": "number"
                          }
                        },
                        "required": [
                          "name",
                          "level"
                        ]
                      }
                    }
                  },
                  "required": [
                    "units",
                    "displayMin",
                    "displayMax",
                    "type",
                    "reservedLevels"
                  ]
                }
              },
              "flags": {
                "type": "array",
                "items": {
                  "type": "string"
                }
              }
            },
            "required": [
              "name",
              "element",
              "flags"
            ]
          }
        }
      },
      "required": [
        "version",
        "name",
        "commonAxes",
        "subsets"
      ]
    }
    ```
## Root Object

### Type: `object`

### Required Properties:
- `version` (string)
- `name` (string)
- `commonAxes` (array of objects)
- `subsets` (array of objects)

---

## Properties

### `version`
- **Type**: `string`

### `name`
- **Type**: `string`

### `commonAxes`
- **Type**: `array` of objects  
Each object contains:
  - `points`: number (required)
  - `start`: number (required)
  - `resolution`: number (required)
  - `units`: string (required)
  - `type`: string (required)

### `subsets`
- **Type**: `array` of objects  
Each object contains:

#### `name`
- **Type**: `string`

#### `element`
- **Type**: `array` of objects  
Each object contains:
  - `units`: string (required)
  - `displayMin`: number (required)
  - `displayMax`: number (required)
  - `type`: string (required)
  - `reservedLevels`: array of objects  
    Each object contains:
    - `name`: string (required)
    - `level`: number (required)

#### `flags`
- **Type**: `array` of strings
