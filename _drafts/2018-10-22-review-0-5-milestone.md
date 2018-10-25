---
layout: post
title: "Review of the 0.5 milestone"
description: "A review of the work carried out during the v0.5 milestone and a look forward to what happens next."
date: 2018-10-25 10:29:00 +0000
categories: workbench
---
## Introduction
After eight months, most of the work for the v0.5 milestone has now been completed. The only work to complete are a couple of bug issues and the completion of the expression error issue.

## User interface
One major change has been the change in direction on the user interface front. Out is the move towards a single screen with model and visualizers. The causes for this were two fold. Firstly, I came to the conclusion that the model graphics didn't add very much. And secondly, the WPF grid control was giving me a lot of problems with focus. In other words, I would have needed to scrap the grid control as the display part of the table visualizer. I did not have the time to do that. So I came to the conclusion that a single display wasn't going to work. I therefore scrapped the single editor screen and split the relevant editors and solution out into a tabbed interface.

The model editor now occupies its own tab, as does the solution display and the various visualizers like table and chessboard.

## Rich domains
The addition of rich domains has turned into one of the most useful additions to the Workbench in a long time.

Instead of modeling your problem using just numbers, you can now use something that probably makes a lot more sense to you like green, blue or Julia. Numbers are still used underneath the hood to solve the model, but you don't have to worry about that.

## Table cell text
One of the more interesting features implemented during the v0.5 milestone has been the addition of cell property expressions. I am no fan of the binding expressions and wondered how they could eventually be replaced. One possible solution is to bind an expression to various properties inside the visualizers. The only property that is currently implemented is the *Text* property inside a table cell. In due course, many properties in the table and chessboard should be editable in a similar way to the *Text* property of an individual table cell.

## Document format
The old document serialization mechanism has been replaced by an XML based file format. This has largely been motivated by a desire for a format that is much easier to retain backwards compatibility. As you can imagine, I am getting pretty tired of typing the same variable names and domain expressions during testing. From now on, I want to have a file format that I know I can keep updating with new features but not lose backward compatibility with existing files.

## External data
If the Workbench is to be of any use, it will need to be able to process external data in various formats. To this end I have begun the process by adding the ability to use the table visualizer as a store of external data in quite simple ways. I expect that in due course future releases will greatly increase the Workbench's ability to work with external data in many different ways. At the moment the only thing the Workbench is able to do is take a domain's values from a range of cells inside a table.

## Model validation
There have been a lot of changes to the various mini-languages lurking inside Workbench. As of the v0.5 milestone, the following mini-languages exist:

+ constraint expressions
+ all different expressions
+ variable domain expressions
+ shared domain expressions
+ property binding expressions
+ visualizer binding expressions

Unfortunately, the model validator has not kept up with the many changes to these languages over the last year or two. This milestone includes some improvements to ensure that the model is sufficiently valid that the solver can make a reasonable job of producing a solution. When the model is not valid, a list of relatively easy to understand error messages are displayed.

In addition, the error status should be displayed inline with the model.

## What's next...
