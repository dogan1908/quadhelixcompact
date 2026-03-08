# From the Quadratic Sequence to the Conical Helix

**A Direct Algebraic Construction via the Universal Quantity Q(k) = √(48k+1)**

*Dogan Balban, 2026*

---

## Overview

This paper shows that the quadratic sequence

$$k(n) = \frac{1}{6}(2n^2 + 3n + 1)$$

— the arithmetic mean of the first *n* square numbers — determines a conical helix whose every geometric property follows from a single algebraic identity:

$$(4n+3)^2 = 48\,k(n) + 1.$$

The **universal quantity** $Q(k) = \sqrt{48k+1}$ encodes the complete three-dimensional geometry:

| Quantity | Formula in Q |
|----------|-------------|
| Height z | (Q − 3) / 4 |
| Angle θ | πQ / 12 |
| Radius r | Q / (2π) |

The helix lies simultaneously on an **Archimedean spiral** $r = (6/\pi^2)\,\theta$ and a **cone of revolution** $z = -3/4 + (\pi/2)\,r$ — both as one-line algebraic corollaries of the identity.

**All primes p > 3** appear as discrete points on the helix. This is a theorem, not an empirical observation.

## Main Results

1. **Integrality condition:** k(n) ∈ ℤ iff n ≡ 1, 5 (mod 6)
2. **Fundamental identity:** (4n+3)² = 48k(n) + 1
3. **Exact helix parametrisation** via Q(k) alone
4. **Spiral conformity:** r = (6/π²)θ, with slope constant 1/ζ(2) (Basel problem)
5. **Cone conformity:** z = −3/4 + (π/2)r
6. **Arc-length equivalence:** L → Δk asymptotically
7. **Prime corollary:** all p > 3 at θₚ = (π/3)p + π/4

## Repository Structure

```
├── main.tex              # Main LaTeX document
├── references.bib        # BibLaTeX bibliography
├── chapters/
│   ├── 01_introduction.tex    # §1 — Introduction and Main Theorem
│   ├── 02_sequence.tex        # §2 — The Quadratic Sequence
│   ├── 03_identity.tex        # §3 — Fundamental Identity and Q(k)
│   ├── 04_helix.tex           # §4 — The Conical Helix
│   ├── 05_arclength.tex       # §5 — Arc Length and Asymptotics
│   └── 06_primes.tex          # §6 — Prime Numbers on the Helix
├── bilder/               # Figures (add your own)
├── zenodo_description.html
├── LICENSE
└── README.md
```

## Building the PDF

Requires a standard TeX Live (2022+) or MiKTeX installation.

```bash
pdflatex main
biber main
pdflatex main
pdflatex main
```

### Required LaTeX packages

`mathtools`, `amssymb`, `amsthm`, `tcolorbox`, `booktabs`, `tabularx`,
`siunitx`, `biblatex` (with `biber` backend), `hyperref`, `enumitem`,
`graphicx`, `xcolor`, `float`.

## Figures

The `bilder/` directory is provided empty. If you wish to include figures,
place them there. The paper compiles without figures (LaTeX will issue
warnings for missing graphics but produce a complete PDF).

## Related Sequences

- [OEIS A164576](https://oeis.org/A164576) — Integer averages of the first n squares
- [OEIS A007310](https://oeis.org/A007310) — Positive integers coprime to 6

## Connection to the Extended Work

This compact paper is a self-contained extraction from a larger work
(*From the Quadratic Sequence to the Conical Helix: An Inductive Derivation*)
that follows the historical path of discovery — from table values through
the Archimedean spiral and cone construction to the helix. The present
version takes the direct algebraic route: the identity (4n+3)² = 48k+1
is the starting point, not the final insight.

## Citation

```bibtex
@misc{Balban2026helix,
  author = {Dogan Balban},
  title  = {From the Quadratic Sequence to the Conical Helix:
            A Direct Algebraic Construction},
  year   = {2026},
  doi    = {10.5281/zenodo.XXXXXXX},
  note   = {LaTeX source, GitHub repository}
}
```

*(Replace the DOI with your actual Zenodo DOI after upload.)*

## Licence

This work is licensed under the [Creative Commons Attribution 4.0 International Licence (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to share and adapt this material for any purpose, provided
you give appropriate credit.
