# Signal Over Noise

Detection engineering and SOC decision-making notes focused on reducing alert fatigue
and increasing signal quality.

This repository documents how security detections are designed, reviewed, tuned,
and sometimes rejected in real production environments.

These are not copy-paste rules.

Each detection or analysis aims to answer:
- Why this detection should exist
- What assumptions it relies on
- What it will miss
- Common false positives
- How it should be tuned or constrained

Topics include:
- Detection engineering principles
- KQL-based detections
- Alert postmortems and reviews
- MITRE ATT&CK mapping (and its limitations)
- False positives as a signal
- Tradeoffs between coverage, fidelity, and operational cost

If you are looking for perfect coverage, universal alerts, or vendor-driven examples,
this repository is probably not for you.
