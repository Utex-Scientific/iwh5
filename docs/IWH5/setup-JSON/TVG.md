# TVG (Time-Varied Gain)

_See the [Legend](#legend) for symbol definitions._

---

## Setup

| IW Property Name | IW Scan Name | Property Type | Data Type | Units | Example | Comments |
| ---------------- | ------------ | ------------- | --------- | ----- | ------- | -------- |
| Simple TVG       |              | *             | Boolean   |       |         |          |
| Start            |              | *             | Double    | us    |         |          |

## Points

| IW Property Name     | IW Scan Name | Property Type | Data Type | Units | Example | Comments                    |
| -------------------- | ------------ | ------------- | --------- | ----- | ------- | --------------------------- |
| Number Of Points     |              | *             | Integer   |       |         |                             |
| Points               |              | *             | List      |       |         | In setup JSON as `tvgTable` |
| Auto Level Amplitude |              | *             | Double    |       |         |                             |
| Time Tolerance       | Tolerance    | *             | Double    | us    |         |                             |

## Advanced

| IW Property Name | IW Scan Name                        | Property Type | Data Type | Units          | Example | Comments                               |
| ---------------- | ----------------------------------- | ------------- | --------- | -------------- | ------- | -------------------------------------- |
| Active Width     |                                     | D             | Double    | us             |         | Available if Advanced TVG Mode enabled |
| Enable 2nd Gain  |                                     | O             | Boolean   |                |         |                                        |
| 2nd Gain         | Gain                                | D             | Double    | dB             |         | Available if 2nd Gain enabled          |
| MAC              | Material Amplitude Correction (MAC) | D             | Double    | dB/us or dB/mm |         | Available if Advanced TVG Mode enabled |

### Comments

| IW Property Name | Comment|
| --- | -- |
| Active Width | Available if Advanced TVG Mode enabled |

---

## 🧭 Legend

| Symbol | Definition      |
| ------ | --------------- |
| *      | Required        |
| O      | Optional        |
| A      | Auto Calculated |
| D      | Dependent       |
