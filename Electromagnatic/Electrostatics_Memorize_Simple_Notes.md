# Electrostatics — Simple Memorize Notes

**Purpose:** This is a short note from your electrostatics handwritten images.  
**Use this first:** Memorize these formulas + meanings, then try past papers.

---

# 1. Electric Potential Difference

Potential difference between two points `a` and `b` is:

```text
V(b) - V(a) = - ∫a^b E · dl
```

Meaning:

> Potential difference tells how much electric potential changes when moving from point `a` to point `b`.

Important:

```text
E = electric field
V = electric potential
 dl = small path element
```

Simple memory:

```text
Potential difference = negative line integral of electric field
```

---

# 2. Relation between Electric Field and Potential

The most important relation is:

```text
E = -∇V
```

Meaning:

> Electric field points in the direction where potential decreases fastest.

Like a hill:

- potential `V` is like height
- electric field points downhill

In one dimension:

```text
E = - dV/dx
```

In 3D:

```text
E = -∇V
```

Memory:

```text
E is negative gradient of V
```

---

# 3. Potential of a Point Charge

For a point charge `q`:

```text
V = (1 / 4πε0) q/r
```

where:

- `q` = charge
- `r` = distance from charge to point
- `ε0` = permittivity of free space

Memory:

```text
Point charge potential ∝ 1/r
```

---

# 4. Potential of Many Discrete Charges

For many point charges:

```text
V(r) = (1 / 4πε0) Σ qi / ri
```

Meaning:

> Total potential is the algebraic sum of potentials due to all charges.

Important:

Potential is scalar, so we add normally. No vector directions needed.

---

# 5. Potential of Continuous Charge Distribution

For continuous charge, replace sum with integral.

General formula:

```text
V(r) = (1 / 4πε0) ∫ dq / |r - r'|
```

where:

- `r` = field point
- `r'` = source point
- `|r - r'|` = distance between source and field point

---

## 5.1 Line Charge

```text
dq = λ dl
```

```text
V = (1 / 4πε0) ∫ λ dl / |r - r'|
```

---

## 5.2 Surface Charge

```text
dq = σ dS
```

```text
V = (1 / 4πε0) ∫ σ dS / |r - r'|
```

---

## 5.3 Volume Charge

```text
dq = ρ dv
```

```text
V = (1 / 4πε0) ∫ ρ dv / |r - r'|
```

Memory:

```text
λ → line charge density
σ → surface charge density
ρ → volume charge density
```

---

# 6. Potential of Charged Spherical Shell

For a uniformly charged spherical shell of radius `R` and total charge `q`:

## Outside shell: `r > R`

```text
V = (1 / 4πε0) q/r
```

Same as point charge at centre.

## Inside shell: `r < R`

```text
V = (1 / 4πε0) q/R
```

Constant.

Important:

```text
Inside spherical shell: E = 0, V = constant
```

Memory:

```text
Outside shell → acts like point charge
Inside shell → constant potential
```

---

# 7. Poisson’s Equation and Laplace Equation

We know:

```text
E = -∇V
```

Gauss’s law differential form:

```text
∇ · E = ρ/ε0
```

Substitute `E = -∇V`:

```text
∇ · (-∇V) = ρ/ε0
```

So:

```text
∇²V = -ρ/ε0
```

This is **Poisson’s equation**.

---

## 7.1 Poisson’s Equation

```text
∇²V = -ρ/ε0
```

Use when charge exists in the region.

Memory:

```text
Charge present → Poisson equation
```

---

## 7.2 Laplace Equation

If there is no charge:

```text
ρ = 0
```

Then Poisson’s equation becomes:

```text
∇²V = 0
```

This is **Laplace equation**.

Memory:

```text
No charge → Laplace equation
```

---

# 8. Electrostatic Potential Energy

Electrostatic energy is the energy stored in a charge system.

---

## 8.1 Work to Move a Test Charge

Force on charge:

```text
F = qE
```

Work done against electric field:

```text
W = -q ∫ E · dl
```

Using potential difference:

```text
W = q[V(b) - V(a)]
```

So potential energy of charge `q` at potential `V` is:

```text
U = qV
```

Memory:

```text
Potential energy = charge × potential
```

---

## 8.2 Energy of Discrete Charge Distribution

For many charges:

```text
W = (1/2) Σ qi Vi
```

Why `1/2`?

> To avoid counting each charge pair twice.

For charge pairs:

```text
W = (1 / 4πε0) Σ(i<j) qi qj / rij
```

Memory:

```text
i < j avoids double counting
```

---

## 8.3 Energy of Continuous Charge Distribution

```text
W = (1/2) ∫ ρ V dv
```

Also:

```text
W = (ε0/2) ∫ E² dv
```

This is very important for past papers.

Memory:

```text
Energy can be found using charge-potential OR field squared
```

---

# 9. Electric Dipole

An electric dipole consists of two equal and opposite charges separated by a small distance.

```text
+q and -q separated by distance s
```

Dipole moment:

```text
p = q s
```

Vector direction:

```text
from -q to +q
```

Memory:

```text
Dipole moment points from negative to positive charge
```

---

# 10. Potential of an Electric Dipole

For a dipole at the origin:

```text
V(r,θ) = (1 / 4πε0) (p cosθ / r²)
```

Vector form:

```text
V(r) = (1 / 4πε0) (p · r̂ / r²)
```

Important:

- `p` = dipole moment
- `θ` = angle between dipole moment and position vector
- dipole potential decreases as `1/r²`

Memory:

```text
Point charge potential ∝ 1/r
Dipole potential ∝ 1/r²
```

---

# 11. Electric Field of a Dipole

From:

```text
E = -∇V
```

Dipole electric field in spherical coordinates:

```text
E = (p / 4πε0 r³) (2cosθ r̂ + sinθ θ̂)
```

Important:

```text
Dipole electric field ∝ 1/r³
```

Memory:

```text
Dipole V → 1/r²
Dipole E → 1/r³
```

---

# 12. Dipole in External Electric Field

Interaction energy of a dipole in an external electric field:

```text
W = -p · E
```

or:

```text
W = -pE cosθ
```

Meaning:

- minimum energy when dipole aligns with electric field
- maximum energy when opposite to electric field

Memory:

```text
Dipole wants to align with E field
```

---

# 13. Separation of Variables

Separation of variables is a method used to solve Laplace equation.

Used when there is symmetry:

- spherical symmetry
- cylindrical symmetry
- planar symmetry

Idea:

```text
V(r,θ) = R(r) P(θ)
```

Meaning:

> We separate the potential into radial part and angular part.

---

# 14. Laplace Equation in Spherical Coordinates

When there is azimuthal symmetry, potential does not depend on `φ`.

So:

```text
∂V/∂φ = 0
```

Then:

```text
V = V(r,θ)
```

General solution:

```text
V(r,θ) = Σ [Al r^l + Bl / r^(l+1)] Pl(cosθ)
```

This is very important.

---

# 15. Legendre Polynomials

First few Legendre polynomials:

```text
P0(cosθ) = 1
```

```text
P1(cosθ) = cosθ
```

```text
P2(cosθ) = (1/2)(3cos²θ - 1)
```

```text
P3(cosθ) = (1/2)(5cos³θ - 3cosθ)
```

Memory:

```text
P0 = 1
P1 = cosθ
P2 = 1/2(3cos²θ - 1)
```

At least memorize first three.

---

# 16. Boundary Conditions for Spherical Laplace Problems

General solution:

```text
V(r,θ) = Σ [Al r^l + Bl/r^(l+1)] Pl(cosθ)
```

## Inside sphere

Potential must be finite at `r = 0`.

So remove the term:

```text
Bl/r^(l+1)
```

Inside solution:

```text
Vinside = Σ Al r^l Pl(cosθ)
```

## Outside sphere

Potential usually goes to zero at infinity.

So remove the term:

```text
Al r^l
```

Outside solution:

```text
Voutside = Σ Bl/r^(l+1) Pl(cosθ)
```

Memory:

```text
Inside → no infinity at r = 0
Outside → V goes to 0 at infinity
```

---

# 17. Orthogonality of Legendre Polynomials

Used to find coefficients.

```text
∫0^π Pl(cosθ) Pl'(cosθ) sinθ dθ = 0, if l ≠ l'
```

```text
∫0^π [Pl(cosθ)]² sinθ dθ = 2/(2l+1)
```

Simple meaning:

> Different Legendre terms do not mix.

This helps find constants in boundary problems.

---

# 18. Common Past Paper Style: Surface Potential on Sphere

If surface potential is given, like:

```text
V(R,θ) = k sin²(θ/2)
```

Use identity:

```text
sin²(θ/2) = (1 - cosθ)/2
```

So:

```text
V(R,θ) = k/2 - (k/2)cosθ
```

Using Legendre polynomials:

```text
P0 = 1
P1 = cosθ
```

So:

```text
V(R,θ) = (k/2)P0 - (k/2)P1
```

Then match coefficients with general solution.

---

# 19. Another Surface Potential Form

If:

```text
V(R,θ) = k cos²(θ/2)
```

Use:

```text
cos²(θ/2) = (1 + cosθ)/2
```

So:

```text
V(R,θ) = k/2 + (k/2)cosθ
```

Then:

```text
V(R,θ) = (k/2)P0 + (k/2)P1
```

Memory:

```text
sin²(θ/2) = (1 - cosθ)/2
cos²(θ/2) = (1 + cosθ)/2
```

---

# 20. Must Memorize Formula Sheet

## Potential difference

```text
V(b) - V(a) = -∫a^b E · dl
```

## Electric field and potential

```text
E = -∇V
```

## Point charge potential

```text
V = (1/4πε0) q/r
```

## Continuous charge potential

```text
V = (1/4πε0) ∫ dq/|r-r'|
```

## Poisson equation

```text
∇²V = -ρ/ε0
```

## Laplace equation

```text
∇²V = 0
```

## Electrostatic energy

```text
W = (1/2)∫ρV dv
```

```text
W = (ε0/2)∫E² dv
```

## Dipole moment

```text
p = qs
```

## Dipole potential

```text
V = (1/4πε0)(p cosθ/r²)
```

## Dipole electric field

```text
E = (p/4πε0r³)(2cosθ r̂ + sinθ θ̂)
```

## Dipole energy

```text
W = -p · E
```

## Spherical Laplace solution

```text
V(r,θ) = Σ [Al r^l + Bl/r^(l+1)] Pl(cosθ)
```

---

# 21. What to Memorize First

If you feel this chapter is hard, memorize in this order:

1. `E = -∇V`
2. `V = (1/4πε0)q/r`
3. `V = (1/4πε0)∫dq/|r-r'|`
4. `∇²V = -ρ/ε0`
5. `∇²V = 0`
6. `W = (1/2)∫ρVdv`
7. `W = (ε0/2)∫E²dv`
8. `p = qs`
9. `Vdipole = (1/4πε0)(p cosθ/r²)`
10. `Wdipole = -p · E`
11. spherical Laplace general solution
12. `P0 = 1`, `P1 = cosθ`, `P2 = 1/2(3cos²θ - 1)`

---

# 22. Very Simple Concept Summary

- Potential `V` is a scalar.
- Electric field `E` is a vector.
- Electric field comes from change of potential.
- `E = -∇V` means field points from high potential to low potential.
- Poisson equation is used when charge exists.
- Laplace equation is used when no charge exists.
- Electrostatic energy can be calculated from charges or from electric field.
- A dipole is `+q` and `-q` separated by small distance.
- Dipole moment points from negative charge to positive charge.
- Separation of variables helps solve Laplace equation in symmetric problems.

---

# 23. Small Sinhala-style Memory Help

- **Potential difference**: point දෙකක් අතර potential වෙනස.
- **E = -∇V**: electric field එක potential අඩු වෙන direction එකට යනවා.
- **Poisson equation**: charge තියෙන region එකට.
- **Laplace equation**: charge නැති region එකට.
- **Dipole**: `+q` සහ `-q` charges දෙකක් පොඩි distance එකකින් වෙන් වෙලා තියෙන system එක.
- **Dipole moment**: negative charge එකෙන් positive charge එකට direction.
- **Separation of variables**: Laplace equation solve කරන්න symmetry තියෙන විට භාවිතා කරන method එක.

---

## End of memorize notes
