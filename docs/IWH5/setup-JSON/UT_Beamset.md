# UT Beamset
See the [Legend](#legend) for symbol definitions.

| Section  | IW Property Name | Property Type | IW Scan Name    | Data Type       | Options            | Units | Other Unit Options | Example | Comments                         |
|----------|------------------|---------------|-----------------|-----------------|--------------------|-------|--------------------|---------|----------------------------------|
| Settings | Inspection Mode  | *             |                 | List of strings | Longitudinal,Shear |       |                    |         |                                  |
|          | Beam Angle       | *             | Refracted Angle | Double          |                    | deg   |                    |         |                                  |
|          | First Element    | *             |                 | Integer         |                    |       |                    |         |                                  |
|          | Aperture         | *             |                 | Integer         |                    |       |                    |         |                                  |
|          | Element Step     | *             | Step            | Integer         |                    |       |                    |         |                                  |
|          | Linear Start     | *             |                 | Double          |                    |       |                    |         |                                  |
|          | Number of Beams  | *             |                 | Integer         |                    |       |                    |         |                                  |
|          | Focal Law        | A             |                 | Law file/xml    |                    |       |                    |         | In setup json as a focalLawTable |
|          | Focus Type       | O             |                 | String          | None,Path,Depth    |       |                    | Path    |

## Legend

| Symbol | Meaning         |
|--------|------------------|
| *      | Required         |
| O      | Optional         |
| A      | Auto Calculated  |
| D      | Dependent        |