# TVG (Time-Varied Gain)

_See the [Legend](#legend) for symbol definitions._

---

## Setup

| IW Property Name | Property Type | Data Type | Options | Units |
|------------------|---------------|-----------|---------|-------|
| Simple TVG       | *             | Boolean   |         |       |
| Start            | *             | Double    |         | us    |

## Points

| IW Property Name     | IW Scan Name | Property Type | Data Type | Options                                                 | Units |
|----------------------|--------------|---------------|-----------|---------------------------------------------------------|-------|
| Number Of Points     |              | *             | Integer   |                                                         |       |
| Points               |              | *             | List      | (Time1,Path1,Depth1,Gain1)(Time2,Path2,Depth2,Gain2)... |       |
| Auto Level Amplitude |              | *             | Double    |                                                         |       |
| Time Tolerance       | Tolerance    | *             | Double    |                                                         | us    |

### Comments

| IW Property Name | Comment                   |
|------------------|---------------------------|
| Points           | In setup json as tvgTable |

## Advanced

| IW Property Name | IW Scan Name                        | Property Type | Data Type | Units          | Comments                               |
|------------------|-------------------------------------|---------------|-----------|----------------|----------------------------------------|
| Active Width     |                                     | D             | Double    | us             | Available if Advanced TVG Mode enabled |
| Enable 2nd Gain  |                                     | O             | Boolean   |                |                                        |
| 2nd Gain         | Gain                                | D             | Double    | dB             | Available if 2nd Gain enabled          |
| MAC              | Material Amplitude Correction (MAC) | D             | Double    | dB/us or dB/mm | Available if Advanced TVG Mode enabled |




---

## 🧭 Legend

| Symbol | Definition      |
|--------|-----------------|
| *      | Required        |
| O      | Optional        |
| A      | Auto Calculated |
| D      | Dependent       |
