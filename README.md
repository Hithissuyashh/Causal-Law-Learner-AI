Causal Law Learner AI
An AI System That Learns Causes Instead of Patterns
1. Project Overview

This project introduces a fundamentally different AI paradigm:
an explicit causal reasoning system that discovers causal laws instead of fitting statistical patterns.

The system:

Learns from interventions

Tests causal invariance

Refuses to predict when causality is ambiguous

This directly addresses the failure demonstrated in Project 1.

2. Core Principle

Prediction must be earned through identifiable causality.

Unlike machine learning models:

No loss minimization

No backpropagation

No black-box function approximation

Only explicit hypotheses + invariance testing.

3. Domain Choice: Physics

Physics is used because:

Causal mechanisms are well-defined

Interventions are meaningful

Ground truth is interpretable

The system starts in 1D motion, then extends to full 3D physics.

4. Learning Pipeline
Step 1 — Observation

Input: time-series data (t, x, y, z)

Compute first and second derivatives

Step 2 — Hypothesis Generation

Examples:

Constant velocity

Constant acceleration

Independent axis acceleration

Joint vector acceleration

Step 3 — Intervention

Modify acceleration mechanisms

Regenerate worlds

Observe invariance

Step 4 — Causal Decision

Possible outcomes:

law_found

causal_equivalence

refused

Prediction is allowed only if exactly one law survives.

5. Key Techniques Used

Finite hypothesis spaces

Causal invariance principle

Do-interventions

Physics-based generative worlds

Prediction gating

Refusal as a valid outcome

6. Major Results

Correctly identifies causal laws in 1D and 3D systems

Detects causal equivalence and refuses prediction

Works on synthetic and real motion data

Never hallucinates a prediction

7. Web Interface (FastAPI)

The project includes a UI where users can:

Upload CSV motion data

Trigger causal discovery

Receive explanations

See whether prediction is allowed

Endpoints:

/ → UI

/analyze → causal discovery

/query → explain / predict / what-if

8. Project Structure
causal_law_learner_ai/
│
├── agent/                  # Observer, hypothesis, causal tester
├── world/                  # 1D & 3D physics worlds
├── experiments/            # Sanity checks & real data tests
├── interface/              # Query engine
├── ui/                     # HTML + CSS UI
├── app.py                  # FastAPI backend
└── README.md

9. Key Contribution

This project demonstrates that:

Causal intelligence is achievable without ML or LLMs

Refusal is a feature, not a failure

Invariance under intervention is sufficient for learning laws

10. Relationship Between the Two Projects
Project	Purpose
Project 1	Proves that pattern-based AI hallucinates causality
Project 2	Demonstrates a viable causal alternative

Together, they form a complete research narrative.

11. Final Statement

These projects show that the future of reliable AI lies not in scaling patterns, but in respecting causality.
