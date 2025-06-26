# 📋 Channel Properties

_See the [Legend](#legend) for symbol definitions._

---

## General

| Property | Type | Data Type | Units | Example           |
| -------- | ---- | --------- | ----- | ----------------- |
| Name     | *    | String    |       | Conventional Ch A |

## Pulser/Receiver

| Property      | Type | Data Type       | Units | Example |
| ------------- | ---- | --------------- | ----- | ------- |
| Gain          | *    | Double          | dB    |         |
| Rectification | *    | List of Strings |       | RF      |

## Filters

| Property                 | Type | Data Type | Units | Example     |
| ------------------------ | ---- | --------- | ----- | ----------- |
| Filter                   | *    | String    |       | 2 to 10 MHz |
| Digital High Pass Filter | *    | String    |       | 0.7         |
| Digital Low Pass Filter  | *    | String    |       | 1.8         |
| Smoothing                | *    | Integer   |       |             |
| Number of Averages       | *    | String    |       | 2           |

## Digitizer

| Property          | Type | Data Type | Units | Example |
| ----------------- | ---- | --------- | ----- | ------- |
| Delay             | *    | Double    | us    |         |
| Range             | *    | Double    | us    |         |
| End               | *    | Double    | us    |         |
| Decimation Factor | *    | Integer   |       |         |

## Time To Distance

| Property           | Type | Data Type | Units | Example |
| ------------------ | ---- | --------- | ----- | ------- |
| Distance Type Mode | *    | String    |       | Path    |

## Butterworth Filter

| Property         | Type | Data Type | Units | Example |
| ---------------- | ---- | --------- | ----- | ------- |
| Filter Type      | *    | Integer   |       |         |
| Cutoff Frequency | *    | Double    | MHz   |         |

## AScan

| Property                   | Type | Data Type | Units | Example |
| -------------------------- | ---- | --------- | ----- | ------- |
| AScan Time Axis Res. Raw   | *    | Double    | us/mm |         |
| AScan Amplitude Resolution | *    | Double    | %     |         |

## Collection

| Property          | Type | Data Type | Units | Example |
| ----------------- | ---- | --------- | ----- | ------- |
| Scan Axis Offset  | *    | Double    | mm    |         |
| Index Axis Offset | *    | Double    | mm    |         |
| Merge Data Mode   | *    | String    |       |         |

## Dynamic Range Expansion

| Property                | Type | Data Type | Units | Example |
| ----------------------- | ---- | --------- | ----- | ------- |
| Dynamic Range Expansion | O    | String    |       |         |

---

## 🧭 Legend

| Symbol | Definition      |
| ------ | --------------- |
| *      | Required        |
| O      | Optional        |
| A      | Auto Calculated |
| D      | Dependent       |