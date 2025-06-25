# Scan

_See the [Legend](#legend) for symbol definitions._

---

??? info "Basic Configuration"

    | Property                     | Type | Data Type       | Example          | Comments |
    |------------------------------|------|-----------------|------------------|----------|
    | Name                         | *    | String          | 2 Axis Recording |          |
    | Motion Pattern               | *    | List of strings |                  | Options: Unknown, Raster, Continuous Rotation, Helical |
    | Start from current position  | *    | Boolean         |                  |          |
    | Set Encoders On Start        | *    | Boolean         |                  |          |
    | Automatically Clear Data     | *    | Boolean         |                  | Clear Data On Scan Start |

---

??? info "Encoder Pre-Sets"

    | Property             | Type | Data Type | Example | Comments |
    |----------------------|------|-----------|---------|----------|
    | Set Scan Encoder To  | *    | Double    |         | Encoder Pre-Set: Scan |
    | Set Index Encoder To | *    | Double    |         | Encoder Pre-Set: Index |

---

??? info "Scan Axis"

    | Property         | Type | Data Type | Units | Example | Comments                                   |
    |------------------|------|-----------|--------|---------|--------------------------------------------|
    | Scan Axis        | *    | String    |        | X       | Axis : Scan                                |
    | Scan Start       | *    | Double    |        |         |                                            |
    | Scan Length      | *    | Double    |        |         |                                            |
    | Scan End         | A    | Double    |        |         | End Autocalculated from Start & Length     |
    | Scan Resolution  | *    | Double    |        |         |                                            |

---

??? info "Index Axis"

    | Property          | Type | Data Type | Units | Example | Comments                                   |
    |-------------------|------|-----------|--------|---------|--------------------------------------------|
    | Index Axis        | *    | String    |        | Y       | Axis : Index                               |
    | Index Start       | *    | Double    |        |         |                                            |
    | Index Length      | *    | Double    |        |         |                                            |
    | Index End         | A    | Double    |        |         | End Autocalculated from Start & Length     |
    | Index Resolution  | *    | Double    |        |         |                                            |

---

??? info "Paintbrushing"

    | Property                   | Type | Data Type | Example | Comments         |
    |----------------------------|------|-----------|---------|------------------|
    | Swept Array Paintbrush     | *    | Boolean   |         | PA Paintbrushing |
    | Paintbrush Mode            | *    | Boolean   |         | Conv. Paintbrush |
    | Specify Backlash In Points | *    | Boolean   |         |                  |

---

## 🧭 Legend

| Symbol | Definition       |
|--------|------------------|
| *      | Required         |
| O      | Optional         |
| A      | Auto Calculated  |
| D      | Dependent        |