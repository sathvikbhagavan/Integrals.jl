# [Integral Solver Algorithms](@id solvers)

The following algorithms are available:

  - `QuadGKJL`: Uses QuadGK.jl. Requires `nout=1` and `batch=0`, in-place is not allowed.
  - `HCubatureJL`: Uses HCubature.jl. Requires `batch=0`.
  - `VEGAS`: Uses MonteCarloIntegration.jl. Requires `nout=1`. Works only for `>1`-dimensional integrations.
  - `CubatureJLh`: h-Cubature from Cubature.jl. Requires `using IntegralsCubature`.
  - `CubatureJLp`: p-Cubature from Cubature.jl. Requires `using IntegralsCubature`.
  - `CubaVegas`: Vegas from Cuba.jl. Requires `using IntegralsCuba`, `nout=1`.
  - `CubaSUAVE`: SUAVE from Cuba.jl. Requires `using IntegralsCuba`.
  - `CubaDivonne`: Divonne from Cuba.jl. Requires `using IntegralsCuba`. Works only for `>1`-dimensional integrations.
  - `CubaCuhre`: Cuhre from Cuba.jl. Requires `using IntegralsCuba`. Works only for `>1`-dimensional integrations.
  - `GaussLegendre`: Uses Gauss-Legendre quadrature with nodes and weights from FastGaussQuadrature.jl.
  - `QuadratureRule`: Accepts a user-defined function that returns nodes and weights.

```@docs
QuadGKJL
HCubatureJL
VEGAS
GaussLegendre
QuadratureRule
```
