# Micropulse Device Encoder

_See the [Legend](#legend) for symbol definitions._

---

## Encoder Settings

| IW Property Name | Property Type | Data Type | Options                    |
|------------------|---------------|-----------|----------------------------|
| Name             | *             | String    |                            |
| Channel          | *             | Integer   |                            |
| Encoder Mode     | *             | String    | Quadrature, Step/Direction |

## Calibration/Setup

| IW Property Name  | Property Type | Data Type       | Options         | Units    |
|-------------------|---------------|-----------------|-----------------|----------|
| Modulus Enabled   | *             | Boolean         |                 |          |
| Rollover At       | D             | Double          |                 |          |
| Measure per Step  | *             | Double          |                 | mm/step  |
| Steps per Measure | A             | Double          |                 | steps/mm |
| Calibration Units | *             | List of strings | mm, deg         |          |
| Channel           | *             | Integer         | X,Y,Z,W,E,F,G,H |          |

### Comments

| IW Property Name  | Comments                              |
|-------------------|---------------------------------------|
| Rollover At       | Dependent on Modulus Enabled          |
| Measure per Step  |                                       |
| Steps per Measure | Auto Calculated from Measure per Step |
| Reset Input Line  | Available if Hardware Modulus Enabled |
| Rising Edge       | Available if Hardware Modulus Enabled |

## Hardware

| IW Property Name | IW Scan Name            | Property Type | Data Type | Units |
|------------------|-------------------------|---------------|-----------|-------|
| Hardware Modulus | Hardware Encoder Reset: | *             | Boolean   |       |
| Reset Input Line |                         | *             | Integer   |       |
| Rising Edge      |                         | *             | Boolean   |       |
| Terminated       |                         | *             | Boolean   |       |
| Encoder Filter   |                         | *             | Integer   |       |
| Pulse Divider    |                         | *             | Integer   |       |
| Backlash Period  |                         | *             | Float     | s     |

### Comments

| IW Property Name | Comment                         |
|------------------|---------------------------------|
| Encoder Filter   | Available if Terminated Enabled |
| Pulse Divider    | Available if Terminated Enabled |
| Backlash Period  | Available if Terminated Enabled |

## Measured Speed

| IW Property Name      | IW Scan Name         | Property Type | Data Type | Units |
|-----------------------|----------------------|---------------|-----------|-------|
| Encoder               |                      | *             | Double    |       |
| Minimum Time Interval | Update Interval: (s) | *             | Double    | s     |
| Conversion Factor     |                      | *             | Double    |       |

---

## 🧭 Legend

| Symbol | Definition      |
|--------|-----------------|
| *      | Required        |
| O      | Optional        |
| A      | Auto Calculated |
| D      | Dependent       |
