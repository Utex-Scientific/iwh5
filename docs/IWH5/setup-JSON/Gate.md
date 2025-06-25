# Gate

_See the [Legend](#legend) for symbol definitions._

---

??? info "Gate Setup"

    | Property     | Type | Data Type       | Units | Example | Comments                            |
    |--------------|------|-----------------|--------|---------|-------------------------------------|
    | Name         | A    | String          |        | Gate 1  |                                     |
    | Gate Tag     | O    | String          |        |         |                                     |
    | Delay        | *    | Double          | us     |         |                                     |
    | Range        | *    | Double          | us     |         |                                     |
    | Parent Gate  | *    | List of Strings |        |         | Options: Pulse, IF, [Gate Name]     |
    | Start        | *    | Double          | mm     |         |                                     |
    | Length       | A    | Double          | mm     |         | Auto-calculated from start + range |
    | End          | A    | Double          | mm     |         | Auto-calculated from start + range |
    | Threshold    | *    | Double          | % / V  |         |                                     |

---

??? info "Amplitude Measurement"

    | Property                    | Type | Data Type       | Comments |
    |-----------------------------|------|-----------------|----------|
    | Amplitude Type              | *    | List of Strings | Options: Peak, Peak To Peak |
    | Amplitude Peak              | *    | List of Strings | Options include Maximum, Minimum, Largest Peak Over Threshold, etc. |
    | If Amp Peak Below Threshold| D    | List of Strings | Based on Amplitude Peak (e.g., Set To Undefined, Zero, Max) |
    | Interpolate Amplitude      | *    | Boolean         |          |
    | Absolute                   | *    | Boolean         | Absolute Measurement |

---

??? info "Time-of-Flight (TOF) Measurement"

    | Property                    | Type | Data Type       | Comments |
    |-----------------------------|------|-----------------|----------|
    | TOF Type                    | *    | List of Strings | Options: Peak, Threshold, Threshold Relative To Peak |
    | TOF Peak                    | *    | List of Strings | Same options as Amplitude Peak |
    | Reference Peak Height       | D    | Double          | Based on TOF Peak              |
    | If Amp Peak Below Threshold| D    | List of Strings | Same as above                 |
    | Relative To (TOF)          | *    | List of Strings | Measurement Relative To: Interface, First Interface, etc. |
    | Trim                        | *    | Double          | Units: us |
    | Trim Converted              | A    | Double          | Units: mm |

---

??? info "Alarm Configuration"

    | Property      | Type | Data Type       | Comments                          |
    |---------------|------|-----------------|-----------------------------------|
    | Show Alarm    | *    | Boolean         | Alarm enabled/visible             |
    | Condition     | D    | List of Strings | Based on Show Alarm: Above/Below Threshold |
    | Alarm Mode    | D    | List of Strings | Simple or Persistent              |
    | Persist Time  | D    | Double          | Units: seconds                    |

---

## 🧭 Legend

| Symbol | Meaning         |
|--------|------------------|
| *      | Required         |
| O      | Optional         |
| A      | Auto Calculated  |
| D      | Dependent        |
