# Probe Config

See the [Legend](#legend) for symbol definitions.

---

??? info "General"

    | IW Property Name       | IW Scan Name                | Property Type | Data Type       | Options                                                                | Units | Example           | Comments       |
    |-----------------------|-----------------------------|---------------|-----------------|------------------------------------------------------------------------|-------|-------------------|----------------|
    | Name                  |                             | *             | String          |                                                                        |       | Conventional UT   |                |
    | Probe Type            |                             | A             | String          |                                                                        |       | Conventional      |                |
    | Scanning Direction    |                             | *             | List of strings | Length,Width                                                           |       |                   |                |
    | Probe Orientation     | Orientation                 | *             | List of strings | Index Forward, Index Backward,Scan Forward,Scan Backward               |       |                   |                |
    | Surface               |                             | *             | List of strings | X Positive, X Negative, Y Positive, Y Negative, Z Positive, Z Negative |       |                   |                |
    | Scan Offset           |                             | *             | Double          |                                                                        | mm    |                   |                |
    | Index Offset          |                             | *             | Double          |                                                                        | mm    |                   |                |
    | Interface Type        |                             | *             | List of strings | Contact,Wedge,Immersion                                                |       |                   |                |
    | Frequency             |                             | *             | Double          |                                                                        |       |                   |                |
    | Bandwidth             |                             | *             | Double          |                                                                        |       |                   |                |
    | Instrument Channel    | Channel For First Element    | *             | Integer         |                                                                        |       |                   |                |
    | Device Index          |                             | *             | Integer         |                                                                        |       |                   |                |

---

??? info "Linear Array"

    | IW Property Name         | IW Scan Name              | Property Type | Data Type       | Options                              | Units | Example | Comments |
    |-------------------------|---------------------------|---------------|-----------------|------------------------------------|-------|---------|----------|
    | Manufacturer            |                           | O             | String          |                                    |       |         |          |
    | Transducer Part Number  |                           | O             | String          |                                    |       |         |          |
    | Transducer Serial Number|                           | O             | String          |                                    |       |         |          |
    | Number Of Elements X    | Number Of Elements         | *             | Integer         |                                    |       |         |          |
    | Element Pitch X         | Pitch                     | *             | Double          |                                    | mm    |         |          |
    | Element Width X         | Width                     | *             | Double          |                                    | mm    |         |          |
    | Element Width Y         | Elevation                 | *             | Double          |                                    | mm    |         |          |
    | Focusing Type           | Type                      | *             | List of strings | Unfocused,Cylindrical In X,Cylindrical In Y |       |         |          |
    | Element Map             | Element Mapping           | *             | List of strings | Normal,Reversed                    |       |         |          |

---

??? info "Conventional"

    | IW Property Name     | IW Scan Name | Property Type | Data Type       | Options                     | Units | Example | Comments       |
    |---------------------|--------------|---------------|-----------------|-----------------------------|-------|---------|----------------|
    | Focusing Type       | Type         | *             | List of strings | Unfocused,Focused            |       |         |                |
    | Element Shape       | Shape        | *             | List of strings | Circle,Ellipse,Rectangle     |       |         |                |
    | Element Diameter    |              | *             | Double          |                             | mm    |         |                |
    | Length              |              | D             | Double          |                             | mm    |         | Based on shape |
    | Focal Length        |              | *             | Double          |                             |       |         |                |
    | Inspection Mode     |              | *             | List of strings | Longitudinal,Shear           |       |         |                |

---

??? info "Coupling"

    | IW Property Name             | IW Scan Name | Property Type | Data Type | Options | Units | Example | Comments |
    |-----------------------------|--------------|---------------|-----------|---------|-------|---------|----------|

---

??? info "Immersion"

    | IW Property Name          | IW Scan Name | Property Type | Data Type | Options | Units | Example | Comments |
    |--------------------------|--------------|---------------|-----------|---------|-------|---------|----------|
    | Beam Angle in Couplant   | Angle        | *             | Double    |         | deg   |         |          |
    | Path In Couplant        | Path         | *             | Double    |         | mm    |         |          |
    | Couplant Material       | Material     | *             | String    |         |       | Water   |          |
    | Couplant Velocity of Sound | Speed of Sound | *          | Double    |         | mm/us |         |          |

---

??? info "Wedge (Linear Array)"

    | IW Property Name          | IW Scan Name                 | Property Type | Data Type | Options | Units | Example | Comments |
    |--------------------------|------------------------------|---------------|-----------|---------|-------|---------|----------|
    | Wedge Part Number         | Part Number                  | O             | String    |         |       |         |          |
    | Wedge Serial Number       | Serial Number                | O             | String    |         |       |         |          |
    | Manufacturer             |                              | O             | String    |         |       |         |          |
    | Wedge Angle              | Angle                        | *             | Double    |         | deg   |         |          |
    | Wedge Roof Angle         | Roof Angle                   | *             | Double    |         | deg   |         |          |
    | Height At First Element  |                              | *             | Double    |         | mm    |         |          |
    | Length To First Element  | First Element From Front Face | *            | Double    |         | mm    |         |          |
    | Length After First Element | First Element From Back Face | *            | Double    |         | mm    |         |          |
    | Wedge Length             | Length                       | *             | Double    |         | mm    |         |          |
    | Wedge Height             | Height                       | *             | Double    |         | mm    |         |          |
    | Wedge Width              | Width                        | *             | Double    |         | mm    |         |          |
    | Damping Groove Depth     |                              | *             | Double    |         | mm    |         |          |
    | Material                 |                              | *             | String    |         |       | Plexiglass |        |
    | Longitudinal Velocity    |                              | *             | Double    |         | mm    |         |          |

---

??? info "Wedge (Conventional)"

    | IW Property Name          | IW Scan Name                 | Property Type | Data Type | Options | Units | Example | Comments |
    |--------------------------|------------------------------|---------------|-----------|---------|-------|---------|----------|
    | Wedge Part Number         | Part Number                  | O             | String    |         |       |         |          |
    | Wedge Serial Number       | Serial Number                | O             | String    |         |       |         |          |
    | Manufacturer             |                              | O             | String    |         |       |         |          |
    | Wedge Angle              | Angle                        | *             | Double    |         | deg   |         |          |
    | Wedge Roof Angle         | Roof Angle                   | *             | Double    |         | deg   |         |          |
    | Wedge Back Height        | Back Height                  | *             | Double    |         |       |         |          |
    | Wedge Exit Point         | Exit Point                   | *             | Double    |         |       |         |          |
    | Wedge Length             | Length                       | *             | Double    |         | mm    |         |          |
    | Wedge Height             | Height                       | *             | Double    |         | mm    |         |          |
    | Wedge Width              | Width                        | *             | Double    |         | mm    |         |          |
    | Damping Groove Depth     |                              | *             | Double    |         | mm    |         |          |
    | Material                 |                              | *             | String    |         |       |         |          |
    | Longitudinal Velocity    |                              | *             | Double    |         | mm    |         |          |

---

## Legend

| Symbol | Meaning         |
|--------|------------------|
| *      | Required         |
| O      | Optional         |
| A      | Auto Calculated  |
| D      | Dependent        |
