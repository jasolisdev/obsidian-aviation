---
tags: [ppl, weather, human-factors, concept]
acs: [W.III.A]
sources: ["PHAK Ch 2", "PHAK Ch 12"]
status: seed
---

# Weather Decision-Making Flow

## What it is
This is the structured process of identifying hazards, assessing risk, and deciding (DECIDE model) while considering personal minimums, aircraft capabilities, and weather data.

## Why it matters
A credible go/no-go briefing proves the DPE you can instrument the tools (METAR, TAF, radar) into safe choices rather than rely on wishful thinking.

## How it shows up on a checkride
- **Q:** “How do you use the DECIDE model with weather?” **A:** Detect hazards (low ceilings), Estimate risks (IMC), Choose options (delay/diversion), Identify controls (alternate plan), Do the plan, Evaluate results.
- **Q:** “What personal minimums guide your weather decisions?” **A:** Fuel reserves, ceiling/visibility minimums tailored to your experience and the airplane’s capabilities.
- **Q:** “When would you abort a flight after departure?” **A:** Sudden loss of visibility, unexpected icing, or a sigmet/TAF update showing lowering ceilings below your minimums.

## Common mistakes
- Treating weather data as static; keep re-evaluating en route as TAFs and radar updates change.
- Ignoring personal minimums for the sake of meeting a schedule.
- Skipping the step of identifying mitigations (e.g., fly around convective cells or divert to nearest airport).

## Diagram
```mermaid
flowchart TD
    Detect[Detect hazard (METAR/TAF)] --> Estimate[Estimate risk level]
    Estimate --> Choose[Choose plan (delay, route change, cancel)]
    Choose --> Identify[Identify mitigations (alternate airfields, fuel)]
    Identify --> Do[Do the mitigation (file IFR, divert)]
    Do --> Evaluate[Evaluate outcome & log lesson]
    Personal[Personal minimums] --> Estimate
```

## ACS Tags
- Area of Operation: Weather Decision Making (W.III)
- Task(s): W.III.A Apply DECIDE to weather hazards and personal minimums.
- Knowledge elements: Hazard recognition, risk estimation, mitigation techniques.

## References
- PHAK Ch 2 Aeronautical decision-making (DECIDE, PAVE, personal minimums).
- PHAK Ch 12 Weather theory (hazard identification, stability, icing).
