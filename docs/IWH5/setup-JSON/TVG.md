# TVG
See the [Legend](#legend) for symbol definitions.

| Section  | IW Property Name     | IW Scan Name                        | Property Type | Data Type | Options                                                  | Units          | Other Unit Options | Example | Comments                               |
|----------|----------------------|-------------------------------------|---------------|-----------|----------------------------------------------------------|----------------|--------------------|---------|----------------------------------------|
| Setup    | Simple TVG           |                                     | *             | Boolean   |                                                          |                |                    |         |                                        |
|          | Start                |                                     | *             | Double    |                                                          | us             |                    |         |                                        |
| Points   | Number Of Points     |                                     | *             | Integer   |                                                          |                |                    |         |                                        |
|          | Points               |                                     | *             | List      | (Time 1,Path1,Depth1,Gain 1)(Time 2,Path2,Depth2,Gain2)… |                |                    |         | In setup json as tvgTable              |
|          | Auto Level Amplitude |                                     | *             | Double    |                                                          |                |                    |         |                                        |
|          | Time Tolerance       | Tolerance                           | *             | Double    |                                                          | us             |                    |         |                                        |
| Advanced | Active Width         |                                     | D             | Double    |                                                          | us             |                    |         | Available if Advanced TVG Mode enabled |
|          | Enable 2nd Gain      |                                     | O             | Boolean   |                                                          |                |                    |         |                                        |
|          | 2nd Gain             | Gain                                | D             | Double    |                                                          | dB             |                    |         | Available if 2nd Gain enabled          |
|          | MAC                  | Material Amplitude Correction (MAC) | D             | Double    |                                                          | dB/us or dB/mm |                    |         | Available if Advanced TVG Mode enabled |

## Legend

| Symbol | Meaning         |
|--------|------------------|
| *      | Required         |
| O      | Optional         |
| A      | Auto Calculated  |
| D      | Dependent        |