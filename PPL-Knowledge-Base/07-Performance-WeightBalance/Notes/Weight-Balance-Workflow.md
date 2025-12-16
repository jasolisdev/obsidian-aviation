---
tags: [performance, weight-balance, definitions, acs-PA.I]
acs_code: PA.I.C
---

# Weight & Balance Definitions

## Key Terms

1.  **Datum:** An imaginary vertical plane from which all horizontal distances are measured. (Usually the firewall or propeller tip).
2.  **Arm:** The horizontal distance (in inches) from the Datum to an item (seat, fuel tank).
    - **Aft** of datum = Positive (+)
    - **Forward** of datum = Negative (-)
3.  **Moment:** The turning force. **Weight × Arm = Moment**.
4.  **Center of Gravity (CG):** The point where the aircraft would balance if suspended.
    - **Total Moment / Total Weight = CG**.
5.  **Useful Load:** Max Ramp Weight minus Basic Empty Weight. (What you can put in: Pilot + Passengers + Fuel + Bags).

## The Math
$$Weight \times Arm = Moment$$
$$Total Moment \div Total Weight = CG$$

## Checkride Angle
- **Question:** "Where is the Datum on your plane?"
- **Answer:** (Know your POH). E.g., "The firewall."
- **Question:** "What is 'Basic Empty Weight'?"
- **Answer:** The standard empty weight plus optional equipment and *unusable* fuel/oil.

## Diagram: The Seesaw

```mermaid
graph LR
    Datum[Datum (0 inches)]
    
    subgraph Calculation
    W1[Pilot Weight] -->|x Arm| M1[Pilot Moment]
    W2[Fuel Weight] -->|x Arm| M2[Fuel Moment]
    W3[Bags Weight] -->|x Arm| M3[Bags Moment]
    end
    
    M1 & M2 & M3 --> SumM[Total Moment]
    W1 & W2 & W3 --> SumW[Total Weight]
    
    SumM -->|Divide by SumW| CG[Center of Gravity]
```

## Study Drills
1. If you add weight *aft* of the CG, what happens to the CG? (It moves aft).
2. What is the formula for Moment? (Weight x Arm).

## References
- PHAK Chapter 9