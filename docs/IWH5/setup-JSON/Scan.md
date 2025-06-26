# Scan

_See the [Legend](#legend) for symbol definitions._

---

## Basic Configuration

| Property                    | IW Scan Name                | Type | Data Type       | Example          | Comments                                               |
|-----------------------------|-----------------------------|------|-----------------|------------------|--------------------------------------------------------|
| Name                        |                             | *    | String          | 2 Axis Recording |                                                        |
| Motion Pattern              |                             | *    | List of strings |                  | Options: Unknown, Raster, Continuous Rotation, Helical |
| Start from current position | Start From Current Position | *    | Boolean         |                  |                                                        |
| Set Encoders On Start       | Pre-Set Encoders On Start   | *    | Boolean         |                  |                                                        |
| Automatically Clear Data    | Clear Data On Scan Start    | *    | Boolean         |                  | Clear Data On Scan Start                               |

## Encoder Pre-Sets

| Property             | IW Scan Name            | Type | Data Type |
|----------------------|-------------------------|------|-----------|
| Set Scan Encoder To  | Encoder Pre-Set : Scan  | *    | Double    |
| Set Index Encoder To | Encoder Pre-Set : Index | *    | Double    |

## Scan Axis

| Property        | IW Scan Name | Type | Data Type | Example | Comments                               |
|-----------------|--------------|------|-----------|---------|----------------------------------------|
| Scan Axis       | Axis : Scan  | *    | String    | X       | Axis : Scan                            |
| Scan Start      |              | *    | Double    |         |                                        |
| Scan Length     |              | *    | Double    |         |                                        |
| Scan End        |              | A    | Double    |         | End Autocalculated from Start & Length |
| Scan Resolution |              | *    | Double    |         |                                        |

## Index Axis

| Property         | IW Scan Name | Type | Data Type | Example | Comments                               |
|------------------|--------------|------|-----------|---------|----------------------------------------|
| Index Axis       | Axis : Index | *    | String    | Y       | Axis : Index                           |
| Index Start      |              | *    | Double    |         |                                        |
| Index Length     |              | *    | Double    |         |                                        |
| Index End        |              | A    | Double    |         | End Autocalculated from Start & Length |
| Index Resolution |              | *    | Double    |         |                                        |

## Paintbrushing

| Property                   | IW Scan Name        | Type | Data Type |
|----------------------------|---------------------|------|-----------|
| Swept Array Paintbrush     | PA Paintbrushing    | *    | Boolean   |
| Paintbrush Mode            | Conv. Paintbrushing | *    | Boolean   |
| Specify Backlash In Points | Backlash Amount     | *    | Boolean   |

---

## 🧭 Legend

| Symbol | Definition      |
|--------|-----------------|
| *      | Required        |
| O      | Optional        |
| A      | Auto Calculated |
| D      | Dependent       |
