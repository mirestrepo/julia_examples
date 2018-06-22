## Plotting with Julia

<span style="font-size:0.6em; color:gray">Isabel Restrepo, PhD</span> |
<span style="font-size:0.6em; color:gray">Brown University</span> |
<span style="font-size:0.6em; color:gray">June 15, 2017</span>

Repository: https://github.com/bcbi/julia_tutorials.git

---
## Libraries
* [Gadfly.jl](https://github.com/GiovineItalia/Gadfly.jl)
* [Plots.jl](https://github.com/JuliaPlots/Plots.jl)
* [PlotlyJS.jl](https://github.com/sglyon/PlotlyJS.jl)
* [PyPlot.jl](https://github.com/JuliaPy/PyPlot.jl)
* [GLVisualize.jl](https://github.com/JuliaGL/GLVisualize.jl)
* [Vega.jl](https://github.com/johnmyleswhite/Vega.jl)


---
## Gladfly.jl

A Julia implementation inspired by the "Grammar of Graphics" and ggplot2.

+++
### Pros:
* Clean look Lots of features
* Flexible when combined with Compose.jl (inset plots, etc)
* Familiar to R users
* Good aesthetics

+++
### Cons:
* Does not support 3D
* Slow time-to-first-plot
* Lots of dependencies
* No interactivity
* Not very extensive documentation. Although because it was one
  of the first, there are discussions

---
### Plots.jl

High-level, powerful library that wraps many plotting backends

+++
#### Pros
* Flexibility - use your favorite backend library to produce your plots
* Consistency - change backend without changing your code
* Smart - use features such as recipes and layouts
* Many Examples
* Recipes for stat plots and fancy subplots

+++
#### Cons
* Ambitious Goal. In some cases some features may not be implemented
* Sometimes its hard to find documentation of how to changes properties

---
## PlotlyJS/Plotly

* Wrapper of plotly.js, a javascript library built on top of d3.js.
* The first one uses local resources, the later the cloud.




+++
### Pros:
* Tons of functionality
* Super configurable
* 2D and 3D
* Mature library
* Interactivity (even when inline)
* Standalone or inline
* Good aesthetics

+++
### Cons:
* No custom shapes
* JSON may limit performance
* Sometime it's difficult to save to file as SVG. (Okay as png and html)
* To save to file requires "plotting front-end", which may not work when working on remote servers
* Silent failures of undefined properties

---
## PyPlot.jl

A Julia wrapper around the popular python package PyPlot (Matplotlib). It uses PyCall.jl to pass data with minimal overhead.

+++
### Pros:
* Tons of functionality
* 2D and 3D
* Mature library
* Standalone or inline
* Well supported in Plots
* Familiar to python users

+++
### Cons:
* Uses python
* Dependencies frequently cause setup issues
* Inconsistent output depending on Matplotlib version

---
## Seaborn.jl

A Julia wrapper around the  python package Seaborn, a high-level visualization library for statistical data analysis

+++
### Pros:
* Tons of functionality
* Great documentation (In Python)
* Easy to use
* Good aesthetics


+++
### Cons:
* Uses python - need to set up Dependencies
* Some of the inputs may need to be imported from Numpy or other python libraries
* No native Julia documentation

---
## Plan for this lecture:

* Compare the basics of PlotlyJS.jl and  Plots.jl
---
### What to explore after this lecture?

* Finish basic exercises for PyPlot and Gadfly
* Seaborn tutorials for [Distributions](http://seaborn.pydata.org/tutorial/distributions.html#distribution-tutorial)
and [Categorical Variables](http://seaborn.pydata.org/tutorial/categorical.html#categorical-tutorial)
* Explore a dataset
