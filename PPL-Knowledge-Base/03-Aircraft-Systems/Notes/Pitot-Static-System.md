---
tags: [ppl, systems, instruments, acs-S.V.A]
acs: [S.V.A]
sources: ["PHAK Ch 8", "POH Section 7"]
status: checkride-ready
---

# Pitot-Static System

## 1. The Basics
The system relies on two types of air pressure to drive the flight instruments:
1.  **Pitot Pressure (Ram Air):** Impact air pressure captured by the tube on the wing. (Only affects Airspeed).
2.  **Static Pressure:** Ambient atmospheric pressure captured by the flush port on the fuselage. (Affects All Three).

### The Instruments
*   **Airspeed Indicator (ASI):** Compares Ram Air minus Static Air.
*   **Altimeter:** Measures Static Air only (barometer).
*   **Vertical Speed Indicator (VSI):** Measures the *rate of change* of Static Air (calibrated leak).

---

## 2. Failure Modes (The "Killer" Table)
*Memorize this behavior.*

| Failure | ASI Indication | Altimeter | VSI |
| :--- | :--- | :--- | :--- |
| **Blocked Pitot** (Open Drain) | **Drops to Zero** (Bleeds out drain) | Normal | Normal |
| **Blocked Pitot** (Blocked Drain) | **Acts like Altimeter** (Increases in climb) | Normal | Normal |
| **Blocked Static Port** | **Inaccurate** (Reads low in climb, high in descent) | **Frozen** (Stuck at blocked altitude) | **Frozen** at Zero |

> [!WARNING] **The Dangerous ASI Failure**
> If the **Pitot and Drain** are blocked (e.g., ice), the air is trapped inside.
> *   **Climb:** The static pressure outside decreases, but the trapped pitot pressure stays high. The diaphragm expands. **ASI indicates FAST.**
> *   **Descent:** **ASI indicates SLOW.**
> *   *Danger:* You might stall the plane thinking you are flying fast, or overspeed thinking you are slow.

---

## 3. Alternate Static Source
If the primary static port blocks (ice, tape, bug), pull the **Alternate Static Source** knob.
*   **Source:** Takes air from *inside* the cabin.
*   **Pressure:** Cabin pressure is usually **lower** than outside pressure (Venturi effect of fuselage).
*   **Indications:**
    *   **Altimeter:** Reads slightly **HIGH**.
    *   **ASI:** Reads slightly **FAST**.
    *   **VSI:** Momentarily shows a **CLIMB**, then stabilizes.

---

## 4. Visualizing Failures

```mermaid
flowchart TD
    Start[Instrument Error Detected] --> CheckASI{ASI erratic?}
    
    CheckASI -- Yes --> CheckAlt{Altimeter/VSI Normal?}
    CheckASI -- No --> CheckStatic[Suspect Static Blockage]
    
    CheckAlt -- Yes --> PitotBlock[Pitot Blockage]
    CheckAlt -- No --> StaticBlock[Static Blockage]
    
    PitotBlock --> Heat[Turn on Pitot Heat]
    StaticBlock --> AltStatic[Activate Alternate Static]
    
    AltStatic --> Emergency[Break VSI Glass \n(If no Alt Static)]
```

---

## 5. Oral Exam / Checkride Scenarios

**Q1: "You are climbing at Vy, but your airspeed indicator starts increasing to the red line. What is happening?"**
> **A:** My Pitot tube and drain hole are likely blocked (ice). The trapped high pressure makes the ASI act like an altimeter. I must rely on pitch and power settings to maintain safe flight.

**Q2: "Your static port is blocked and you don't have an alternate static source. What can you do?"**
> **A:** I can break the glass face of the **VSI** (Vertical Speed Indicator). It is the least critical instrument. This vents the system to cabin air (similar to alternate static).

**Q3: "If you switch to Alternate Static, why does the Altimeter read high?"**
> **A:** The pressure inside the cabin is slightly lower than outside. The altimeter interprets lower pressure as higher altitude.

**Q4: "How do modern glass cockpits (G1000) detect these errors?"**
> **A:** They use an **ADC (Air Data Computer)**. If the pitot/static inputs fail, the ADC will fail, and you will see big Red X's over the airspeed and altitude tapes. You revert to the standby "steam" gauges.

**Q5: "Why is the Pitot Heat switch typically OFF on the ground?"**
> **A:** The heating element is very hot and relies on airflow for cooling. Without airflow, it can burn out or damage the pitot tube cover if left on too long.

---

## References
*   **PHAK Ch 8:** Flight Instruments.
*   **POH Section 7:** Airplane Systems.