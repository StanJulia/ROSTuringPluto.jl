# ROSTuringPluto

![Lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)<!--
![Lifecycle](https://img.shields.io/badge/lifecycle-maturing-blue.svg)
![Lifecycle](https://img.shields.io/badge/lifecycle-stable-green.svg)
![Lifecycle](https://img.shields.io/badge/lifecycle-retired-orange.svg)
![Lifecycle](https://img.shields.io/badge/lifecycle-archived-red.svg)
![Lifecycle](https://img.shields.io/badge/lifecycle-dormant-blue.svg) -->

## Purpose

This project will contain (work is in very early stages of progress!!!) a set of Pluto notebooks that contain Julia versions of the examples in the R project `ROS-Examples` based on the book ["Regression and Other Stories" by A Gelman, J Hill and A Vehtari](https://www.cambridge.org/highereducation/books/regression-and-other-stories/DD20DD6C9057118581076E54E40C372C#overview).

These notebooks are intended to be used in conjunction with above book.

## Personal note

This project will take quite a while to complete, I expect at least a year. But it has a special meaning to me: When I started to work on Julia interfaces for Stan's cmdstan binary in 2011, I did that to work through the ["ARM" book](http://www.stat.columbia.edu/~gelman/arm/). The ["ROS" book](https://www.cambridge.org/highereducation/books/regression-and-other-stories/DD20DD6C9057118581076E54E40C372C#overview) in a sense the successor to the ARM book.

I will document the progress in the table of content (TOC.md).

## Prerequisites

1. A functioning [Julia](https://julialang.org/downloads/).
2. A Julia base environment containing `Pkg`, `DrWatson`, `Pluto` and `PlutoUI`.
3. Turing.jl.

## Setup the Pluto based ROSTuringPluto notebooks

To (locally) use this project, do the following:

Select and download ROSTuringPluto.jl from [StanJulia on Github](https://github.com/StanJulia/), e.g. to clone it to the `~/.julia/dev/ROSTuringPluto` directory:
```Julia
$ git clone https://github.com/StanJulia/ROSTuringPluto.jl ~/.julia/dev/ROSTuringPluto
$ cd ROSTuringPluto # Move to the downloaded directory
$ julia --project=ROSTuringPluto # Available from Julia-1.7 onwards.
(ROSTuringPluto) pkg> activate .
(ROSTuringPluto) pkg> instantiate     # Only the first time
```

Still in the Julia REPL, start a Pluto notebook server.
```Julia
julia> using Pluto
julia> Pluto.run()
```

A Pluto page should open in a browser. See [this page](https://www.juliafordatascience.com/first-steps-5-pluto/) for a quick Pluto introduction.

## Usage

Select a notebook in the `open a file` entry box, e.g. type `./` and step to e.g. `./notebooks/01/02/hibbs.jl`, the first notebook from the book.

The code examples are organized in subdirectories according to  chapter/section/example, e.g. `01/02/hibbs.jl`.

See [TIPS](https://github.com/StanJulia/ROSTuringPluto.jl/blob/master/TIPS.md) for some more details or file an [issue](https://github.com/StanJulia/ROSTuringPluto.jl/issues) if any difficulties are encountered with above steps.