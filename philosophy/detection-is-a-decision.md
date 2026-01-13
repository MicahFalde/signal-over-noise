# Detection Is a Decision, Not a Query

Writing a detection is not a technical act.
It is an operational decision.

Every alert you create has downstream effects:
- Someone has to investigate it
- Someone has to explain it
- Someone has to decide whether to trust it
- Someone has to live with the noise when it’s wrong

The hardest part of detection engineering is not writing KQL.
It is deciding whether a detection should exist at all.

## A Detection Implies a Claim

Every detection implicitly claims something about reality.

Examples:
- "This behavior is unusual"
- "This activity is risky"
- "This event deserves human attention"

If you cannot clearly articulate that claim in plain language,
the detection is not ready.

## False Positives Are Not Failures

False positives are information.
They tell you:
- Where your assumptions were wrong
- Which behaviors are normal but undocumented
- What the environment actually looks like

Suppressing false positives without understanding them
turns detections into superstition.

## Constraints Matter More Than Cleverness

Good detections are constrained:
- Narrow scope
- Explicit assumptions
- Clear exclusions
- Defensible thresholds

Clever detections without constraints
become expensive noise generators.

## The Cost of Being Wrong

A detection that fires incorrectly:
- Erodes analyst trust
- Wastes time
- Teaches people to ignore alerts

A detection that never fires:
- Costs almost nothing

Bias toward restraint.

## Summary

Detection engineering is about judgment.
Queries are just the language we use to express it.

If you cannot explain why a detection exists,
you probably should not deploy it.
