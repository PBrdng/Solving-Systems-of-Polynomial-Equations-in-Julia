# Solving-Systems-of-Polynomial-Equations-in-Julia

This repository contains material for the course [Numerical Algebraic Geometry in Julia](https://kvv.imp.fu-berlin.de/portal/site/34e97129-0915-401f-9f0e-cef093568c18/page/7122cafb-c0cb-42e2-aefe-c014146d98c0?sakai.state.reset=true) taking place in the winter semester 2019 at FU Berlin.

The simplest way to download the Jupyter notebooks from this repository is using the green button on the right.

### Installation
Download the latest Julia version at [julialang.org](https://julialang.org/downloads/).
Please see the [platform specific instructions](https://julialang.org/downloads/platform.html) if you have trouble installing Julia.

All packages that we need in this course are available through the Julia package manager.
You can enter it by first starting a Julia session and then pressing `]` in the REPL.

We need the packages [HomotopyContinuation.jl](https://github.com/JuliaHomotopyContinuation/HomotopyContinuation.jl), [DynamicPolynomials.jl](https://github.com/JuliaAlgebra/DynamicPolynomials.jl), [Plots.jl](https://github.com/JuliaPlots/Plots.jl), [ImplicitPlots](https://github.com/saschatimme/ImplicitPlots) and [IJulia](https://github.com/JuliaLang/IJulia.jl). In the package manager they are installed as follows:

```julia
pkg> add HomotopyContinuation DynamicPolynomials Plots IJulia
pkg> add https://github.com/saschatimme/ImplicitPlots
```

Alternatively, in the REPL you can also use

```julia-repl
julia> import Pkg
julia> Pkg.add("HomotopyContinuation")
julia> Pkg.add("DynamicPolynomials")
julia> Pkg.add("Plots")
julia> Pkg.add("IJulia")
julia> Pkg.clone("https://github.com/saschatimme/ImplicitPlots")
```

### Starting IJulia

For using the Jupyter notebooks from this repository you need to start IJulia. This is done in the Julia REPL as follows.
```julia-repl
julia> using IJulia
julia> notebook()
```
After executing this a browser window should pop up, which lets you easily navigate towards the Jupyter notebook files.
