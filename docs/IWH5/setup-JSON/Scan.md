# Scan
See the [Legend](#legend) for symbol definitions.

| Section | IW Property Name            | IW Scan Name                | Property Type | Data Type       | Options                                    | Units | Other Unit Options | Example          | Comments                                   |
|---------|-----------------------------|-----------------------------|---------------|-----------------|--------------------------------------------|-------|--------------------|------------------|--------------------------------------------|
|         | Name                        |                             | *             | String          |                                            |       |                    | 2 Axis Recording |                                            |
|         | Motion Pattern              |                             | *             | List of strings | Unknown,Raster,Continuous Rotation,Helical |       |                    |                  |                                            |
|         | Start from current position | Start From Current Position | *             | Boolean         |                                            |       |                    |                  |                                            |
|         | Set Encoders On Start       | Pre-Set Encoders On Start   | *             | Boolean         |                                            |       |                    |                  |                                            |
|         | Set Scan Encoder To         | Encoder Pre-Set : Scan      | *             | Double          |                                            |       |                    |                  |                                            |
|         | Set Index Encoder To        | Encoder Pre-Set : Index     | *             | Double          |                                            |       |                    |                  |                                            |
|         | Scan Axis                   | Axis : Scan                 | *             | String          |                                            |       |                    | X                |                                            |
|         | Scan Start                  |                             | *             | Double          |                                            |       |                    |                  |                                            |
|         | Scan Length                 |                             | *             | Double          |                                            |       |                    |                  |                                            |
|         | Scan End                    |                             | A             | Double          |                                            |       |                    |                  | End Autocalculated based on Start & Length |
|         | Scan Resolution             |                             | *             | Double          |                                            |       |                    |                  |                                            |
|         | Index Axis                  | Axis : Index                | *             | String          |                                            |       |                    | Y                |                                            |
|         | Index Start                 |                             | *             | Double          |                                            |       |                    |                  |                                            |
|         | Index Length                |                             | *             | Double          |                                            |       |                    |                  |                                            |
|         | Index End                   |                             | A             | Double          |                                            |       |                    |                  | End Autocalculated based on Start & Length |
|         | Index Resolution            |                             | *             | Double          |                                            |       |                    |                  |                                            |
|         | Automatically Clear Data    | Clear Data On Scan Start    | *             | Boolean         |                                            |       |                    |                  |                                            |
|         | Swept Array Paintbrush      | PA Paintbrushing            | *             | Boolean         |                                            |       |                    |                  |                                            |
|         | Paintbrush Mode             | Conv. Paintbrushing         | *             | Boolean         |                                            |       |                    |                  |                                            |
|         | Specify Backlash In Points  | Backlash Amount             | *             | Boolean         |

## Legend

| Symbol | Meaning         |
|--------|------------------|
| *      | Required         |
| O      | Optional         |
| A      | Auto Calculated  |
| D      | Dependent        |