# Newton

Lean 4 formalization of **Newton's inequalities** for real polynomials whose roots are all real: for such a polynomial of degree `n`, the squared coefficients satisfy

\[
\frac{c_i^2}{c_{i-1} c_{i+1}} \geq \frac{(n-i+1)(i+1)}{(n-i)(i)}
\]

(with the obvious conventions when some coefficients vanish).

## Main files

- [`Newton/newton.lean`](Newton/newton.lean) — forward direction of Newton's inequalities.
- [`Newton/reverse.lean`](Newton/reverse.lean) — supporting results on reversed/split polynomials used in the proof.

The root library module is [`Newton.lean`](Newton.lean).

## Build

Requires [Lean 4](https://leanprover.github.io/lean4/doc/setup.html) and [Lake](https://github.com/leanprover/lean4/tree/master/src/lake). Mathlib is fetched via `lake-manifest.json`.

```bash
lake build
```
