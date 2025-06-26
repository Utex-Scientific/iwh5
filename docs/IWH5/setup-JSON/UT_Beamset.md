# UT Beamset

_See the [Legend](#legend) for symbol definitions._

---

## Settings

| IW Property Name | IW Scan Name    | Property Type | Data Type       | Options             | Units |
|------------------|-----------------|---------------|-----------------|---------------------|-------|
| Inspection Mode  |                 | *             | List of strings | Longitudinal, Shear |       |
| Beam Angle       | Refracted Angle | *             | Double          |                     | deg   |
| First Element    |                 | *             | Integer         |                     |       |
| Aperture         |                 | *             | Integer         |                     |       |
| Element Step     | Step            | *             | Integer         |                     |       |
| Linear Start     |                 | *             | Double          |                     |       |
| Number of Beams  |                 | *             | Integer         |                     |       |
| Focal Law        | A               |               | Law file/xml    |                     |       |
| Focus Type       |                 | O             | String          | None, Path, Depth   |       |

### Comments

| IW Property Name | Comment                          |
|------------------|----------------------------------|
| Focus Law        | In setup json as a focalLawTable |
| Focus Type       | Example: Path                    |

---

## 🧭 Legend

| Symbol | Definition      |
|--------|-----------------|
| *      | Required        |
| O      | Optional        |
| A      | Auto Calculated |
| D      | Dependent       |
