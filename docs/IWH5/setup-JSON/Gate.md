# Gate

_See the [Legend](#legend) for symbol definitions._

---

## Gate Setup

| IW Property Name | IW Scan Name | Property Type | Data Type       | Options                                      | Units  | Example |
|------------------|--------------|---------------|-----------------|----------------------------------------------|--------|---------|
| Name             |              | A             | String          |                                              |        | Gate 1  |
| Gate Tag         | Tag          | O             | String          |                                              |        |         |
| Delay            |              | *             | Double          |                                              | us     |         |
| Range            |              | *             | Double          |                                              | us     |         |
| Parent Gate      | Follows      | *             | List of Strings | Pulse, IF, [Gate Name]                       |        |         |
| Start            |              | *             | Double          |                                              | mm     |         |
| Length           |              | A             | Double          |                                              | mm     |         |
| End              |              | A             | Double          |                                              | mm     |         |
| Threshold        |              | *             | Double          |                                              | % or V |         |
| Relative To      | Follows      | *             | List of Strings | Interface, Gate Start, Zero, First Interface |        |         |

### Comments

| IW Property Name | Comment                             |
|------------------|-------------------------------------|
| Length           | Autocalculated from start and range |
| End              | Autocalculated from start and range |

## Amplitude Measurement

| IW Property Name            | IW Scan Name            | Property Type | Data Type       | Options                                                                                                          | Comments                |
|-----------------------------|-------------------------|---------------|-----------------|------------------------------------------------------------------------------------------------------------------|-------------------------|
| Amplitude Type              | Measurement Type        | *             | List of Strings | Peak, Peak To Peak                                                                                               |                         |
| Amplitude Peak              | Measurement At          | *             | List of Strings | Maximum, Minimum, Extreme, Largest Peak Over Threshold, First Peak Over Threshold, ..., Last Peak Over Threshold |                         |
| If Amp Peak Below Threshold | If No Crossing          | D             | List of Strings | Set To Undefined, Set To Zero, Set To Maximum, Set To Largest Peak                                               | Based on Amplitude Peak |
| Interpolate Amplitude       | Interpolate Measurement | *             | Boolean         |                                                                                                                  |                         |
| Absolute                    | Absolute Measurement    | *             | Boolean         |                                                                                                                  |                         |

## Time-of-Flight (TOF) Measurement

| IW Property Name            | IW Scan Name            | Property Type | Data Type       | Options                                                              | Units |
|-----------------------------|-------------------------|---------------|-----------------|----------------------------------------------------------------------|-------|
| TOF Type                    | Measurement Type        | *             | List of Strings | Peak, Threshold, Threshold Relative To Peak                          |       |
| TOF Peak                    | Peak Measurement At     | *             | List of Strings | Maximum, Minimum, Extreme, First/Second/... Last Peak Over Threshold |       |
| Reference Peak Height       |                         | D             | Double          |                                                                      |       |
| If Amp Peak Below Threshold | If No Crossing          | D             | List of Strings | Set To Undefined, Set To Zero, Set To Maximum, Set To Largest Peak   |       |
| Relative To                 | Measurement Relative To | *             | List of Strings | Interface, First Interface, Zero (Parent Gate, IF Gate, AScan Zero)  |       |
| Trim                        |                         | *             | Double          |                                                                      | us    |
| Trim Converted              |                         | A             | Double          |                                                                      | mm    |

### Comments

| IW Property Name | Comment           |
|------------------|-------------------|
| Length           | Based on TOF Peak |
| End              | Based on TOF Peak |

## Alarm Configuration

| IW Property Name | IW Scan Name | Property Type | Data Type       | Options                          | Units | Comments                |
|------------------|--------------|---------------|-----------------|----------------------------------|-------|-------------------------|
| Show Alarm       | Alarm        | *             | Boolean         |                                  |       |                         |
| Condition        | Trigger When | D             | List of Strings | Above Threshold, Below Threshold |       | Set based on Show Alarm |
| Alarm Mode       | Trigger Mode | D             | List of Strings | Simple, Persistent               |       | Set based on Show Alarm |
| Persist Time     |              | D             | Double          |                                  | s     | Set based on Show Alarm |

---

## 🧭 Legend

| Symbol | Definition      |
|--------|-----------------|
| *      | Required        |
| O      | Optional        |
| A      | Auto Calculated |
| D      | Dependent       |
