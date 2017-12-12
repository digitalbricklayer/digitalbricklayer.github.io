---
layout: post
title:  "Constraint Capers Workbench Version 0.4 Milestone"
date:   2017-12-12 14:07:00 +0000
categories: workbench
---
The aim of the 0.4 milestone was to solve the Australian state map colors problem. Solving the map problem did not require any changes to the model. It did require adding a new visualizer in order to display the result.

## Grid Visualizer
A new visualizer was added to the Workbench to display information inside a grid or table. In the case of the Australian map coloring problem, each state is shown down the left hand side and the color allocated to the state in the right column.

## Variable Size
One of the things that was found to be a problem in the model is duplicating a lot of information effectively depending upon the size of an aggregate variable. To reduce this duplication I added a `size` function to the domain and visualizer binding languages.

In the binding language usage would look something like this:

`1..size(cols)`

Where `cols` is the aggregate variable name.

## Solution Viewer
When there is no visualizer present on the solution display, it is very difficult to know what values have been bound to the variables. So, I added a display that is automatically displayed when the solution viewer is displayed to show the values.

## Conclusion
It has taken a long time to implement the 0.4 milestone. Some of the changes have broken some big assumptions in the code. It is providing a great base onto which the 0.5 milestone is being built.