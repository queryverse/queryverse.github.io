---
date: 2019-02-13
title: ElectronDisplay.jl v1.0.0 Released
categories:
  - announcement
author: Tony Lian
---

[ElectronDisplay.jl](https://github.com/queryverse/ElectronDisplay.jl) is a package that provides a simple UI based on [Electron](https://electronjs.org/) for displaying plots and tabular data. It works with most plotting packages and almost all data structures that represent tabular data in the Julia ecosystem. The package is a core piece of the [Queryverse](https://github.com/queryverse).

## What is new?
There are a bunch of bugfixes as well as some new features in v1.0.0. The main feature is the [plotgallery](https://github.com/julia-vscode/plotgallery), a frontend used for plot display with TypeScript and react. It support displaying multiple plots in the same window at the same time, even if those plots are of different MIME types. For example, you can display an PNG image and then plot a VegaLite plot, or multiple VegaLite plots, and they would show in a single window instead of opening a new window each time or replacing the old plots:

### Some functionalities in detail
* Press CTRL + C on Windows and Linux or Command + C on macOS to copy the current figure
* Press arrow keys to switch between plots quickly and delete/backspace to remove a graph
* Supports Vega, VegaLite, and several image formats (such as PNG, JPG, and SVG)
* Support viewport-sized plots that resize according to the window size

![Plotgallery screenshot](/assets/blog/images/electrondisplay-screenshot-plotgallery.png)

You can have a look at the detailed update [here](https://github.com/queryverse/ElectronDisplay.jl/releases).

## Contributions are welcomed

[ElectronDisplay.jl](https://github.com/queryverse/ElectronDisplay.jl) is still a new package that needs help from the community to resolve the current issues that it has. In fact, as an apprentice of the [Undergraduate Research Apprentice Program](https://urap.berkeley.edu/) supervised by David Anthoff, I have been working on several issues on this project over the past few weeks after I made the initial pull request. If you are interested in making contributions to the project, you can have a look at [Issues for ElectronDisplay.jl](https://github.com/queryverse/ElectronDisplay.jl/issues), or [Issues for Plotgallery](https://github.com/julia-vscode/plotgallery/issues).