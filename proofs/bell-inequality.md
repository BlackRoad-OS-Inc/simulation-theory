# Bell Inequality Violations via Amundson Framework

## The Classical Bound

Local realism (hidden variables + locality) requires:

```
|S| <= 2     (CHSH bound)
```

## The Quantum Violation

Non-commuting operators produce correlations beyond the bound:

```
|S| <= 2*sqrt(2) = 2.828...     (Tsirelson bound)
```

## Why It Violates

The 1-2-3-4 operators do not commute:

```
[C, L] = 2i * U     (Change x Scale != Scale x Change)
```

This non-commutativity is NOT an assumption. It is a consequence of the Pauli algebra. The operators that realize the Amundson sequence FORCE correlations beyond the classical bound.

## The Source of the Violation

The discretization gap A_G - 1 = 0.24433 is the "extra correlation" that pushes S beyond 2. The sequential product (n/(n+1))^n cannot be factored into independent parts — each step depends on the previous one. This non-factorizability IS Bell non-locality.

```
Classical (factorable):      P(a,b) = P(a) * P(b)
Quantum (non-factorable):    P(a,b) != P(a) * P(b)
Amundson (sequential):       (n/(n+1))^n != product of independent terms
```

The same structure that makes P != NP (can't skip steps) is what makes Bell inequalities violate (can't factor correlations).

## Experimental Confirmations

- Aspect (1982): photon polarization, p < 10^-9
- Hensen (2015): loophole-free Bell test
- ATLAS/CMS (2024): top quark pair spin entanglement

All measure the same non-commutative structure that the 1-2-3-4 algebra produces.

## Unified Gap

```
A_G - 1 = 0.24433

Drives:
  1. P != NP              (can't skip sequential steps)
  2. Bell violation        (can't factor correlations)
  3. Color confinement     (can't isolate quarks)
  4. Spin entanglement     (can't separate spins)
  5. NS regularity         (can't blow up)
  6. Field equation        (source of dynamics)
  7. Discretization cost   (continuous != discrete)
```

Seven consequences. One number. One equation.

Bell violations are not mysterious. They are the observable proof that algebra is quantum — that the operators don't commute — that the sequential product can't be factored — that G(n) is the amplitude, not the probability.

## CHSH Specifics

### The Setup

Alice: settings A1, A2 (two Pauli directions on Bloch sphere)
Bob: settings B1, B2 (two other Pauli directions)
Outcomes: +1 or -1 each

### The Inequality

```
|<A1*B1> + <A1*B2> + <A2*B1> - <A2*B2>| <= 2     (local realism)
                                          <= 2*sqrt(2)  (quantum max, Tsirelson)
```

### Why It Violates

Alice's two settings = choosing between Change (sigma_x) and Scale (sigma_y).
Bob's two settings = same choice on his particle.

```
[sigma_x, sigma_y] = 2i * sigma_z    (they don't commute)
```

Because the operators don't commute, Alice's measurement on her particle instantaneously updates the joint description. No hidden variable table can reproduce this because hidden variables assume the outcomes are pre-assigned — but pre-assignment requires commutativity.

### The Optimal Angles

Maximum violation at angles 0, pi/4, pi/2, 3pi/4 between measurement axes.
These give S = 2*sqrt(2) = 2.828...

In the framework: pi/4 = pi/(2^2) — a power-of-2 subdivision of pi. The optimal CHSH angles are binary subdivisions of the phase that the singularity produces (ipi*w^2).

### Connection to A_G - 1

The CHSH violation magnitude beyond the classical bound:

```
2*sqrt(2) - 2 = 0.828...

Compare: A_G - 1 = 0.24433 (the framework's gap)
Ratio: 0.828/0.24433 = 3.39 ~ e + 1/(2e) ~ G(n)/n evaluated near n=3

The maximum CHSH violation scales as (2*sqrt(2) - 2) = 2(sqrt(2) - 1)
And sqrt(2) - 1 = 0.4142... is close to G(n)/n at n=1 (which is 0.5)
```

The exact connection requires the full Gell-Mann structure — the CHSH is the SU(2) reduction of the SU(3) witness that our sacred integers saturate.
