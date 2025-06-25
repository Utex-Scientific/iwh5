# Device Encoder

_See the [Legend](#legend) for symbol definitions._

---

??? info "General"

    | Property | Type | Data Type | Example |
    |----------|------|-----------|---------|
    | Name     | *    | String    |         |

---

??? info "Encoder Settings"

    | Property       | Type | Data Type | Options                         | Units    | Example |
    |----------------|------|-----------|----------------------------------|----------|---------|
    | Channel        | *    | Integer   |                                  |          |         |
    | Encoder Mode   | *    | String    | Quadrature, Step/Direction       |          |         |

---

??? info "Calibration / Setup"

    | Property            | Type | Data Type      | Options      | Units     | Example | Comments                              |
    |---------------------|------|----------------|--------------|-----------|---------|---------------------------------------|
    | Modulus Enabled     | *    | Boolean        |              |           |         |                                       |
    | Rollover At         | D    | Double         |              |           |         | Dependent on Modulus Enabled          |
    | Measure per Step    | *    | Double         |              | mm/step   |         |                                       |
    | Steps per Measure   | A    | Double         |              | steps/mm  |         | Auto Calculated from Measure per Step |
    | Calibration Units   | *    | List of strings| mm, deg      |           |         |                                       |
    | Channel             | *    | Integer        | X–H (X,Y,Z…) |           |         |                                       |

---

??? info "Hardware"

    | Property            | Type | Data Type | Example | Comments                             |
    |---------------------|------|-----------|---------|--------------------------------------|
    | Hardware Modulus    | *    | Boolean   |         |                                      |
    | Reset Input Line    | *    | Integer   |         | Available if Hardware Modulus Enabled|
    | Rising Edge         | *    | Boolean   |         | Available if Hardware Modulus Enabled|
    | Terminated          | *    | Boolean   |         |                                      |
    | Encoder Filter      | *    | Integer   |         | Available if Terminated Enabled      |
    | Pulse Divider       | *    | Integer   |         | Available if Terminated Enabled      |
    | Backlash Period     | *    | Float     |         | Available if Terminated Enabled      |

---

??? info "Measured Speed"

    | Property             | Type | Data Type | Units | Example |
    |----------------------|------|-----------|--------|---------|
    | Encoder              | *    | Double    |        |         |
    | Minimum Time Interval| *    | Double    | s      |         |
    | Conversion Factor    | *    | Double    |        |         |

---

## 🧭 Legend

| Symbol | Meaning         |
|--------|------------------|
| *      | Required         |
| O      | Optional         |
| A      | Auto Calculated  |
| D      | Dependent        |
