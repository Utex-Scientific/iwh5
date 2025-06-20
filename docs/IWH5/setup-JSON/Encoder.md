# Device Encoder
See the [Legend](#legend) for symbol definitions.

| Section           | IW Property Name      | IW Scan Name            | Property Type | Data Type       | Options                    | Units    | Other Unit Options | Example | Comments                              |
|-------------------|-----------------------|-------------------------|---------------|-----------------|----------------------------|----------|--------------------|---------|---------------------------------------|
|                   | Name                  |                         | *             | String          |                            |          |                    |         |                                       |
| Encoder Settings  | Channel               |                         | *             | Integer         |                            |          |                    |         |                                       |
|                   | Encoder Mode          |                         | *             | String          | Quadrature, Step/Direction |          |                    |         |                                       |
| Calibration/Setup | Modulus Enabled       |                         | *             | Boolean         |                            |          |                    |         |                                       |
|                   | Rollover At           |                         | D             | Double          |                            |          |                    |         | Dependent on Modulus Enabled          |
|                   | Measure per Step      |                         | *             | Double          |                            | mm/step  |                    |         |                                       |
|                   | Steps per Measure     |                         | A             | Double          |                            | steps/mm |                    |         | Auto Calculated from Measure per Step |
|                   | Calibration Units     |                         | *             | List of strings | mm,deg                     |          |                    |         |                                       |
|                   | Channel               |                         | *             | Integer         | X,Y,Z,W,E,F,G,H            |          |                    |         |                                       |
| Hardware          | Hardware Modulus      | Hardware Encoder Reset: | *             | Boolean         |                            |          |                    |         |                                       |
|                   | Reset Input Line      |                         | *             | Integer         |                            |          |                    |         | Available if Hardware Modulus Enabled |
|                   | Rising Edge           |                         | *             | Boolean         |                            |          |                    |         | Available if Hardware Modulus Enabled |
|                   | Terminated            |                         | *             | Boolean         |                            |          |                    |         |                                       |
|                   | Encoder Filter        |                         | *             | Integer         |                            |          |                    |         | Avaiable if Terminated Enabled        |
|                   | Pulse Divider         |                         | *             | Integer         |                            |          |                    |         | Avaiable if Terminated Enabled        |
|                   | Backlash Period       |                         | *             | Float           |                            | s        |                    |         | Avaiable if Terminated Enabled        |
| Measured Speed    | Encoder               |                         | *             | Double          |                            |          |                    |         |                                       |
|                   | Minimum Time Interval | Update Interval: (s)    | *             | Double          |                            | s        |                    |         |                                       |
|                   | Conversion Factor     |                         | *             | Double          |

## Legend

| Symbol | Meaning         |
|--------|------------------|
| *      | Required         |
| O      | Optional         |
| A      | Auto Calculated  |
| D      | Dependent        |