---
tags: [ppl, nav, avionics, acs-PA.VI.A]
acs: [PA.VI.A]
sources: ["PHAK Ch 16", "AIM 1-1"]
status: checkride-ready
---

# VOR & GPS Basics

## 1. VOR (Very High Frequency Omnidirectional Range)

### How it Works
The VOR ground station emits two signals:
1.  **Reference Phase:** Omnidirectional (pulses everywhere at once).
2.  **Variable Phase:** Rotating beam (sweeps like a lighthouse).
The aircraft receiver compares the **phase difference** between the two. If the difference is 90 degrees, you are on the 090 radial.

### Service Volumes (Standard Service Volume - SSV)
*Know these distances for the oral.*

| Class | Altitude (AGL) | Range (NM) | Use Case |
| :--- | :--- | :--- | :--- |
| **Terminal (T)** | 1,000 - 12,000 ft | 25 NM | Local airport navigation |
| **Low (L)** | 1,000 - 18,000 ft | 40 NM | Low altitude airways (Victor) |
| **High (H)** | 1,000 - 14,500 ft | 40 NM | Jet Routes (high altitude) |
| | 14,500 - 60,000 ft | 100-130 NM | |

### VOR Checks & Limits
*Required every **30 days** for IFR flight. Good practice for VFR.*

| Check Type | Max Error | Note |
| :--- | :--- | :--- |
| **VOT (Test Facility)** | +/- 4° | Tune VOT freq. Center needle. Should read **180 TO** or **360 FROM**. |
| **Ground Checkpoint** | +/- 4° | Designated spot on airport taxiway. |
| **Airborne Checkpoint** | +/- 6° | Designated landmark over a known radial. |
| **Dual VOR Check** | +/- 4° | Compare VOR 1 vs VOR 2 against each other. |

> [!WARNING] **Reverse Sensing**
> If you are flying **TO** a station but have a **FROM** indication set (e.g., flying inbound on the 180 radial but OBS is set to 180 instead of 360), the needle will move **opposite** to your turn.
> *   **Rule:** Always set the OBS to your *intended course*.

---

## 2. GPS (Global Positioning System)

### The Constellation
*   **24+ Satellites.**
*   **Trilateration:** The receiver measures the time it takes for a signal to arrive from 3 satellites to calculate a 2D position (Lat/Long).
*   **3D Position:** Requires **4 Satellites** (adds Altitude).

### RAIM (Receiver Autonomous Integrity Monitoring)
*   **What is it?** The GPS receiver "self-checks" the accuracy of the signal. It needs to know if a satellite is lying.
*   **Requirements:**
    *   **5 Satellites** needed for Fault Detection.
    *   **4 Satellites + Baro-Aiding** (Barometric Altimeter input) can also provide RAIM.
*   **Result:** If RAIM fails, you have no assurance of accuracy. You must not use GPS for navigation (especially IFR approaches).

### WAAS (Wide Area Augmentation System)
*   **Concept:** Ground stations measure GPS errors and beam corrections up to a master satellite, which broadcasts a "correction signal" back to your plane.
*   **Benefit:** Improves accuracy from ~15 meters to <3 meters. Allows **LPV Approaches** (Vertical guidance similar to an ILS).

### Database Currency
*   **Cycle:** Updates every **28 days**.
*   **Rule:**
    *   **IFR:** Must be current to use for navigation.
    *   **VFR:** Legally, you can use an expired database for situational awareness, but you must verify waypoints with current charts. (Best practice: Update it!).

---

## 3. Visualizing RAIM Logic

```mermaid
flowchart TD
    Start[GPS Start Up] --> SatSearch{Satellites in View?}
    
    SatSearch -- < 4 Sats --> NoPos[No Position Lock]
    SatSearch -- 4 Sats --> 3DPos[3D Position (No Integrity)]
    
    SatSearch -- 5 Sats (or 4+Baro) --> CheckRAIM{RAIM Check}
    
    CheckRAIM -- Integrity Good --> Nav[Navigation Allowed]
    CheckRAIM -- Fault Detected --> Alert[MSG: RAIM FAILURE]
    Alert --> NoNav[Do Not Use GPS]
```

---

## 4. Oral Exam / Checkride Scenarios

**Q1: "You tune a VOR and the needle is erratic. You are 50 miles away at 2,000 ft. Why?"
> **A:** I am likely outside the **Service Volume**. A Low or High VOR is reliable to 40 NM at that altitude. At 50 NM, the signal is weak or blocked by line-of-sight.

**Q2: "What is the 'Cone of Confusion'?"
> **A:** The area directly above the VOR station where the signal is scrambled. The TO/FROM flag will flicker, and the CDI will swing fully. Once past it, the flag flips to distinct FROM.

**Q3: "How do you verify your GPS is providing accurate information?"
> **A:** I check the status page for **RAIM availability** and look for any integrity error messages. I also cross-check GPS waypoints against VORs or visual landmarks.

**Q4: "Can you use a VOR check found in the back of the chart supplement (A/FD)?"
> **A:** Yes. These are published Ground or Airborne checkpoints. I would taxi to the specific spot or fly over the landmark at the specific altitude and verify the error is within limits (+/- 4° ground, +/- 6° air).

**Q5: "Does your aircraft have WAAS? How do you know?"
> **A:** (Know your specific avionics). If yes, I can fly LPV approaches. If no (e.g., standard G430 non-W), I am limited to LNAV minimums and must check RAIM prediction before flight.

---

## References
*   **PHAK Ch 16:** Navigation.
*   **AIM 1-1:** Navigation Aids.