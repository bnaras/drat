# Additional Repository for `CVXR`

While we mostly tend to use [r-universe](https://r-universe.dev) for
additional packages, there are some that cannot be built using the
r-universe.dev tool chain currently.

So this is a [drat](https://cran.r-project.org/package=drat)
repository for a few exceptional packages that
[CVXR](https://cvxr.rbind.io) enhances. Only **source** packages are
distributed here (in `src/contrib`); there are no binary builds.

## Available packages

- **[ipopt](https://github.com/bnaras/ipopt)** — R interface to the
  [Ipopt](https://github.com/coin-or/Ipopt) nonlinear optimizer. It needs the
  Ipopt system library (and `pkg-config`) at install time, so it can be built
  neither on CRAN nor on r-universe and is distributed here as source. CVXR
  uses it as one of the backends for its differentiable nonlinear programming
  (DNLP) path.

  See <https://bnaras.github.io/ipopt/> for platform-specific instructions on
  installing Ipopt and building the package from source.
