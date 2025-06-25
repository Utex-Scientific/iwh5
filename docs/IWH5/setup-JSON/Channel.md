# 📋 Channel Properties

_See the [Legend](#legend) for symbol definitions._

---

??? info "General"

    | Property | Type | Data Type | Units | Example           |
    |----------|------|-----------|-------|-------------------|
    | Name     | *    | String    |       | Conventional Ch A |

---

??? info "Pulser/Receiver"

    | Property      | Type | Data Type       | Units | Example |
    |---------------|------|-----------------|-------|---------|
    | Gain          | *    | Double          | dB    |         |
    | Rectification | *    | List of Strings |       | RF      |

---

??? info "Filters"

    | Property                 | Type | Data Type | Units | Example     |
    |--------------------------|------|-----------|-------|-------------|
    | Filter                   | *    | String    |       | 2 to 10 MHz |
    | Digital High Pass Filter | *    | String    |       | 0.7         |
    | Digital Low Pass Filter  | *    | String    |       | 1.8         |
    | Smoothing                | *    | Integer   |       |             |
    | Number of Averages       | *    | String    |       | 2           |

---

??? info "Digitizer"

    | Property          | Type | Data Type | Units | Example |
    |-------------------|------|-----------|-------|---------|
    | Delay             | *    | Double    | us    |         |
    | Range             | *    | Double    | us    |         |
    | End               | *    | Double    | us    |         |
    | Decimation Factor | *    | Integer   |       |         |

---

??? info "Time To Distance"

    | Property           | Type | Data Type | Units | Example |
    |--------------------|------|-----------|-------|---------|
    | Distance Type Mode | *    | String    |       | Path    |

---

??? info "Butterworth Filter"

    | Property         | Type | Data Type | Units | Example |
    |------------------|------|-----------|-------|---------|
    | Filter Type      | *    | Integer   |       |         |
    | Cutoff Frequency | *    | Double    | MHz   |         |

---

??? info "AScan"

    | Property                   | Type | Data Type | Units | Example |
    |----------------------------|------|-----------|-------|---------|
    | AScan Time Axis Res. Raw   | *    | Double    | us/mm |         |
    | AScan Amplitude Resolution | *    | Double    | %     |         |

---

??? info "Collection"

    | Property           | Type | Data Type | Units | Example |
    |--------------------|------|-----------|-------|---------|
    | Scan Axis Offset   | *    | Double    | mm    |         |
    | Index Axis Offset  | *    | Double    | mm    |         |
    | Merge Data Mode    | *    | String    |       |         |

---

??? info "Dynamic Range Expansion"

    | Property                | Type | Data Type | Units | Example |
    |-------------------------|------|-----------|-------|---------|
    | Dynamic Range Expansion | O    | String    |       |         |

---

## 🧭 Legend

| Symbol | Meaning         |
|--------|------------------|
| *      | Required         |
| O      | Optional         |
| A      | Auto Calculated  |
| D      | Dependent        |