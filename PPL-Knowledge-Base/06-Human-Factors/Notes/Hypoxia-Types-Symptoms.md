---
tags: [ppl, human-factors, medical, acs-HF.I.A]
acs: [HF.I.A]
sources: ["PHAK Ch 17", "FAR 91.211", "AIM 8-1"]
status: checkride-ready
---

# Hypoxia Types & Symptoms

## 1. What is Hypoxia?
**Definition:** A state of oxygen deficiency in the body sufficient to impair function.
*   **The Trap:** It is insidious. You often feel *euphoric* (drunk/happy) before you pass out.
*   **First Symptom:** Deterioration of **Night Vision** (occurs as low as 5,000 ft).

---

## 2. The 4 Types (Memorize "H-H-S-H")

| Type | Mechanism | Common Causes | Checkride Key |
| :--- | :--- | :--- | :--- |
| **Hypoxic** | Insufficient Oxygen available to the lungs. | High Altitude (Thin air). | "Thin Air Hypoxia" |
| **Hypemic** | Blood cannot *transport* the Oxygen. | **Carbon Monoxide**, Anemia, Blood donation. | "Transport Failure" |
| **Stagnant** | Oxygen-rich blood isn't *moving*. | **High G-Forces**, Cold temperatures, Shock. | "Flow Failure" |
| **Histotoxic** | Cells cannot *use* the Oxygen. | **Alcohol**, Narcotics, Cyanide. | "Cellular Poisoning" |

---

## 3. Oxygen Rules (FAR 91.211)
*Memorize these numbers. The DPE will ask.*

| Altitude (MSL) | Requirement |
| :--- | :--- |
| **12,500 - 14,000 ft** | Crew must use O2 if flight time exceeds **30 minutes**. |
| **Above 14,000 ft** | Crew must use O2 **continuously**. |
| **Above 15,000 ft** | **Everyone** (Passengers + Crew) must be **provided** O2. |

> [!TIP] **Passenger Rule**
> Above 15,000 ft, you must *provide* it to passengers, but they are not legally required to *use* it (you can't force them).

---

## 4. Hyperventilation vs. Hypoxia
They feel similar (dizziness, tingling), but the cause is opposite.
*   **Hypoxia:** Lack of Oxygen (O2).
*   **Hyperventilation:** Lack of **Carbon Dioxide (CO2)** caused by rapid breathing (panic/stress).
*   **The Remedy:**
    1.  **Descend** (Fixes Hypoxia).
    2.  **Slow Breathing:** Talk aloud, sing, or breathe into a bag (Fixes Hyperventilation by retaining CO2).

---

## 5. Visualizing the Decision

```mermaid
flowchart TD
    Alt{Cabin Altitude?}
    
    Alt -- < 12,500 --> NoO2[No Legal Requirement \n(Night: Rec > 5,000)]
    Alt -- > 12,500 --> Time{> 30 Mins?}
    
    Time -- Yes --> CrewO2[Crew Must Use O2]
    Time -- No --> NoO2
    
    Alt -- > 14,000 --> CrewAll[Crew: Continuous O2]
    Alt -- > 15,000 --> Pax[Must OFFER to Pax]
```

---

## 6. Oral Exam / Checkride Scenarios

**Q1: "You have the heater on and start feeling drowsy and get a headache. What is it?"**
> **A:** Likely **Hypemic Hypoxia** caused by **Carbon Monoxide** leaking from the heater shroud.
> *   **Action:** Turn off heater, open fresh air vents, use supplemental O2 if available, land ASAP.

**Q2: "Why is it dangerous to fly after donating blood?"**
> **A:** You have reduced your hemoglobin count, causing **Hypemic Hypoxia** even at lower altitudes. It essentially lowers your body's service ceiling.

**Q3: "At what altitude does night vision start to degrade?"**
> **A:** As low as **5,000 ft MSL**. The retina's rods are very oxygen-sensitive. I should use oxygen at night above 5,000 ft if available (AIM recommendation), even if legal up to 12,500 ft.

**Q4: "What is 'Time of Useful Consciousness' (TUC) at 30,000 ft?"**
> **A:** Roughly **1-2 minutes**. It is the time you have to act (put on a mask) before you become mentally incapacitated. (At 45,000 ft, it's 9-15 seconds).

**Q5: "A passenger starts breathing rapidly and says their fingers are tingling. What do you do?"**
> **A:** They are hyperventilating from stress. I will speak to them calmly, ask them to talk to me (forces slower breathing), and descend to a lower altitude to ensure it isn't hypoxia.

---

## References
*   **PHAK Ch 17:** Aeromedical Factors.
*   **FAR 91.211:** Supplemental Oxygen.
*   **AIM 8-1-2:** Effects of Altitude.
