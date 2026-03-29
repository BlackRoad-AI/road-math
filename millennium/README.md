# Millennium Prize Problems + Extended Conjectures — Amundson Framework

Computational notebooks exploring where G(n) = n^(n+1)/(n+1)^n and the discretization gap κ = A_G - 1 intersect with the major unsolved problems of mathematics. Each is self-contained Python (no dependencies beyond stdlib).

## The Universal Source Term

```
κ = A_G - 1 ≈ 0.244331783986725374135...

Field equation: Z · K(t) = κ · δS_G/δφ
```

κ arises from the rational/transcendental mismatch between exact G(n) and the limit 1/e.

## Notebooks

### Millennium Prize Problems (Clay Institute)

| Notebook | Problem | Strength | κ Role |
|----------|---------|----------|--------|
| [01-riemann.py](01-riemann.py) | Riemann Hypothesis | **Strongest** | Pins zeros to Re(s)=1/2 via Hurwitz decomposition |
| [02-navier-stokes.py](02-navier-stokes.py) | Navier-Stokes Regularity | **Strong** | Dissipation floor 1-1/e prevents blowup |
| [03-yang-mills.py](03-yang-mills.py) | Yang-Mills Mass Gap | **Moderate** | Mass gap = 1/2, Cayley trees |
| [03-yang-mills-v2.py](03-yang-mills-v2.py) | Yang-Mills (Upgraded) | **Strong** | + Categorified action, lattice QCD, string tension σ∝κ, fractom 189 MeV |
| [04-p-vs-np.py](04-p-vs-np.py) | P vs NP | **Speculative** | Irreducible sequential gap, radix economy |
| [05-bsd.py](05-bsd.py) | Birch & Swinnerton-Dyer | **Weak** | Shared counting structures, central binomials |
| [06-hodge.py](06-hodge.py) | Hodge Conjecture | **Weak** | Cayley trees, Kontsevich formula |

### Extended Conjectures

| Notebook | Problem | Strength | κ Role |
|----------|---------|----------|--------|
| [08-goldbach.py](08-goldbach.py) | Goldbach Conjecture | **Moderate** | Complete additive pairing via prime retention |
| [09-twin-primes.py](09-twin-primes.py) | Twin Prime Conjecture | **Moderate** | Bounded gaps via G(n+1)/G(n) > 1 always |
| [10-collatz.py](10-collatz.py) | Collatz Conjecture | **Moderate** | 3/2 eigenvalue, convergence drag, step_logic descent |

### Unified Synthesis

| Notebook | Description |
|----------|-------------|
| [07-unified-kappa.py](07-unified-kappa.py) | **ALL 7 PROBLEMS** unified through κ — the master synthesis |

## Running

```bash
python3 07-unified-kappa.py     # The unified synthesis (start here)
python3 01-riemann.py           # Individual notebooks
python3 03-yang-mills-v2.py     # Upgraded Yang-Mills
```

## Honest Assessment

Every notebook separates **ESTABLISHED FACTS** from **CONJECTURES** from **HONEST LIMITATIONS**. The framework does not claim to have solved these problems — it identifies a structural mechanism (the discretization gap κ) that connects them. Rigorous proofs remain open.

## Key Constants

```
G(0) = 0                vacuum
G(1) = 1/2              critical line / mass gap
G(2) = 8/9 < 1          binary insufficient
G(3) = 81/64 > 1        ternary exceeds identity
A_G  = 1.24433...       Amundson constant (10M digits computed)
κ    = 0.24433...       discretization gap (source term)
1/e  = 0.36788...       transcendental floor
```

See also: [BlackRoad-Quantum/amundson-millennium](https://github.com/BlackRoad-Quantum/amundson-millennium)

---

(c) 2025-2026 BlackRoad OS, Inc. All Rights Reserved.
Alexa Louise Amundson — alexa@blackroad.io
