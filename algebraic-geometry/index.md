---
layout: default
title: Algebraic Geometry
---

# 𝕍 Algebraic Geometry

The branch of mathematics that studies geometric objects defined by polynomial equations, connecting algebra and geometry through the language of schemes, varieties, and sheaves.

---

## Quick Overview

- [FOAG — Ravi Vakil's Notes](https://math.stanford.edu/~vakil/216blog/FOAGnov1817public.pdf)
- [Stacks Project](https://stacks.math.columbia.edu/)
- [MIT 18.725 — Algebraic Geometry](https://ocw.mit.edu/courses/18-725-algebraic-geometry-fall-2015/)

## Core Concepts

### Classical Algebraic Geometry

#### Affine and Projective Varieties
- **Affine Variety:** Zero set $V(I) \subseteq \mathbb{A}^n$ of an ideal $I \subseteq k[x_1,\ldots,x_n]$.
- **Projective Variety:** Zero set in projective space $\mathbb{P}^n$; the natural setting for compact geometry.
- **Hilbert's Nullstellensatz:** $I(V(I)) = \sqrt{I}$ — algebraic/geometric correspondence over algebraically closed fields.
- **Coordinate Ring:** $k[V] = k[x_1,\ldots,x_n]/I(V)$ — functions on the variety.
- **Morphisms:** Maps between varieties given locally by polynomials.

#### Dimension and Smoothness
- **Krull Dimension:** Length of the longest chain of prime ideals.
- **Tangent Space:** Dual of $\mathfrak{m}/\mathfrak{m}^2$ at a point; detects singularities.
- **Smooth Point:** Dimension of tangent space equals dimension of variety.
- **Blow-up:** Resolution of singularities by replacing a point with a projective space.

### Sheaves and Modern Language

#### Sheaves
- **Presheaf:** Functor $\mathcal{F}: \text{Open}(X)^{\text{op}} \to \textbf{Set}$ assigning sections to open sets.
- **Sheaf Condition:** Local sections compatible on overlaps glue to a unique global section.
- **Structure Sheaf $\mathcal{O}_X$:** Sheaf of regular functions on a variety or scheme.
- **Quasi-coherent Sheaf:** Algebraic analogue of a vector bundle.

#### Schemes
- **Spectrum $\text{Spec}(A)$:** Topological space of prime ideals of a ring $A$, with structure sheaf.
- **Scheme:** Locally ringed space locally isomorphic to $\text{Spec}(A)$.
- **Morphism of Schemes:** Map of locally ringed spaces.
- **Fiber Product:** $X \times_S Y$ — base change; fundamental construction.
- **Separated / Proper:** Scheme-theoretic analogues of Hausdorff / compact.

#### Cohomology
- **Čech Cohomology:** $\check{H}^i(\mathcal{U}, \mathcal{F})$ — computed from open covers.
- **Sheaf Cohomology $H^i(X, \mathcal{F})$:** Right derived functors of global sections.
- **Serre Duality:** $H^i(X, \mathcal{F}) \cong H^{n-i}(X, \omega_X \otimes \mathcal{F}^\vee)^\vee$ for smooth projective $X$.
- **Riemann-Roch Theorem:** $\chi(\mathcal{L}) = \deg(\mathcal{L}) + 1 - g$ for a line bundle on a curve of genus $g$.

## Recommended Books

### Introductory

- **Cox, Little, O'Shea** — *Ideals, Varieties, and Algorithms*
  - Accessible introduction via computational methods; Gröbner bases.
  - Difficulty: ★★★☆☆ | Language: English

- **Reid** — *Undergraduate Algebraic Geometry*
  - Short and readable; classical varieties and the Nullstellensatz.
  - Difficulty: ★★☆☆☆ | Language: English

- **Fulton** — *Algebraic Curves*
  - Free online; classical curves and the Riemann-Roch theorem.
  - Difficulty: ★★★☆☆ | Language: English

### Intermediate

- **Hartshorne** — *Algebraic Geometry*
  - The standard graduate reference; schemes, sheaves, cohomology.
  - Difficulty: ★★★★★ | Language: English

- **Shafarevich** — *Basic Algebraic Geometry* (2 vols.)
  - Broad coverage from classical to modern; many examples.
  - Difficulty: ★★★★☆ | Language: English

### Advanced

- **Grothendieck / Dieudonné** — *EGA*
  - Foundational treatise on scheme theory.
  - Difficulty: ★★★★★ | Language: French / English translations partial

- **Vakil** — *The Rising Sea: Foundations of Algebraic Geometry* (FOAG)
  - Modern, freely available notes; highly recommended.
  - Difficulty: ★★★★☆ | Language: English

## Web Resources

- [FOAG — Ravi Vakil's Notes](https://math.stanford.edu/~vakil/216blog/FOAGnov1817public.pdf) — Comprehensive free textbook
- [Stacks Project](https://stacks.math.columbia.edu/) — Online reference for algebraic geometry and commutative algebra
- [MIT OCW — Algebraic Geometry](https://ocw.mit.edu/courses/18-725-algebraic-geometry-fall-2015/) — Lecture notes and problem sets
- [nLab — Algebraic Geometry](https://ncatlab.org/nlab/show/algebraic+geometry) — Categorical perspective

### Problem Sets

- [Hartshorne Exercises](https://math.stackexchange.com/questions/tagged/algebraic-geometry) — Community solutions on Math StackExchange
- [Algebraic Geometry — MathOverflow](https://mathoverflow.net/questions/tagged/algebraic-geometry) — Research-level discussions

## Video Lectures

### University Courses

- [MIT 18.725 — Algebraic Geometry](https://ocw.mit.edu/courses/18-725-algebraic-geometry-fall-2015/) — Lecture notes
- [ICTP Diploma — Algebraic Geometry](https://www.youtube.com/playlist?list=PLLq_gUfXAnkk3OQRNwN8-JkF_lv2B_6oM) — Full lecture series

### YouTube

- [Algebraic Geometry — Richard Borcherds](https://www.youtube.com/@RichardBorcherds) — Graduate-level lectures
- [The Rising Sea — supplementary videos](https://www.youtube.com/results?search_query=algebraic+geometry+schemes) — Schemes and sheaves

---

[← Differential Geometry]({{ '/differential-geometry/' | relative_url }}) | [Home]({{ '/' | relative_url }})
