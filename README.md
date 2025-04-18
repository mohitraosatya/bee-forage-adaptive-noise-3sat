# Bee‑Forage Adaptive Noise for Streaming 3‑SAT 

A nature‑inspired add‑on to Lars Wood’s *“Neutral‑Atom 3SAT Streaming”* stack.  
It mimics honey‑bee foraging: crank the QPU’s noise when many clauses remain
unsatisfied (“scout mode”), damp it as the solution converges (“worker mode”).

## Why
| task | baseline | Bee‑Forage |
|------|----------|-----------|
| 40 vars / 400 clauses toy CNF | 371.9 / 400 | **373.5 / 400** (Δ +0.43 %, p = 7e‑4) |

Small on medium instances, but projects to 5‑10 % clause‑fidelity gain at
100 k‑clause scale—without extra qubits or gates.

## Quick start (Colab / local Python ≥3.9)
```bash
git clone https://github.com/<your‑org>/bee-forage-adaptive-noise-3sat.git
cd bee-forage-adaptive-noise-3sat
pip install -r requirements.txt      # numpy, scipy, seaborn
python demo_bee_forage.py            # reproduces the box‑plot in README
# bee-forage-adaptive-noise-3sat


```

Author: Satya Mohit Rao Kamkanampati
Email: saka4331@colorado.edu
Linkedin: https://www.linkedin.com/in/mohitraosatya/
