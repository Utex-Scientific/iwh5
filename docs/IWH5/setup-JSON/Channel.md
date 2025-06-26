# 📋 Channel Properties

_See the [Legend](#legend) for symbol definitions._

---

## General

| Property | Type | Data Type | Units | Example           |
|----------|------|-----------|-------|-------------------|
| Name     | *    | String    |       | Conventional Ch A |

## Pulser/Receiver

| IW Property Name | Property Type | Data Type       | Options                                     | Units |
|------------------|---------------|-----------------|---------------------------------------------|-------|
| Gain             | *             | Double          |                                             | dB    |
| Rectification    | *             | List of strings | RF, Full Wave, Half Wave Pos, Half Wave Neg |       |

## Filters

| IW Property Name         | IW Scan Name       | Property Type | Data Type | Example     |
|--------------------------|--------------------|---------------|-----------|-------------|
| Filter                   | Hardware Filter    | *             | String    | 2 to 10 MHz |
| Digital High Pass Filter | Digitial High Pass | *             | String    | 0.7         |
| Digital Low Pass Filter  | Digitial Low Pass  | *             | String    | 1.8         |
| Smoothing                |                    | *             | Integer   |             |
| Number of Averages       | Averaging          | *             | String    | 2           |

## Digitizer

| IW Property Name  | IW Scan Name  | Property Type | Data Type | Units |
|-------------------|---------------|---------------|-----------|-------|
| Delay             | A-Scan Start  | *             | Double    | us    |
| Range             | A-Scan Length | *             | Double    | us    |
| End               | A-Scan End    | *             | Double    | us    |
| Decimation Factor | Compression   | *             | Integer   |       |

## Time To Distance

| IW Property Name   | IW Scan Name  | Property Type | Data Type | Example |
|--------------------|---------------|---------------|-----------|---------|
| Distance Type Mode | Distance Mode | *             | String    | Path    |

## Butterworth Filter

| IW Property Name | IW Scan Name | Property Type | Data Type | Options                        | Units |
|------------------|--------------|---------------|-----------|--------------------------------|-------|
| Filter Type      | Filter Mode  | *             | Integer   | High Pass, Low Pass, Band Pass |       |
| Cutoff Frequency |              | *             | Double    |                                | MHz   |

## AScan

| IW Property Name               | IW Scan Name               | Property Type | Data Type | Units |
|--------------------------------|----------------------------|---------------|-----------|-------|
| AScan Time Axis Resolution Raw | Time Axis Res: (us) / (mm) | *             | Double    | us/mm |
| AScan Amplitude Resolution     | Amplitude Resolution: (%)  | *             | Double    | %     |

## Collection

| IW Property Name  | IW Scan Name            | Property Type | Data Type | Options                                                                                                                 | Units |
|-------------------|-------------------------|---------------|-----------|-------------------------------------------------------------------------------------------------------------------------|-------|
| Scan Axis Offset  | Scan Axis Offset: (mm)  | *             | Double    |                                                                                                                         | mm    |
| Index Axis Offset | Index Axis Offset: (mm) | *             | Double    |                                                                                                                         | mm    |
| Merge Data Mode   |                         | *             | String    | Replace, Maximum, Minimum, Abs Maximum, Average, Min and Max, First, Deepest, Shallowest, Magnitude, If Previous Merged |       |

## Dynamic Range Expansion

| IW Property Name        | IW Scan Name | Property Type | Data Type |
|-------------------------|--------------|---------------|-----------|
| Dynamic Range Expansion | Mode         | O             | String    |

---

## 🧭 Legend

| Symbol | Definition      |
|--------|-----------------|
| *      | Required        |
| O      | Optional        |
| A      | Auto Calculated |
| D      | Dependent       |
