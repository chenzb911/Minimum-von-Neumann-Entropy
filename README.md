# The minimum von Neumann entropy of a connected graph

LaTeX source for a research manuscript on the density matrix
`rho(G) = L(G)/(2|E(G)|)`, where `L(G)` is the combinatorial Laplacian
of a finite simple graph. All logarithms are natural.

## Main results

- The star uniquely minimizes von Neumann entropy among connected
  simple graphs of a given order, resolving Conjecture 1.2 of Dairyko
  et al. (2017).
- Sharp bounds under prescribed Laplacian rank and clique or chromatic
  number, with pineapple graphs and isolated vertices as the equality cases.
- Completion of the star-minimum Rényi conjecture for all orders greater
  than one. The additional range is `1 < alpha < 2`: the range
  `alpha >= 2` follows from earlier results, as explained in the manuscript.
- The triangle pineapple uniquely minimizes entropy among all connected
  nontrees for every finite Rényi order at least one. The main new comparison
  concerns von Neumann entropy and orders between one and two.
- Explicit counterexamples showing limitations below order one, for
  coefficient comparison above order two, and for high-order bounds with
  prescribed clique or chromatic number.

The proofs use earlier Kelmans transformation and Laplacian coefficient
theorems. The main optimization compares threshold graphs with different
numbers of edges and different normalizing traces. Tree extrema and
several probability comparisons are recorded with their prior sources;
they are not presented as independent new results.

## Source

`Minimum_von_Neumann_Entropy.tex` is self-contained: the bibliography
and TikZ figure are embedded. It uses the standard `amsart` class and
packages available in ordinary TeX Live or MiKTeX installations. It can
also be imported into Overleaf. No PDF or external figure files are included.

A source check without generating a PDF can be run twice:

```sh
pdflatex -draftmode -interaction=nonstopmode -halt-on-error Minimum_von_Neumann_Entropy.tex
pdflatex -draftmode -interaction=nonstopmode -halt-on-error Minimum_von_Neumann_Entropy.tex
```

## Status and references

This repository contains a manuscript draft, not a journal publication.
The author and affiliation fields in the source are awaiting completion.
The source includes a disclosure of assistance from ChatGPT.

The conjectures are from M. Dairyko et al., *Note on von Neumann and
Rényi entropies of a graph*, Linear Algebra and its Applications 521
(2017), 240–253, [doi:10.1016/j.laa.2017.01.037](https://doi.org/10.1016/j.laa.2017.01.037).
Detailed statements, equality conditions, and attribution to prior work
are provided in the manuscript.
