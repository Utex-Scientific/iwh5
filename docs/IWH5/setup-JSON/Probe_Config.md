# Probe Configuration

_See the [Legend](#legend) for symbol definitions._

---

## General

| Property           | Type | Data Type       | Units | Example         |
| ------------------ | ---- | --------------- | ----- | --------------- |
| Name               | *    | String          |       | Conventional UT |
| Probe Type         | A    | String          |       | Conventional    |
| Scanning Direction | *    | List of strings |       |                 |
| Probe Orientation  | *    | List of strings |       |                 |
| Surface            | *    | List of strings |       |                 |
| Scan Offset        | *    | Double          | mm    |                 |
| Index Offset       | *    | Double          | mm    |                 |
| Interface Type     | *    | List of strings |       |                 |
| Frequency          | *    | Double          |       |                 |
| Bandwidth          | *    | Double          |       |                 |
| Instrument Channel | *    | Integer         |       |                 |
| Device Index       | *    | Integer         |       |                 |

## Linear Array

| Property                 | Type | Data Type       | Units | Example |
| ------------------------ | ---- | --------------- | ----- | ------- |
| Manufacturer             | O    | String          |       |         |
| Transducer Part Number   | O    | String          |       |         |
| Transducer Serial Number | O    | String          |       |         |
| Number Of Elements X     | *    | Integer         |       |         |
| Element Pitch X          | *    | Double          | mm    |         |
| Element Width X          | *    | Double          | mm    |         |
| Element Width Y          | *    | Double          | mm    |         |
| Focusing Type            | *    | List of strings |       |         |
| Element Map              | *    | List of strings |       |         |

## Conventional

| Property         | Type | Data Type       | Units | Example |
| ---------------- | ---- | --------------- | ----- | ------- |
| Focusing Type    | *    | List of strings |       |         |
| Element Shape    | *    | List of strings |       |         |
| Element Diameter | *    | Double          | mm    |         |
| Length           | D    | Double          | mm    |         |
| Focal Length     | *    | Double          |       |         |
| Inspection Mode  | *    | List of strings |       |         |

## Coupling

| Property           | Type | Data Type | Units | Example |
| ------------------ | ---- | --------- | ----- | ------- |
| _(None specified)_ |      |           |       |         |

## Immersion

| Property                   | Type | Data Type | Units | Example |
| -------------------------- | ---- | --------- | ----- | ------- |
| Beam Angle in Couplant     | *    | Double    | deg   |         |
| Path In Couplant           | *    | Double    | mm    |         |
| Couplant Material          | *    | String    |       | Water   |
| Couplant Velocity of Sound | *    | Double    | mm/us |         |

## Wedge (Linear Array)

| Property                   | Type | Data Type | Units | Example    |
| -------------------------- | ---- | --------- | ----- | ---------- |
| Wedge Part Number          | O    | String    |       |            |
| Wedge Serial Number        | O    | String    |       |            |
| Manufacturer               | O    | String    |       |            |
| Wedge Angle                | *    | Double    | deg   |            |
| Wedge Roof Angle           | *    | Double    | deg   |            |
| Height At First Element    | *    | Double    | mm    |            |
| Length To First Element    | *    | Double    | mm    |            |
| Length After First Element | *    | Double    | mm    |            |
| Wedge Length               | *    | Double    | mm    |            |
| Wedge Height               | *    | Double    | mm    |            |
| Wedge Width                | *    | Double    | mm    |            |
| Damping Groove Depth       | *    | Double    | mm    |            |
| Material                   | *    | String    |       | Plexiglass |
| Longitudinal Velocity      | *    | Double    | mm    |            |

## Wedge (Conventional)

| Property              | Type | Data Type | Units | Example |
| --------------------- | ---- | --------- | ----- | ------- |
| Wedge Part Number     | O    | String    |       |         |
| Wedge Serial Number   | O    | String    |       |         |
| Manufacturer          | O    | String    |       |         |
| Wedge Angle           | *    | Double    | deg   |         |
| Wedge Roof Angle      | *    | Double    | deg   |         |
| Wedge Back Height     | *    | Double    |       |         |
| Wedge Exit Point      | *    | Double    |       |         |
| Wedge Length          | *    | Double    | mm    |         |
| Wedge Height          | *    | Double    | mm    |         |
| Wedge Width           | *    | Double    | mm    |         |
| Damping Groove Depth  | *    | Double    | mm    |         |
| Material              | *    | String    |       |         |
| Longitudinal Velocity | *    | Double    | mm    |         |

---

## 🧭 Legend

| Symbol | Definition      |
| ------ | --------------- |
| *      | Required        |
| O      | Optional        |
| A      | Auto Calculated |
| D      | Dependent       |