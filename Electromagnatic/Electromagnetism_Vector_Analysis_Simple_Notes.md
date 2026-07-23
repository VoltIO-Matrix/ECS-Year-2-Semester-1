# Electromagnetism Lecture Notes — Vector Analysis

**Course:** Electromagnetism (BECS 21422)  
**Topic:** Course introduction + Review of vector analysis  
**Lecturer:** Dr. P.A.N.S. Priyadharshana

---

## 1. Course introduction

Electromagnetism studies electric fields, magnetic fields, and how they are connected. In this course you will learn:

- **Vector analysis** — the mathematics needed for fields.
- **Electrostatics** — electric charges and electric fields when charges are not moving.
- **Magnetostatics** — magnetic fields due to steady currents.
- **Electromagnetism** — changing electric and magnetic fields, Maxwell’s equations, and electromagnetic waves.

### Evaluation

- Final exam: **90%**
- Class participation and tutorials: **10%**

### Main learning objectives

By the end of the course, you should be able to:

1. Use the mathematical tools needed for electromagnetism.
2. Understand basic electromagnetic concepts.
3. Use Maxwell’s equations to explain electromagnetic wave propagation.
4. Solve problems in electromagnetic applications.

---

# 2. Scalars and vectors

## 2.1 Scalar quantities

A **scalar** has magnitude only. It does not have direction.

Examples:

- Mass
- Distance
- Time
- Temperature
- Energy

Example:  
If the temperature is **30 °C**, it is just a value. There is no direction.

## 2.2 Vector quantities

A **vector** has both magnitude and direction.

Examples:

- Displacement
- Velocity
- Acceleration
- Force / weight
- Momentum
- Electric field
- Magnetic field

Example:  
A velocity of **20 m/s east** is a vector because it has:

- Magnitude = 20 m/s
- Direction = east

---

# 3. Vector representation in Cartesian coordinates

In 3D Cartesian coordinates, we use the axes:

- x-axis
- y-axis
- z-axis

The unit vectors along these axes are:

- `î` along x-axis
- `ĵ` along y-axis
- `k̂` along z-axis

A vector **A** can be written as:

```text
A = Ax î + Ay ĵ + Az k̂
```

where:

- `Ax` = x component
- `Ay` = y component
- `Az` = z component

Example:

```text
A = 2 î + 3 ĵ + 4 k̂
```

This means:

- 2 units in x direction
- 3 units in y direction
- 4 units in z direction

---

# 4. Vector addition and subtraction

Suppose:

```text
A = Ax î + Ay ĵ + Az k̂
B = Bx î + By ĵ + Bz k̂
```

## 4.1 Addition

```text
A + B = (Ax + Bx)î + (Ay + By)ĵ + (Az + Bz)k̂
```

You add matching components.

### Example

```text
A = 2 î + 3 ĵ + 4 k̂
B = 1 î + 0 ĵ - 1 k̂
```

Then:

```text
A + B = (2 + 1)î + (3 + 0)ĵ + (4 - 1)k̂
A + B = 3 î + 3 ĵ + 3 k̂
```

## 4.2 Subtraction

```text
A - B = (Ax - Bx)î + (Ay - By)ĵ + (Az - Bz)k̂
```

### Example

```text
A - B = (2 - 1)î + (3 - 0)ĵ + (4 - (-1))k̂
A - B = 1 î + 3 ĵ + 5 k̂
```

---

# 5. Dot product / scalar product

The dot product of two vectors gives a **scalar** answer.

```text
A · B = |A||B| cos θ
```

where:

- `|A|` = magnitude of A
- `|B|` = magnitude of B
- `θ` = angle between A and B

In component form:

```text
A · B = AxBx + AyBy + AzBz
```

## Important points

- Dot product gives a **number**, not a vector.
- Dot product is commutative:

```text
A · B = B · A
```

## Simple meaning

Dot product tells how much one vector points in the direction of another vector.

### Example

```text
A = 2 î + 3 ĵ + 4 k̂
B = 1 î + 0 ĵ - 1 k̂
```

```text
A · B = (2)(1) + (3)(0) + (4)(-1)
A · B = 2 + 0 - 4
A · B = -2
```

---

# 6. Cross product / vector product

The cross product of two vectors gives a **vector** answer.

```text
A × B = |A||B| sin θ n̂
```

where:

- `θ` = angle between A and B
- `n̂` = unit vector perpendicular to both A and B

## Important points

- Cross product gives a vector.
- The direction is perpendicular to the plane containing A and B.
- Cross product is not commutative:

```text
A × B = - B × A
```

## Component formula

If:

```text
A = Ax î + Ay ĵ + Az k̂
B = Bx î + By ĵ + Bz k̂
```

then:

```text
A × B = (AyBz - AzBy)î - (AxBz - AzBx)ĵ + (AxBy - AyBx)k̂
```

This can also be written using a determinant:

```text
        | î   ĵ   k̂  |
A × B = | Ax  Ay  Az |
        | Bx  By  Bz |
```

### Example from lecture

```text
A = 2 î + 3 ĵ + 4 k̂
B = 1 î + 0 ĵ - 1 k̂
```

Answer:

```text
A × B = -3 î + 6 ĵ - 3 k̂
```

---

# 7. Position vector, unit vector, and separation vector

## 7.1 Position vector

A position vector tells the location of a point from the origin.

For a point `P(x, y, z)`:

```text
r = x î + y ĵ + z k̂
```

The magnitude of `r` is:

```text
|r| = √(x² + y² + z²)
```

## 7.2 Unit vector

A unit vector has magnitude **1**. It only shows direction.

To find a unit vector in the direction of `r`:

```text
r̂ = r / |r|
```

So:

```text
r̂ = (x î + y ĵ + z k̂) / √(x² + y² + z²)
```

## 7.3 Separation vector

In electromagnetism, we often use two points:

- Source point: `r'`
- Field point: `r`

The separation vector from source point to field point is:

```text
r - r'
```

The unit vector along the separation vector is:

```text
(r - r') / |r - r'|
```

## Simple meaning

If a charge is at the source point and we want to find the electric field at the field point, the separation vector tells the direction from the charge to the point of interest.

---

# 8. Del operator / nabla operator

The del operator is written as:

```text
∇
```

In Cartesian coordinates:

```text
∇ = î ∂/∂x + ĵ ∂/∂y + k̂ ∂/∂z
```

It is used to define:

1. Gradient
2. Divergence
3. Curl
4. Laplacian

---

# 9. Gradient of a scalar field

A scalar field gives a scalar value at every point in space.

Example:

- Temperature in a room
- Height of a hill
- Electric potential

If the scalar field is:

```text
φ(x, y, z)
```

then the gradient is:

```text
∇φ = (∂φ/∂x)î + (∂φ/∂y)ĵ + (∂φ/∂z)k̂
```

## Meaning of gradient

The gradient tells:

1. The direction where the scalar field increases fastest.
2. How fast the scalar field increases in that direction.

## Simple example

Imagine a hill:

- The scalar field is height.
- The gradient points uphill, in the steepest direction.

So:

```text
Gradient of scalar field = vector field
```

---

# 10. Divergence of a vector field

A vector field gives a vector at every point in space.

Examples:

- Fluid velocity field
- Electric field
- Magnetic field

If:

```text
F = Fx î + Fy ĵ + Fz k̂
```

then divergence is:

```text
∇ · F = ∂Fx/∂x + ∂Fy/∂y + ∂Fz/∂z
```

## Meaning of divergence

Divergence measures how much a vector field spreads out from a point.

### Positive divergence

The field spreads outward.

Example: water flowing out from a source.

### Negative divergence

The field goes inward.

Example: water flowing into a sink.

### Zero divergence

No net spreading or sinking.

## Important

```text
Divergence of vector field = scalar field
```

---

# 11. Curl of a vector field

Curl measures how much a vector field rotates or curls around a point.

If:

```text
F = Fx î + Fy ĵ + Fz k̂
```

then:

```text
∇ × F
```

is the curl of `F`.

In determinant form:

```text
        | î       ĵ       k̂    |
∇ × F = | ∂/∂x   ∂/∂y   ∂/∂z |
        | Fx      Fy      Fz   |
```

## Meaning of curl

Curl tells whether the field has rotation.

Examples:

- Water rotating in a whirlpool has curl.
- Uniform straight-line flow has no curl.

## Important

```text
Curl of vector field = vector field
```

---

# 12. Worked exercises from lecture

## Exercise 1: Divergence

Find the divergence of:

```text
F = (x²y, yz², zx²)
```

This means:

```text
Fx = x²y
Fy = yz²
Fz = zx²
```

Formula:

```text
∇ · F = ∂Fx/∂x + ∂Fy/∂y + ∂Fz/∂z
```

Calculate each part:

```text
∂(x²y)/∂x = 2xy
∂(yz²)/∂y = z²
∂(zx²)/∂z = x²
```

Therefore:

```text
∇ · F = 2xy + z² + x²
```

## Exercise 2: Curl

Find the curl of:

```text
G = (yz, xz, xy)
```

So:

```text
Gx = yz
Gy = xz
Gz = xy
```

Curl formula:

```text
∇ × G = (∂Gz/∂y - ∂Gy/∂z)î
      + (∂Gx/∂z - ∂Gz/∂x)ĵ
      + (∂Gy/∂x - ∂Gx/∂y)k̂
```

Now calculate:

```text
∂Gz/∂y = ∂(xy)/∂y = x
∂Gy/∂z = ∂(xz)/∂z = x
```

First component:

```text
x - x = 0
```

Second component:

```text
∂Gx/∂z = ∂(yz)/∂z = y
∂Gz/∂x = ∂(xy)/∂x = y

y - y = 0
```

Third component:

```text
∂Gy/∂x = ∂(xz)/∂x = z
∂Gx/∂y = ∂(yz)/∂y = z

z - z = 0
```

Therefore:

```text
∇ × G = (0, 0, 0)
```

---

# 13. Fundamental theorem for gradient

The theorem says:

```text
∫ from a to b ∇φ · dl = φ(b) - φ(a)
```

## Meaning

If a vector field is the gradient of a scalar field, then the line integral depends only on the start and end points.

It does not depend on the path taken.

## Important results

1. The line integral is path-independent.
2. Around a closed path:

```text
∮ ∇φ · dl = 0
```

## Simple explanation

Imagine walking on a hill from point A to point B.

The change in height depends only on:

- height at A
- height at B

It does not depend on the path you walked.

---

# 14. Fundamental theorem for divergence — Gauss’s theorem

Gauss’s theorem says:

```text
∫V (∇ · F) dv = ∮S F · n̂ ds
```

## Meaning

The total divergence inside a volume equals the total flux through the closed surface around that volume.

## Terms

- `V` = volume
- `S` = closed surface around the volume
- `n̂` = outward unit normal vector
- `F · n̂` = part of the vector field going through the surface

## Simple explanation

Imagine a balloon with air flowing inside.

- If more air is created inside, air must flow out through the surface.
- Gauss’s theorem connects what happens inside the volume with what crosses the surface.

## Conditions

1. The surface can have any shape.
2. The surface must be closed.
3. The vector field must be continuous.

---

# 15. Fundamental theorem for curl — Stokes’ theorem

Stokes’ theorem says:

```text
∫S (∇ × F) · n̂ ds = ∮C F · dl
```

## Meaning

The surface integral of curl over a surface equals the line integral around the boundary curve of that surface.

## Terms

- `S` = surface
- `C` = boundary curve around the surface
- `n̂` = unit normal to the surface
- `dl` = small path element along the boundary

## Simple explanation

Stokes’ theorem connects:

- rotation over a surface
- circulation around the edge of that surface

Example:  
If water rotates inside a circular region, the total rotation is related to how much water circulates around the boundary.

## Conditions

1. The boundary must be a closed loop.
2. The normal direction must follow the right-hand rule.
3. The vector field must be continuous.

---

# 16. Important vector identities

## 16.1 Laplacian operator

The Laplacian is:

```text
∇²φ = ∂²φ/∂x² + ∂²φ/∂y² + ∂²φ/∂z²
```

It is written as:

```text
∇² = ∇ · ∇
```

## 16.2 Curl of a gradient

```text
∇ × ∇φ = 0
```

Meaning:  
The curl of a gradient is always zero.

## 16.3 Divergence of a curl

```text
∇ · (∇ × V) = 0
```

Meaning:  
The divergence of a curl is always zero.

## 16.4 Curl of curl identity

```text
∇ × (∇ × V) = ∇(∇ · V) - ∇²V
```

This identity is useful in electromagnetism and wave equations.

---

# 17. Integral calculus summary

## 17.1 Line integral

```text
∫ F · dl
```

This measures circulation or work along a path.

Example:  
Work done by a force along a path.

## 17.2 Surface integral / flux

```text
∫ F · n̂ ds
```

This measures how much of a vector field passes through a surface.

Example:  
Electric flux through a surface.

## 17.3 Volume integral

```text
∫ φ dv
```

This adds a scalar quantity over a volume.

Example:  
Total mass from density over a volume.

---

# 18. Spherical polar coordinates

Spherical coordinates are useful when a problem has spherical symmetry.

A point is written as:

```text
P(r, θ, φ)
```

where:

- `r` = radial distance from origin
- `θ` = polar angle from z-axis
- `φ` = azimuthal angle in xy-plane

## 18.1 Relation with Cartesian coordinates

```text
x = r sinθ cosφ
y = r sinθ sinφ
z = r cosθ
```

## 18.2 Unit vectors

Spherical coordinates use:

- `r̂` = radial direction
- `θ̂` = direction of increasing θ
- `φ̂` = direction of increasing φ

## 18.3 Infinitesimal displacement

```text
dl = dr r̂ + r dθ θ̂ + r sinθ dφ φ̂
```

## 18.4 Surface elements

When `r` is constant:

```text
ds = r² sinθ dθ dφ r̂
```

When `θ` is constant:

```text
ds = r sinθ dr dφ θ̂
```

## 18.5 Volume element

```text
dv = r² sinθ dr dθ dφ
```

## Simple explanation

Use spherical coordinates when objects look like spheres.

Examples:

- Electric field around a point charge
- Gravitational field around a planet
- Charge distribution in a sphere

---

# 19. Cylindrical coordinates

Cylindrical coordinates are useful when a problem has cylindrical symmetry.

A point is written as:

```text
P(ρ, φ, z)
```

where:

- `ρ` = distance from z-axis
- `φ` = angle around z-axis
- `z` = height, same as Cartesian z

## 19.1 Relation with Cartesian coordinates

```text
x = ρ cosφ
y = ρ sinφ
z = z
```

## 19.2 Unit vectors

Cylindrical coordinates use:

- `ρ̂` = radial direction away from z-axis
- `φ̂` = direction around z-axis
- `ẑ` = vertical direction

## 19.3 Infinitesimal displacement

```text
dl = dρ ρ̂ + ρ dφ φ̂ + dz ẑ
```

## 19.4 Surface elements

When `ρ` is constant:

```text
ds = ρ dφ dz ρ̂
```

When `z` is constant:

```text
ds = ρ dρ dφ ẑ
```

## 19.5 Volume element

```text
dv = ρ dρ dφ dz
```

## Simple explanation

Use cylindrical coordinates when objects look like cylinders.

Examples:

- Long charged wire
- Coaxial cable
- Solenoid
- Cylindrical conductor

---

# 20. Quick comparison table

| Concept | Input | Output | Meaning |
|---|---|---|---|
| Gradient `∇φ` | Scalar field | Vector field | Direction of fastest increase |
| Divergence `∇ · F` | Vector field | Scalar field | Spreading out from a point |
| Curl `∇ × F` | Vector field | Vector field | Rotation around a point |
| Laplacian `∇²φ` | Scalar field | Scalar field | Second-derivative spreading/curvature |

---

# 21. When to use each coordinate system

| Coordinate system | Best for | Example |
|---|---|---|
| Cartesian `(x, y, z)` | Rectangular shapes | Box, flat plates |
| Spherical `(r, θ, φ)` | Spherical symmetry | Point charge, sphere |
| Cylindrical `(ρ, φ, z)` | Cylindrical symmetry | Long wire, cylinder |

---

# 22. Very short exam-focused summary

Remember these main ideas:

1. **Scalar** = magnitude only.
2. **Vector** = magnitude + direction.
3. **Dot product** gives a scalar.
4. **Cross product** gives a vector perpendicular to both vectors.
5. **Gradient** changes a scalar field into a vector field.
6. **Divergence** measures source/sink behavior.
7. **Curl** measures rotation.
8. **Gauss’s theorem** connects volume divergence with surface flux.
9. **Stokes’ theorem** connects surface curl with boundary circulation.
10. Use **spherical coordinates** for spherical symmetry.
11. Use **cylindrical coordinates** for cylindrical symmetry.

---

# 23. Simple memory tricks

- **Gradient**: “Which way is uphill?”
- **Divergence**: “Is the field spreading out or going in?”
- **Curl**: “Is the field rotating?”
- **Gauss**: “Inside source equals outside flux.”
- **Stokes**: “Rotation on surface equals circulation around edge.”

---

# 24. Practice questions

Try these after studying:

1. What is the difference between a scalar and a vector?
2. Find `A + B` if `A = 2î + ĵ + 3k̂` and `B = î - 2ĵ + k̂`.
3. Find `A · B` for the same vectors.
4. What does divergence tell us physically?
5. What does curl tell us physically?
6. When should you use spherical coordinates?
7. When should you use cylindrical coordinates?
8. State Gauss’s theorem in words.
9. State Stokes’ theorem in words.
10. Why is the line integral of a gradient field path-independent?

---

## End of notes
