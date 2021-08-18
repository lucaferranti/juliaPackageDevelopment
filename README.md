# Package development in Julia

This repository contains the materials for the "Package development in Julia" tutorial given on 18th August 2021 as part of the 
Nordic-RSE [Research Software Seminar Series](https://nordic-rse.org/events/seminar-series/). 

## Target audience

This tutorial is meant for people who have previous coding experience and would like to know how to use Julia for packages development. Previous exposure to Julia can be beneficial but is not strictly needed.

## Installation

1. If you haven't already, [install Julia](https://julialang.org/downloads/)
2. (Optional) During the workshop, I will be using VScode, as it has a nice integration with Julia, however you should be able to follow with any other text editor/IDE. 
   1. Download VScode [here](https://code.visualstudio.com/Download)
   2. If you use VScode, do install the [Julia extension](https://marketplace.visualstudio.com/items?itemName=julialang.language-julia)

3. Clone this repository to your preferred location and enter it
  ```
  git clone ...
  ```
  ```
  cd juliaPkgDevelopment
  ```

4. Start a Julia Session
  ```
  julia
  ```

5 Activate and instantiate the environment, this will make sure you have downloaded all the packages needed for the tutorial
  ```julia
  julia> using Pkg; Pkg.activate(__@DIR__); Pkg.instantiate()
  ```

6. Verify it was successful by doing e.g.
  ```julia
  julia> using PkgTemplates
  ```

## Copyright

Author: Luca Ferranti
Codes released under MIT license, text under 