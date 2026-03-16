# Hyperbolic Geometry Visualiser

An interactive single-file HTML application for exploring hyperbolic geometry through five interconnected visualisations.

### [Launch App](https://brendanjameslynskey.github.io/Hyperbolic_Geometry/)

---

## Mathematical Background

Hyperbolic geometry is the unique simply-connected, complete Riemannian 2-manifold of constant sectional curvature K = −1. It is one of the three classical geometries of constant curvature — the others being Euclidean geometry (K = 0) and spherical geometry (K > 0). The hyperbolic plane, denoted ℍ², cannot be isometrically embedded in Euclidean 3-space (a consequence of Hilbert's theorem, 1901), but it admits several faithful models within Euclidean space that preserve different geometric properties. The study of ℍ² reveals a geometry that is, in many respects, richer than its Euclidean counterpart: it possesses a continuum of parallel lines through any external point, its triangles have angle sums strictly less than π, and its isometry group acts transitively on the unit tangent bundle, giving it maximal symmetry among Riemannian surfaces.

The origin of hyperbolic geometry lies in the failure of Euclid's fifth postulate — the parallel postulate. In its original formulation, the postulate states that if a straight line falling on two straight lines makes the interior angles on the same side sum to less than two right angles, then the two lines, if produced indefinitely, meet on that side. An equivalent and more transparent formulation is Playfair's axiom (1795): through any point not on a given line, there exists exactly one line parallel to the given line. For over two millennia, mathematicians attempted to derive this postulate from the other four, believing it to be a theorem rather than an independent axiom. Hyperbolic geometry arises precisely when one negates the parallel postulate: through any point not on a given line, there exist infinitely many lines that do not intersect the given line. These are separated into two classes — the two limiting parallel lines (which approach the given line asymptotically in each direction) and the ultraparallel lines (which diverge from it on both sides).

A defining quantitative feature of the hyperbolic plane is the exponential growth of metric quantities. The circumference of a circle of hyperbolic radius r is 2π sinh r, which grows as πeʳ for large r, in contrast to the linear growth 2πr in Euclidean geometry. Similarly, the area enclosed by such a circle is 4π sinh²(r/2) = 2π(cosh r − 1), again exponential in r. This exponential growth is the geometric root of many of the plane's remarkable properties: hyperbolic space has "more room" at large distances, which is why it admits infinitely many parallels, why regular tilings {p, q} exist whenever (p − 2)(q − 2) > 4, and why trees and other hierarchical structures embed quasi-isometrically into ℍ². It also underlies the connection between hyperbolic geometry and negative curvature in Riemannian geometry more broadly.

The Gauss–Bonnet theorem provides the deepest link between the topology and geometry of hyperbolic surfaces. In ℍ², the theorem takes a particularly clean form: the area of a geodesic triangle with interior angles α, β, γ is π − (α + β + γ). Since all angles are non-negative and the area is positive, the angle sum of any hyperbolic triangle is strictly less than π; the difference π − (α + β + γ) is called the angular defect and is a direct measure of enclosed area. For a geodesic polygon with n sides and interior angles α₁, …, αₙ, the area generalises to π(n − 2) − (α₁ + ⋯ + αₙ). As a triangle becomes ideal (all three vertices move to the boundary at infinity), its angles tend to zero and its area tends to π, which is therefore the supremum of triangle areas in ℍ². The orientation-preserving isometry group of the hyperbolic plane is PSL(2, ℝ) ≅ Isom⁺(ℍ²), a three-dimensional Lie group. Every orientation-preserving isometry falls into one of three conjugacy classes: elliptic isometries (rotations about a fixed point in ℍ², with |tr(A)| < 2), hyperbolic isometries (translations along a unique invariant geodesic, with |tr(A)| > 2), and parabolic isometries (fixing a single point on the boundary ∂ℍ², with |tr(A)| = 2). These three types exhaust all orientation-preserving isometries, and their interplay governs the dynamics of Fuchsian groups and the geometry of hyperbolic surfaces.

## History

The parallel postulate troubled geometers from antiquity. Proclus (5th century CE), in his commentary on Euclid's Elements, noted that the fifth postulate lacked the self-evidence of the other four and recorded early attempts to derive it as a theorem. The most significant pre-modern effort was that of Girolamo Saccheri (1667–1733), whose Euclides ab Omni Naevo Vindicatus (Euclid Freed of Every Flaw, 1733) attempted a proof by reductio ad absurdum. Saccheri considered a quadrilateral with two right base angles and equal lateral sides and examined the three cases for the summit angles: right (Euclidean), obtuse (spherical), and acute. He successfully eliminated the obtuse case but, in pursuing the acute case, unwittingly proved a substantial body of theorems in what we now recognise as hyperbolic geometry — including the existence of asymptotic parallel lines — before declaring the results "repugnant to the nature of a straight line" and claiming victory. Johann Heinrich Lambert (1728–1777) went further in his Theorie der Parallellinien (1766, published posthumously in 1786): he observed that under the acute-angle hypothesis the area of a triangle is proportional to its angular defect, noted the analogy with spherical geometry (where area is proportional to angular excess), and speculated that the acute-angle hypothesis might describe geometry on a "sphere of imaginary radius" — a remarkably prescient insight.

The recognition that the negation of the parallel postulate yields a consistent geometry came independently to three mathematicians in the early nineteenth century. Nikolai Ivanovich Lobachevsky (1792–1856) published On the Principles of Geometry in 1829 in the Kazan Messenger, developing a complete system of "imaginary geometry" including explicit formulas for the angle of parallelism Π(d) = 2 arctan(e⁻ᵈ) and hyperbolic trigonometry. János Bolyai (1802–1860) reached similar conclusions independently and published them as the Appendix to his father Wolfgang Bolyai's Tentamen in 1832, under the title The Science Absolute of Space. Carl Friedrich Gauss (1777–1855) had privately arrived at the same ideas decades earlier — his correspondence reveals deep engagement with non-Euclidean geometry from at least 1816. In an 1824 letter to Franz Taurinus, Gauss described the geometry explicitly but wrote that he feared publishing because of the "cry of the Boeotians" — the outcry from those who would not understand. When Gauss received a copy of Bolyai's Appendix through Wolfgang, he famously replied that he could not praise it, for to do so would be to praise himself. The priority dispute between Lobachevsky and Bolyai, and the shadow of Gauss, remains one of the most storied episodes in the history of mathematics.

The question of logical consistency was settled by Eugenio Beltrami (1835–1900) in his Saggio di Interpretazione della Geometria Non-Euclidea (Essay on the Interpretation of Non-Euclidean Geometry, 1868). Beltrami showed that the geometry of Lobachevsky and Bolyai could be realised on surfaces of constant negative curvature in Euclidean 3-space — the pseudosphere being a local model — thereby proving its consistency relative to Euclidean geometry. Felix Klein (1849–1925) provided the projective disk model in 1871, in which geodesics appear as straight chords of a disk and the metric is derived from cross-ratios, building on earlier work of Arthur Cayley. Henri Poincaré (1854–1912) introduced the conformal disk and upper half-plane models in 1882, arising naturally from his work on automorphic functions and Fuchsian groups — discrete subgroups of PSL(2, ℝ) acting on the upper half-plane. These models made hyperbolic geometry accessible and computationally tractable, and remain the standard tools today.

Klein's Erlangen Programme (1872) provided the unifying framework: geometry is the study of properties invariant under a group of transformations. Euclidean geometry is the study of invariants under the group of rigid motions E(2); hyperbolic geometry is the study of invariants under PSL(2, ℝ). This perspective, in which the group determines the geometry, was revolutionary and remains foundational. In modern mathematics and physics, hyperbolic geometry appears in diverse and essential roles. The velocity addition formula in special relativity has hyperbolic geometry as its natural setting (the space of relativistic velocities is a model of ℍ³). Thurston's geometrisation conjecture (1982), proved by Grigori Perelman (2003) using Ricci flow, established that every closed 3-manifold can be decomposed into pieces each carrying one of eight model geometries — of which hyperbolic geometry is by far the most prevalent and the richest. Hyperbolic 3-manifolds are central objects in low-dimensional topology. In geometric group theory, Gromov hyperbolicity captures the large-scale features of negative curvature in a purely combinatorial setting. More recently, hyperbolic embeddings have found applications in machine learning, where the exponential growth of volume in hyperbolic space provides a natural and efficient geometry for representing hierarchical and tree-like data structures.

## The Models

**Poincaré disk model.** The hyperbolic plane is represented as the open unit disk 𝔻 = {z ∈ ℂ : |z| < 1} equipped with the metric ds² = 4|dz|² / (1 − |z|²)². This model is conformal: angles in the model coincide with hyperbolic angles. Geodesics are diameters of the disk and arcs of circles that meet the boundary circle ∂𝔻 at right angles. The boundary circle itself represents the "circle at infinity" or ideal boundary ∂ℍ², which is not part of the hyperbolic plane but plays a crucial role in the theory. The orientation-preserving isometries in this model are Möbius transformations of the form z ↦ eⁱᶿ(z − a)/(1 − āz) with a ∈ 𝔻 and θ ∈ ℝ, constituting the group PSU(1, 1) ≅ PSL(2, ℝ).

**Upper half-plane model.** The hyperbolic plane is represented as ℍ = {z ∈ ℂ : Im(z) > 0} with the metric ds² = |dz|² / (Im z)². This model is also conformal. Geodesics are vertical half-lines {x = c, y > 0} and semicircles with centres on the real axis. The real axis ℝ ∪ {∞} serves as the ideal boundary. The orientation-preserving isometries are the Möbius transformations z ↦ (az + b)/(cz + d) with a, b, c, d ∈ ℝ, ad − bc = 1, forming the group PSL(2, ℝ) directly. The Poincaré disk and upper half-plane models are related by the Cayley transform w = (z − i)/(z + i), which is an isometry between them.

**Klein (Beltrami–Klein) model.** The hyperbolic plane is again represented as the open unit disk, but with a different metric: ds² is chosen so that geodesics appear as straight Euclidean chords. This model is projective — collinearity is preserved — but it is not conformal; angles in the model do not correspond to hyperbolic angles. The metric is derived from the cross-ratio. The Klein model is particularly convenient for questions about incidence and betweenness, and for studying convexity in the hyperbolic plane.

**Hyperboloid model.** The hyperbolic plane is realised as the upper sheet of the two-sheeted hyperboloid {(x, y, t) ∈ ℝ²·¹ : −t² + x² + y² = −1, t > 0} in Minkowski space ℝ²·¹ with the Lorentzian inner product ⟨u, v⟩ = −u₀v₀ + u₁v₁ + u₂v₂. The induced metric from the ambient Minkowski space is positive-definite and gives the hyperbolic metric. Geodesics are intersections of the hyperboloid with planes through the origin. The isometry group is the orthochronous Lorentz group SO⁺(2, 1) ≅ PSL(2, ℝ). This model is particularly natural for computations in special relativity, and is the standard setting for the analytic theory. It is related to the other models by gnomonic and stereographic projections.

## Key Formulas

**Distance in the Poincaré disk.** For points z, w ∈ 𝔻:

    d(z, w) = 2 arctanh( |z − w| / |1 − z w̄| )

equivalently, cosh d(z, w) = 1 + 2|z − w|² / ((1 − |z|²)(1 − |w|²)).

**Distance in the upper half-plane.** For points z₁, z₂ ∈ ℍ:

    cosh d(z₁, z₂) = 1 + |z₁ − z₂|² / (2 Im(z₁) Im(z₂))

**Area of a geodesic triangle (Gauss–Bonnet).** For a triangle with interior angles α, β, γ:

    Area = π − (α + β + γ)

For a geodesic n-gon with interior angles α₁, …, αₙ:

    Area = π(n − 2) − (α₁ + ⋯ + αₙ)

**Angle of parallelism.** The angle of parallelism Π(d) for a perpendicular distance d from a point to a line is:

    Π(d) = 2 arctan(e⁻ᵈ)

For d = 0, Π = π/2 (Euclidean case). As d → ∞, Π → 0.

**Circumference and area of a hyperbolic circle of radius r:**

    C = 2π sinh r          A = 2π(cosh r − 1) = 4π sinh²(r/2)

**Isometry group representations.** In the Poincaré disk model, orientation-preserving isometries are SU(1, 1) matrices acting by Möbius transformations:

    z ↦ (az + b) / (b̄z + ā),     |a|² − |b|² = 1

In the upper half-plane model, they are SL(2, ℝ) matrices:

    z ↦ (az + b) / (cz + d),     ad − bc = 1,   a, b, c, d ∈ ℝ

**Classification of isometries (by trace of the SL(2, ℝ) representative A):**

| Type | Condition | Fixed points in ℍ² | Geometric action |
|---|---|---|---|
| Elliptic | \|tr A\| < 2 | One (interior) | Rotation about a fixed point |
| Parabolic | \|tr A\| = 2 | None (one on ∂ℍ²) | Fixes one ideal point; horocyclic translation |
| Hyperbolic | \|tr A\| > 2 | None (two on ∂ℍ²) | Translation along an invariant geodesic |

## Features

### 1. Poincare Disk Model
- Interactive unit disk with hyperbolic grid lines (geodesics rendered as circular arcs)
- Click to place points and draw geodesics between them
- Hyperbolic distance measurement using the formula `d(P,Q) = 2 arctanh|P-Q|/|1-P*conj(Q)|`
- Parallel line demonstration: multiple lines through a point that never meet a given line
- Conformal angle display showing angle-preservation

### 2. Hyperbolic Tilings {p,q}
- Regular tilings satisfying the hyperbolicity condition `(p-2)(q-2) > 4`
- Available tilings: {3,7}, {4,5}, {5,4}, {7,3}, {3,8}, {6,4}, {4,6}, {8,3}
- Recursive generation via reflection (Mobius inversion) across geodesic edges
- Four color schemes: by generation depth, alternating, rainbow, monochrome
- Adjustable recursion depth (2-5 levels)

### 3. Upper Half-Plane Model
- Geodesics as vertical lines and semicircles orthogonal to the real axis
- Distance formula `d = acosh(1 + |z1-z2|^2 / (2*y1*y2))`
- Horocycle and equidistant curve visualisation
- Cayley transform mapping `w = (z-i)/(z+i)` shown as an inset Poincare disk

### 4. Isometry Explorer
- Interactive Mobius transformations on the Poincare disk
- Sliders for hyperbolic translation (X, Y), elliptic rotation, and parabolic isometry
- Multiple test figures: triangle, square, grid, circle packing
- Live display of the SU(1,1) matrix representation

### 5. Hyperbolic Triangle
- Three draggable vertices on the Poincare disk
- Real-time computation of angles, angle sum (always < pi), and angular defect
- Hyperbolic area via the Gauss-Bonnet theorem: `Area = pi - (alpha + beta + gamma)`
- Side-by-side Euclidean comparison (dashed lines)

## Technical Details

- **Rendering**: HTML5 Canvas with device-pixel-ratio scaling for crisp rendering on HiDPI displays
- **Geodesics**: Computed as circular arcs orthogonal to the unit circle boundary
- **Tilings**: Generated by recursive reflection across polygon edges using circle inversion
- **Isometries**: Composed as SU(1,1) Mobius transformations `z -> (az+b)/(conj(b)z+conj(a))`
- **Styling**: Dark theme (#0a0a0f background) with teal, amber, and purple accent colors; DM Sans + JetBrains Mono typography
