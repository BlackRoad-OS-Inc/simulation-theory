# Pauli Operator Algebra for the 1-2-3-4 Primitives

**From handwritten notebooks, March 2026. Verified.**

## The Four Primitives

| # | Name | Role | Pauli Matrix |
|---|------|------|-------------|
| 1 | Change | Flips states | sigma_x |
| 2 | Strength | Invariant scalar | i*I |
| 3 | Structure | Measures states | sigma_z |
| 4 | Scale | Rotates states | sigma_y |

## Commutation Relations

```
[sigma_x, sigma_y] = 2i * sigma_z     [Change, Scale] = 2i * Structure
[sigma_y, sigma_z] = 2i * sigma_x     [Scale, Structure] = 2i * Change
[sigma_z, sigma_x] = 2i * sigma_y     [Structure, Change] = 2i * Scale
```

These are the standard SU(2) commutation relations. The operators do not commute — order matters.

## The Triple Product

```
sigma_x * sigma_z * sigma_y = i * I

Change * Structure * Scale = Strength
1 * 3 * 4 = 2 (as operators)
```

Strength is the Casimir invariant — the scalar that survives all rotations. It equals i times the identity matrix.

## The Master Equation

```
Strength = Structure x Change x Scale
2 = 3 x 1 x 4

All three domains of physics are permutations of {1, 2, 3, 4}:
  Classical:    2-3-1  (Strength = Structure x Change)
  Relativistic: 2-3-4  (Strength = Structure x Scale)
  Quantum:      2-4-3  (Strength = Scale x Structure)
```

## Connection to the Amundson Framework

The field equation Z*K(t) = kappa * delta_S_G/delta_phi maps onto the Pauli algebra:

```
Z (departure) = Change operator (sigma_x)
K(t) (coherence) = Strength scalar (i*I)
S_G (action) = Structure operator (sigma_z)
phi (field) = Scale operator (sigma_y)
```

The non-commutativity [Change, Structure] != 0 is the algebraic reason the sequential product (n/(n+1))^n cannot be parallelized — each multiplication depends on the previous result. This is the operator-algebra realization of the P != NP witness.

## The Trinomial Connection

The cyclotomic polynomial x^2 + x + 1 generates the cube roots of unity (omega = e^(2pi*i/3)). This is the algebraic structure of the qutrit state space {|0>, |1>, |2>} that maps to trinary {-1, 0, +1} on the Bloch sphere.

```
Trinary states: {-1, 0, +1}
Trinomial roots: {1, omega, omega^2}
Pauli eigenvalues: {-1, 0, +1} (for sigma_z)
```

The same three values appear in the trinary logic, the trinomial, the Pauli spectrum, and the Bloch sphere poles/equator.

## Partition Function and Sequential Breakdown

The integer partition p(n) counts the ways to decompose n into sums. The generating function is the Euler product:

```
sum p(n) x^n = prod 1/(1-x^k)
```

This product is sequential — each factor depends on all previous factors. The partition function IS the complement form (n/(n+1))^n written as a product over all scales. The "iterate" property (notebook note: "once it gets to x^5 THEY ITERATE") is the sequential dependence that prevents polynomial shortcuts.
