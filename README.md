# Master Project: "Regularized Four‑Sided Cavity Flows: A Spectral Bifurcation Benchmark implemented in Julia"

Repository of my master project. Contains Tex files for the [PDF](./src/main.pdf)
of the report. The Julia code can be found here:
[FourSidedCavityFlow.jl](https://github.com/morwald/FourSidedCavityFlow.jl.git).

## Abstract 

This master project explores a regularized version of the four-sided lid-driven
cavity for incompressible fluids to be used as a validator benchmark for
Navier-Stokes solvers. The four-sided driven cavity is an extension of the
simple one-sided lid-driven case, where all lids move with the same velocity
profile and parallel lids move in opposite directions. This study focuses on a
regularized version to overcome corner singularities. The considered method
recovers exponential convergence with a pseudo-spectral Chebyshev
discretization scheme. The flow presents a variety of bifurcation scenarios and
could make up for an amenable Navier-Stokes bifurcation benchmark. The
algorithms are implemented in Julia, a high-performance language for scientific
computing. A developed Julia module provides a reproducible example for the
proposed problem.

## Project Structure

- **/src:** Contains the LaTeX source files.
- **/src/figs:** Any images or figures used in the document.
- **/src/bib:** Bibliography files.
- **/externe** External LaTex packages.

## How to Compile

To compile the LaTeX file, inside of the `src` folder:

```bash
pdflatex main.tex
```

Run the BibTex command and compile the document multiple times to resolve
references and generate the bibliography:

```bash
bibtex main
pdflatex main.tex
pdflatex main.tex
```

## Credits 

The [template](https://wiki.epfl.ch/sma/pdm) for the report was provided by
Mathematics sections at EPFL.
