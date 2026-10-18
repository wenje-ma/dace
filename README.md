# DACE Reading Notes

> Close-reading notes (with derivations) for **Santner, Williams & Notz, *The Design and Analysis of Computer Experiments*, 2nd ed., Springer** — Gaussian process models, EBLUP prediction, and the expected improvement algorithm.

This is a reading-notes repository, not the DACE MATLAB toolbox. The `notes.md` file follows the book's structure and records, for each section, a quote from the original text followed by questions and self-worked derivations.

## Contents

```
dace/
├── DACE.pdf      # The textbook itself (2nd ed., 446 pp.)
├── notes.md      # The reading notes (116 lines, English)
└── .gitignore
```

## Notes coverage

- **§2.2 Gaussian process models** — derivation of the multivariate normal conditional-distribution formulas; correlation functions (sinc-type, Gaussian); rate vs. scale parameter distinctions; validity of products/convex combinations of correlation functions.
- **§3.2 BLUP** — prediction under minimal MSPE via the law of total expectation.
- **§3.3 EBLUP** — comparison of MLE, REML and cross-validation estimation, and why REML is "less biased" (degrees-of-freedom argument, n_s − p).
- **§6.3.4 Expected Improvement** — the EI algorithm for global optimization of expensive black boxes.

## Why these sections

They are the three pillars needed for research on constrained Bayesian optimization, feasible-region/level-set learning, and multi-fidelity modeling: the GP surrogate (§2.2), its empirical-Bayes predictor (§3.2–3.3), and the acquisition function (§6.3.4).

## Format

Plain Markdown with inline LaTeX, English throughout; no build system. Read `notes.md` alongside the corresponding pages of `DACE.pdf`.

## Related repositories

See also [ed4dse](https://github.com/wenje-ma/ed4dse) — a full computational reproduction of V. Roshan Joseph's *Experimental Design for Data Science and Engineering* — and the [singapore](https://github.com/wenje-ma/singapore) research project on multi-fidelity Bayesian optimization. Full list on the [profile page](https://github.com/wenje-ma).
