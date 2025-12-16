---
tags: [human-factors, decision-making, acs-I.F]
acs_code: I.F.K.2
---

# DECIDE Model (In-Flight Logic)

## Definition
A continuous loop process for making decisions while the flight is in progress.

## Why It Matters
When things change (engine roughness, unexpected weather), you need a structured way to react so you don't freeze or act impulsively.

## The Acronym

1.  **D**etect: The pilot perceives that a change has occurred. ("The engine sounds weird.")
2.  **E**stimate: The need to counter or react to the change. ("It's losing RPM. If this continues, I can't hold altitude.")
3.  **C**hoose: A desirable outcome. ("I need to land soon.")
4.  **I**dentify: Actions to control the change. ("I will divert to the airport 5 miles away.")
5.  **D**o: The necessary action. (Turn, call ATC, descend.)
6.  **E**valuate: The effect of the action. ("Am I making the field? Is the engine stable?")

## Common Mistakes
- **Skipping "Estimate":** Jumping straight to action without understanding the severity.
- **Skipping "Evaluate":** Doing something and assuming it worked without checking.
- **freezing:** Getting stuck at "Detect" and not moving forward.

## Checkride Angle
- **Scenario:** "You are flying cross-country and notice your oil pressure dropping slowly. Walk me through the DECIDE model."
- **Answer:**
    - **D:** I see the gauge dropping.
    - **E:** It could be an oil leak; engine failure is possible in 10-15 mins.
    - **C:** I want to be on the ground before it quits.
    - **I:** Nearest airport is Smith Field, 10 mins away.
    - **D:** Turn to Smith Field, climb for altitude, monitor engine.
    - **E:** Pressure is still dropping, but I have the field in sight. Plan is working.

## Diagram: The Loop

```mermaid
graph Circular
    D[Detect Change] --> E[Estimate Significance]
    E --> C[Choose Outcome]
    C --> I[Identify Actions]
    I --> Do[Do Action]
    Do --> Eval[Evaluate Effect]
    Eval --> D
```

## Study Drills
1. How is DECIDE different from PAVE? (DECIDE is usually operational/in-flight; PAVE is pre-flight planning).
2. What is the danger of failing to "Evaluate"?

## References
- PHAK Chapter 2
