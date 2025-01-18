# TBI Fuel Injection ECM Connector Identification

This document reproduces the data from a 1990s Chevrolet TBI (Throttle Body Injection) ECM/PCM wiring and voltage‐reference chart exactly as shown in the provided image. All tables, pin designations, wire colors, circuit names, voltage references, and footnotes are included below for completeness.

---

## Overview Text From Original Diagram

“This ECM voltage chart is for use with a digital voltmeter to further aid in diagnosis. The voltages you get may vary due to low battery charge or other reasons, but they should be very close.

**THE FOLLOWING CONDITIONS MUST BE MET BEFORE TESTING:**  
• Engine at operating temperature  
• Engine idling (for “Engine Run” column)  
• Diagnostic terminal not grounded  
• ALDL tool not installed”

---

## 24-Pin A–B Connector and 32-Pin C–D Connector (Back Views)

Below are two main tables. The first section (A–B) corresponds to a 24-pin connector split into A1–A12 and B1–B12. The second section (C–D) corresponds to a 32-pin connector split into C1–C16 and D1–D16. Voltages are shown for “Key On” and “Engine Run” as given in the original chart.

---

### A-Side Pins (24-Pin Connector, Rows A1–A12)

| Voltage         |       |               |      |             |
|-----------------|-------|---------------|------|-------------|
| **Key “On”**   | **Eng “Run”** | **Circuit**                               | **Pin** | **Wire Color** |
| 0              | 14     | Fuel Pump Relay                                | A1  | OK GRN/WHT         |
| –              | –      | Not used                                       | A2  | –           |
| –              | –      | Not used                                       | A3  | –           |
| 12             | 14     | EGR Control                                    | A4  | GRY         |
| 0              | 14     | “Service Engine Soon” Control                  | A5  | BRN/WHT         |
| 12             | 14     | IGN – ECM Fuse SHIFT LIGHT or ECC CONTROL      | A6  | PNK/BLK |
| 12             | 14     | Shift Light or TCC Control                     | A7  | TAN/BLK           |
| 2–5            | 2.5    | Serial Data                                    | A8  | ORN         |
| 5              | 5      | Diagnostic Terminal                            | A9  | WHT/BLK         |
| (1)            | (1)    | Speed Sensor Signal                            | A10 | BRN           |
| 0              | 0      | Sensor Ground                                  | A11 | PPL OR BLK         |
| 0              | 0      | System Ground                                  | A12 | BLK/WHT         |

> **Note**: Where “–” is shown, the chart in the image did not list any voltage or data.  
> “(Footnote 7?)” indicates a possible footnote reference in the original scan; actual voltage was not fully visible.  
> “(1)” references footnote 1 regarding a speed-sensor–dependent voltage.

---

### B-Side Pins (24-Pin Connector, Rows B1–B12)

| **Wire Color** | **Pin** | **Circuit**           | **Key “On”** | **Eng “Run”** |
|---------------|---------|-----------------------|--------------|--------------|
| ORN           | B1      | BATT. 12 Volts        | 12           | 14           |
| TAN/WHT       | B2      | Fuel Pump Signal      | 0            | 14           |
| BLK/RED       | B3      | EST Reflow            | 0            | 0            |
| –             | B4      | Not used              | –            | –            |
| PPL/WHT       | B5      | EST Reference Hi      | 0            | 1.8          |
| –             | B6      | Not used              | –            | –            |
| BLK           | B7      | ESC Signal            | 9            | 9            |
| DK GRN        | B8      | A/C Signal            | 0            | 0            |
| –             | B9      | Not used              | –            | –            |
| ORN/BLK       | B10     | Park/Neutral SW Signal| 0            | 8?           |
| –             | B11     | Not used              | –            | –            |
| –             | B12     | Not used              | –            | –            |

---

### C-Side Pins (32-Pin Connector, Rows C1–C16)

| Voltage         |        |                             |       |               |
|-----------------|--------|-----------------------------|-------|---------------|
| **Key “On”**    | **Eng “Run”** | **Circuit**                       | **Pin** | **Wire Color** |
| 0               | –      | Not used                               | C1    | –             |
| 12              | 14     | “EAC Sol” (exact text uncertain)       | C2    | BRN           |
| –               | –      | NOT USEABLE IAC “A” LO                 | C3    | LT GRN /BLK   |
| –               | –      | NOT USEABLE IAC “B” HI                 | C4    | LT GRN /WHT   |
| –               | –      | NOT USEABLE IAC “A” HI                 | C5    | LT BLU /WHT   |
| –               | –      | NOT USEABLE IAC “A” LO                 | C6    | LT BLU /BLK   |
| 12              | 14     | Hi Gear Switch                         | C7    | LT BLU        |
| –               | –      | Not used                               | C8    | –             |
| 0               | 0      | Crank Signal                           | C9    | PPL/WHT       |
| 1.9             | 1.7    | Coolant Temp. Signal                   | C10   | YEL           |
| 4.9             | 2.8    | MAP Signal                             | C11   | LT GRN        |
| –               | –      | Not used                               | C12   | –             |
| 0.6             | 0.6    | TPS Signal                             | C13   | DK BLU        |
| 5.0             | 5      | 5 Volt Reference                       | C14   | GRY           |
| –               | –      | Not used                               | C15   | –             |
| 12              | 14     | Battery 12 Volts                       | C16   | ORN           |

---

### D-Side Pins (32-Pin Connector, Rows D1–D16)

| **Wire Color** | **Pin** | **Circuit**            | **Key “On”** | **Eng “Run”** |
|---------------|---------|------------------------|--------------|--------------|
| BLK/WHT       | D1      | System Ground          | 0            | 0            |
| BLK/RED PPL/BLK|D2      | Sensor Ground          | 0            | 0            |
| –             | D3      | Not used               | –            | –            |
| WHT           | D4      | EST Control            | 0            | 1.0          |
| TAN/BLK       | D5      | EST Bypass             | 0            | 4.76         |
| TAN           | D6      | GND (O₂)               | 0            | –            |
| PPL           | D7      | O₂ Sensor Signal       | 0            | (3)          |
| –             | D8      | Not used               | –            | –            |
| –             | D9      | Not used               | –            | –            |
| –             | D10     | Not used               | –            | –            |
| –             | D11     | Not used               | –            | –            |
| –             | D12     | Not used               | –            | –            |
| –             | D13     | Not used               | –            | –            |
| LT GRN        | D14     | Injector B             | 12           | 14           |
| –             | D15     | Not used               | –            | –            |
| BLU           | D16     | Injector A             | 12           | 14           |

---

## Footnotes (As Listed on Chart)

1. Varies from 0.60 V to battery voltage depending on the position of drive wheels.  
2. Varies with temperature.  
3. 12v first two seconds on 4.3 L & 5.0 L (12 V first 20 seconds on 5.7 L & 7.4 L).  
4. Measured between terminals C13 and A11 +/- 0.05 V.  
5. Used on 4.3L, 5.0L or 5.7 L engine. Wire color may also be yel/black or yellow/red.  
6. Auto downshift control on THM 400 (some models).  
7. Refer to wiring diagram for terminals A11 or D2 for sensor ground.  

(Additional minor notes on the chart mention that voltage readings may differ slightly by model, or depending on battery charge.)

---

## Additional Notes

• Some rows on the original chart are labeled “Not used” or “Not useable,” particularly for certain IAC (Idle Air Control) lines that do not apply to all TBI variants.  
• The “Hi Gear Switch,” “Crank Signal,” and “Coolant Temp. Signal” entries may vary by application.  
• The acronym “EST” stands for Electronic Spark Timing, “ESC” for Electronic Spark Control.  
• “Service Engine Soon” lamp control is also sometimes called the MIL (Malfunction Indicator Lamp).  
• A11 and/or D2 often serve as sensor grounds—consult the exact wiring diagram for your specific application.

---

_Compiled from original “TBI FUEL INJECTION ECM CONNECTOR IDENTIFICATION” chart (1990s Chevrolet TBI). All data above is transcribed as faithfully as possible from the provided image._ 
