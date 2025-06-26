# MicroPulse Instrument Properties

_See the [Legend](#legend) for symbol definitions._

---

## Global Instrument Settings

| IW Property Name        | IW Scan Name     | Property Type | Data Type | Options                                   | Units | Example |
|-------------------------|------------------|---------------|-----------|-------------------------------------------|-------|---------|
| Name                    |                  | *             | String    |                                           |       | MP      |
| Data Format             |                  | *             | Integer   | 8 Bit, 12 Bit, 16 Bit, 8 Bit Logirathamic |       |         |
| Base Sampling Frequency | Base Sample Rate | *             | String    |                                           | MHz   | 100     |

## Conventioanl Channel Settings

| IW Property Name   | IW Scan Name              | Property Type | Data Type | Units | Example |
|--------------------|---------------------------|---------------|-----------|-------|---------|
| Ch 0 Pulse Width   | Global Pulse Width: (ns)  | *             | String    | ns    | 100     |
| Ch 0 Damping       | Global Damping: (Ω)       | *             | Integer   | Ohm   |         |
| Ch 0 Pulse Voltage | Global Pulse Voltage: (V) | *             | String    | V     | 200     |

## PA Channel Settings

| IW Property Name | IW Scan Name       | Property Type | Data Type | Options | Units |
|------------------|--------------------|---------------|-----------|---------|-------|
| PAVoltage        | Pulse Voltage: (V) | *             | Integer   |         | V     |
| PAWidth          | Pulse Width: (ns)  | *             | Integer   |         | ns    |

## Collection Mode

| IW Property Name          | IW Scan Name    | Property Type | Data Type       | Options                                                                                                         | Units |
|---------------------------|-----------------|---------------|-----------------|-----------------------------------------------------------------------------------------------------------------|-------|
| Use Channel PRFs          | Recurrence      | *             |                 |                                                                                                                 |       |
| Preferred Collection Mode | Collection Mode | *             | List of strings | Software Trigger, Position Stamped, Trigger on Position, Two Axis Position Stamped, External Tigger on Position |       |
| Channel PRF               | PRF             | *             | Integer         |                                                                                                                 | Hz    |


## External Triggering

| IW Property Name   | IW Scan Name | Property Type | Data Type       | Options                      | Comments                                                    |
|--------------------|--------------|---------------|-----------------|------------------------------|-------------------------------------------------------------|
| Externally Trigger |              | *             | List of strings | None, While Scanning, Always | If While scanning or always, enables Trigger Line and Logic |
| Trigger Line       |              | D             | Integer         | 0 to 15                      | Depends on Externally Trigger                               |
| Trigger Logic      |              | D             | Integer         | High to Low, Low to High     | Depends on Externally Trigger                               |

---

## 🧭 Legend

| Symbol | Meaning         |
|--------|-----------------|
| *      | Required        |
| O      | Optional        |
| A      | Auto Calculated |
| D      | Dependent       |
