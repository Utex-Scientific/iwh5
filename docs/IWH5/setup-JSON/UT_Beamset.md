# UT Beamset

_See the [Legend](#legend) for symbol definitions._

---

??? info "Properties"

    | IW Property Name   | IW Scan Name     | Property Type | Data Type     | Options                    | Units | Example | Comments                          |
    |--------------------|------------------|---------------|---------------|----------------------------|--------|---------|-----------------------------------|
    | Inspection Mode    |                  | *             | List of strings | Longitudinal, Shear       |        |         |                                   |
    | Beam Angle         | Refracted Angle  | *             | Double        |                            | deg    |         |                                   |
    | First Element      |                  | *             | Integer       |                            |        |         |                                   |
    | Aperture           |                  | *             | Integer       |                            |        |         |                                   |
    | Element Step       | Step             | *             | Integer       |                            |        |         |                                   |
    | Linear Start       |                  | *             | Double        |                            |        |         |                                   |
    | Number of Beams    |                  | *             | Integer       |                            |        |         |                                   |
    | Focal Law          |                  | A             | Law file/xml  |                            |        |         | In setup JSON as `focalLawTable`  |
    | Focus Type         |                  | O             | String        | None, Path, Depth          |        | Path    |                                   |

---

## 🧭 Legend

| Symbol | Meaning         |
|--------|------------------|
| *      | Required         |
| O      | Optional         |
| A      | Auto Calculated  |
| D      | Dependent        |
