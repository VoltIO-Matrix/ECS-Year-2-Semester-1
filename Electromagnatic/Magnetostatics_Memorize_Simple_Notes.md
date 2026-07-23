# Magnetostatics — Very Simple Memorize Notes

**Purpose:** Small note from your magnetostatics lecture images.  
**How to use:** Memorize this first, then do past papers.

---

# 1. What is magnetostatics?

**Magnetostatics** studies magnetic fields produced by **steady currents**.

Steady current means:

```text
∂I/∂t = 0
```

Simple idea:

```text
stationary charges → electric field
moving charges / current → magnetic field
```

---

# 2. Magnetic force on moving charge

A moving charge in a magnetic field feels force.

```text
F = q(v × B)
```

where:

- `q` = charge
- `v` = velocity
- `B` = magnetic flux density / magnetic field

Direction is given by the **right-hand rule**.

Memory:

```text
Magnetic force is perpendicular to v and B
```

---

# 3. Force on current element

For a small current element:

```text
dF = I(dl × B)
```

For a full wire:

```text
F = I ∫ dl × B
```

If wire is straight and field is uniform:

```text
F = I L × B
```

Magnitude:

```text
F = ILB sinθ
```

---

# 4. Current density types

## 4.1 Line current

Used for thin wire.

Symbol:

```text
I
```

Unit:

```text
A
```

Definition:

```text
I = dq/dt
```

---

## 4.2 Surface current density

Used when current flows on a surface.

Symbol:

```text
K
```

Unit:

```text
A/m
```

Formula:

```text
K = dI/dl⊥
```

If surface charge density `σ` moves with velocity `v`:

```text
K = σv
```

---

## 4.3 Volume current density

Used when current flows through volume.

Symbol:

```text
J
```

Unit:

```text
A/m²
```

Formula:

```text
J = dI/da⊥
```

If volume charge density `ρ` moves with velocity `v`:

```text
J = ρv
```

Memory:

```text
I → wire
K → surface
J → volume
```

---

# 5. Continuity equation

Charge conservation gives:

```text
∂ρ/∂t + ∇ · J = 0
```

For steady current:

```text
∂ρ/∂t = 0
```

So:

```text
∇ · J = 0
```

Meaning:

> In steady current, current does not start or stop inside the material.

Memory:

```text
steady current → divergence of J is zero
```

---

# 6. Biot-Savart law

Biot-Savart law gives magnetic field due to current.

For a small current element:

```text
dB = (μ0/4π) I (dl × r) / r³
```

or:

```text
dB = (μ0/4π) I (dl × r̂) / r²
```

For a full wire:

```text
B = (μ0/4π) ∫ I(dl × r) / r³
```

Memory:

```text
Biot-Savart is like Coulomb law for magnetism
```

---

# 7. Biot-Savart for different current types

## Line current

```text
B = (μ0/4π) ∫ I(dl × r) / r³
```

## Surface current

```text
B = (μ0/4π) ∫ (K × r) / r³ da
```

## Volume current

```text
B = (μ0/4π) ∫ (J × r) / r³ dv
```

---

# 8. Magnetic field intensity H

Relation between `B` and `H`:

```text
B = μH
```

In free space:

```text
B = μ0H
```

where:

```text
μ = μ0 μr
```

---

# 9. Important magnetic field results

## 9.1 Infinite long straight wire

At distance `d` from wire:

```text
B = μ0I / (2πd)
```

Direction: circular around wire by right-hand rule.

Memory:

```text
Long wire B ∝ 1/r
```

---

## 9.2 Circular loop on axis

For loop radius `R`, current `I`, at distance `z` on axis:

```text
B = μ0 I R² / [2(R² + z²)^(3/2)]
```

At centre, `z = 0`:

```text
B = μ0I / (2R)
```

---

## 9.3 Long solid cylinder with uniform current density J

Cylinder radius = `R`.

### Inside cylinder: `r < R`

```text
B = μ0 J r / 2
```

### Outside cylinder: `r > R`

```text
B = μ0 J R² / (2r)
```

If total current is `I = JπR²`, outside becomes:

```text
B = μ0I / (2πr)
```

Memory:

```text
inside cylinder → B ∝ r
outside cylinder → B ∝ 1/r
```

---

## 9.4 Ideal solenoid

For ideal solenoid with `n` turns per unit length:

Inside:

```text
B = μ0 n I
```

Outside:

```text
B ≈ 0
```

Memory:

```text
solenoid inside field is nearly uniform
```

---

# 10. Ampere’s law

Integral form:

```text
∮ B · dl = μ0 Ienc
```

Using `H`:

```text
∮ H · dl = Ienc
```

Differential form:

```text
∇ × B = μ0 J
```

or:

```text
∇ × H = J
```

Meaning:

> Current creates circulating magnetic field.

Memory:

```text
Gauss law counts charge.
Ampere law counts current.
```

---

# 11. Divergence of magnetic field

```text
∇ · B = 0
```

Meaning:

> Magnetic field lines do not start or end.

So:

```text
magnetic monopoles do not exist
```

Memory:

```text
B field lines are closed loops
```

---

# 12. Magnetic force between two parallel wires

Two long parallel wires separated by distance `d`:

Force per unit length:

```text
F/L = μ0 I1 I2 / (2πd)
```

Important:

```text
same current direction → attraction
opposite current direction → repulsion
```

---

# 13. Time-varying fields idea

For steady cases:

```text
electrostatics and magnetostatics can be studied separately
```

For time-varying cases:

```text
changing B creates E
changing E creates B
```

This leads to electromagnetism.

---

# 14. Faraday’s law

Changing magnetic flux induces emf.

Magnetic flux:

```text
ΦB = ∫S B · dS
```

Faraday’s law integral form:

```text
∮ E · dl = - dΦB/dt
```

Differential form:

```text
∇ × E = - ∂B/∂t
```

Meaning:

> Changing magnetic field creates curling electric field.

Negative sign means induced emf opposes the change. This is Lenz’s law.

---

# 15. Maxwell’s equations

These are the four main equations of electromagnetism.

## 15.1 Gauss’s law for electricity

```text
∇ · E = ρ/ε0
```

Meaning:

> Charge creates electric field divergence.

---

## 15.2 Gauss’s law for magnetism

```text
∇ · B = 0
```

Meaning:

> No magnetic monopoles.

---

## 15.3 Faraday’s law

```text
∇ × E = -∂B/∂t
```

Meaning:

> Changing magnetic field creates electric field.

---

## 15.4 Ampere-Maxwell law

```text
∇ × B = μ0J + μ0ε0 ∂E/∂t
```

Meaning:

> Current and changing electric field create magnetic field.

---

# 16. Poynting vector

Poynting vector gives energy flow of electromagnetic field.

```text
S = (1/μ0)(E × B)
```

Meaning:

> EM energy flows in the direction of `E × B`.

Power through a surface:

```text
P = ∫ S · dA
```

Memory:

```text
Poynting vector = power per unit area
```

---

# 17. Coaxial cable important result

For coaxial cable with inner radius `a`, outer radius `b`, current `I`, voltage `V`:

Between conductors `a < r < b`:

```text
E = V / [r ln(b/a)] r̂
```

```text
B = μ0I / (2πr) φ̂
```

Poynting vector:

```text
S = (1/μ0)(E × B)
```

Power transmitted:

```text
P = VI
```

If resistor is `R`:

```text
P = V²/R
```

---

# 18. Must memorize formula sheet

```text
F = q(v × B)
```

```text
dF = I(dl × B)
```

```text
I = dq/dt
```

```text
K = σv
```

```text
J = ρv
```

```text
∂ρ/∂t + ∇ · J = 0
```

```text
steady current → ∇ · J = 0
```

```text
dB = (μ0/4π) I(dl × r)/r³
```

```text
B long wire = μ0I/(2πr)
```

```text
B loop centre = μ0I/(2R)
```

```text
B solenoid = μ0nI
```

```text
∮ B · dl = μ0Ienc
```

```text
∇ × B = μ0J
```

```text
∇ · B = 0
```

```text
∮ E · dl = -dΦB/dt
```

```text
∇ × E = -∂B/∂t
```

```text
S = (E × B)/μ0
```

---

# 19. What to memorize first if this is hard

Memorize only these 8 first:

```text
F = q(v × B)
```

```text
dF = I(dl × B)
```

```text
dB = (μ0/4π) I(dl × r)/r³
```

```text
B = μ0I/(2πr)
```

```text
∮B · dl = μ0Ienc
```

```text
B = μ0nI
```

```text
∇ · B = 0
```

```text
∇ × B = μ0J
```

After that memorize Faraday, Maxwell, and Poynting vector.

---

# 20. Small Sinhala-style memory help

- **Magnetostatics**: steady current නිසා ඇති වෙන magnetic field.
- **B field**: current එක වටේ circular විදියට යනවා.
- **Right-hand rule**: current direction thumb එක, fingers show B direction.
- **Ampere law**: loop එක ඇතුළේ current count කරන law එක.
- **Biot-Savart law**: small current element එකකින් B field හොයන law එක.
- **∇ · B = 0**: magnetic field lines start/end වෙන්නේ නෑ.
- **Faraday law**: changing B field එකෙන් E field එකක් induce වෙනවා.
- **Poynting vector**: EM energy යන direction එක.

---

## End of magnetostatics memorize notes
