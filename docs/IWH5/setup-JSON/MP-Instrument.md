# MicroPulse Instrument Properties

_See the [Legend](#legend) for symbol definitions._

---

## General

| Property                | Type | Data Type | Units | Example |
| ----------------------- | ---- | --------- | ----- | ------- |
| Name                    | *    | String    |       | MP      |
| Data Format             | *    | Integer   |       |         |
| Base Sampling Frequency | *    | String    | MHz   | 100     |

## Pulser Settings

| Property           | Type | Data Type | Units | Example |
| ------------------ | ---- | --------- | ----- | ------- |
| Ch 0 Pulse Width   | *    | String    | ns    | 100     |
| Ch 0 Pulse Voltage | *    | String    | V     | 200     |
| PAVoltage          | *    | Integer   | V     |         |
| PAWidth            | *    | Integer   | ns    |         |


## Receiver Settings

| Property     | Type | Data Type | Units | Example |
| ------------ | ---- | --------- | ----- | ------- |
| Ch 0 Damping | *    | Integer   | Ohm   |         |

## Collection Mode

| Property                  | Type | Data Type       | Units | Example |
| ------------------------- | ---- | --------------- | ----- | ------- |
| Preferred Collection Mode | *    | List of strings |       |         |
| Use Channel PRFs          | *    |                 |       |         |
| Channel PRF               | *    | Integer         | Hz    |         |

## Triggering

| Property           | Type | Data Type       | Units | Example |
| ------------------ | ---- | --------------- | ----- | ------- |
| Externally Trigger | *    | List of strings |       |         |
| Trigger Line       | D    | Integer         |       |         |
| Trigger Logic      | D    | Integer         |       |         |

---

## 🧭 Legend

| Symbol | Meaning         |
| ------ | --------------- |
| *      | Required        |
| O      | Optional        |
| A      | Auto Calculated |
| D      | Dependent       |
