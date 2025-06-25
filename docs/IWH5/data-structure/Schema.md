# JSON Schema

The JSON Schema defines the strcuture of the data structure json in the `.iwh5` file. It describes the data subset structure information. The schema has four top-level fields: `version`, `name`, `commonAxes`, and `subsets`. 

The commonAxes array specifies shared coordinate axes with parameters including points (sample count), start (origin offset), resolution (sampling interval), type (axis role), and units (measurement units, e.g., millimeters).

The subsets array contains multiple data groups, each defined by a name and optionally its own local axes array specifying axis properties similar to commonAxes. Each subset includes an element array detailing measured parameters with attributes such as displayMin and displayMax for visualization bounds, offset and scale for data transformation, units, and an optional type field indicating the data type.

The reservedLevels array within each element defines enumerated special values with associated numeric levels and labels (e.g., "undefined"). This structure supports hierarchical, extensible representation of datasets used commonly in ultrasound (UT) and eddy current (ET) NDE data.

??? info "View Schema as JSON"
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

# Samples
The data structure JSON samples conforms to version 1.0.0 of the schema and encapsulates multidimensional data.

??? info "View UT data_structure JSON"
    ```json
    {
      "commonAxes": [
        {
          "points": 108,
          "resolution": 0.75,
          "start": -0.375,
          "type": "Scan Axis",
          "units": "mm"
        },
        {
          "points": 201,
          "resolution": 0.75,
          "start": -0.375,
          "type": "Index Axis",
          "units": "mm"
        }
      ],
      "name": "Root Data",
      "subsets": [
        {
          "axes": [
            {
              "points": 169,
              "resolution": 0.05,
              "start": 25.332111772789702,
              "type": "Data Axis",
              "units": "us"
            }
          ],
          "element": [
            {
              "displayMax": 100.0,
              "displayMin": 0.0,
              "offset": 0.0,
              "reservedLevels": [
                {
                  "level": 255,
                  "name": "undefined"
                }
              ],
              "scale": 0.393700787401575,
              "units": "%"
            }
          ],
          "name": "Linear Sweep Ch A"
        },
        {
          "element": [
            {
              "displayMax": 100.0,
              "displayMin": 0.0,
              "offset": 0.0,
              "reservedLevels": [
                {
                  "level": 255,
                  "name": "undefined"
                }
              ],
              "scale": 0.393700787401575,
              "units": "%"
            }
          ],
          "name": "Linear Sweep Ch A IF Amp"
        },
        {
          "element": [
            {
              "displayMax": 29.7321117727897,
              "displayMin": 26.332111772789702,
              "reservedLevels": [
                {
                  "level": 987987,
                  "name": "undefined"
                }
              ],
              "type": "Float",
              "units": "us"
            }
          ],
          "name": "Linear Sweep Ch A IF TOF"
        },
        {
          "element": [
            {
              "displayMax": 100.0,
              "displayMin": 0.0,
              "offset": 0.0,
              "reservedLevels": [
                {
                  "level": 255,
                  "name": "undefined"
                }
              ],
              "scale": 0.393700787401575,
              "units": "%"
            }
          ],
          "name": "Linear Sweep Ch A Gate 1 Amp"
        },
        {
          "element": [
            {
              "displayMax": 3.48211177278974,
              "displayMin": 0.932111772789739,
              "reservedLevels": [
                {
                  "level": 987987,
                  "name": "undefined"
                }
              ],
              "type": "Float",
              "units": "us"
            }
          ],
          "name": "Linear Sweep Ch A Gate 1 TOF"
        }
      ],
      "version": "1.0.0"
    }
    ```
??? info "View ET data_structure JSON"
    ```json
    {
      "commonAxes": [
        {
          "points": 61,
          "resolution": 0.5625,
          "start": 0.0,
          "type": "Scan Axis",
          "units": "mm"
        }
      ],
      "name": "Root Data",
      "subsets": [
        {
          "axes": [
            {
              "points": 1815,
              "resolution": 0.25,
              "start": 0.0,
              "type": "Sweep Axis",
              "units": "mm"
            }
          ],
          "element": [
            {
              "displayMax": 10.0,
              "displayMin": -10.0,
              "offset": 0.0,
              "reservedLevels": [
                {
                  "level": -32768,
                  "name": "undefined"
                }
              ],
              "scale": 0.00030518509475997203,
              "type": "Int16",
              "units": "V"
            }
          ],
          "elementFormat": "complex",
          "name": "Axial"
        },
        {
          "axes": [
            {
              "points": 1815,
              "resolution": 0.25,
              "start": 0.0,
              "type": "Sweep Axis",
              "units": "mm"
            }
          ],
          "element": [
            {
              "displayMax": 10.0,
              "displayMin": -10.0,
              "offset": 0.0,
              "reservedLevels": [
                {
                  "level": -32768,
                  "name": "undefined"
                }
              ],
              "scale": 0.00030518509475997203,
              "type": "Int16",
              "units": "V"
            }
          ],
          "elementFormat": "complex",
          "name": "Trans"
        }
      ],
      "version": "1.0.0"
    }
    ```
