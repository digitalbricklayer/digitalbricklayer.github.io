---
layout: post
title: "Tips for Working on a Pet Project"
description: "A few tips for working on your pet software project."
date: 2018-01-10 13:28:00 +0000
categories: productivity
---
I work on a pet project for one hour per work day. I stop whatever I'm doing at approximately 5 pm and finish when I need to catch the 6:07 pm bus back home.

Contained in this blog post are a few tips for managing your time and staying productive in such a limited time.

## State of Play
You may be surprised how much you can actually achieve with just one hour per day. It has certainly surprised me. The work just kind of accumulates gradually over time.

I have now been working on my pet project for two and three quarter years off and on. A total of approximately 520 hours. In standard full time working that is around 13 weeks.

The project is written in C# and currently stands at 6,629 SLOCs including unit tests.

## Less Time
If you are prone to perfectionism, you may find that restricting the number hours you have is quite a handy way to circumvent that particular time thief. With just one hour per day, you cannot afford flights of fancy you have to deliver value every time you sit at the keyboard. If you do not, it will become obvious very quickly. Want to port your code over to some fancy new framework, you will lose weeks or months to that. Is the new framework really going to deliver? You'll probably come to the conclusion that it will not.

## Getting Stuck
More precisely, do not get stuck. Getting stuck for one full day on a regular project might lose you one day. On one hour per day, you will lose the best part of two weeks. This will mean that you have to be conservative about the choices that you make. You need good documentation and a means to have problems resolved quickly. Choosing that edgy language / framework nobody knows about is probably not going to work out. Choose mainstream languages and frameworks. You can get help quickly on sites like Stack Overflow. The documentation is likely to exist as well. Anything from a mainstream vendor like Microsoft or Google is also likely to be documented.

## Context Switching
The biggest problem with working in very short bursts in something like software development is that in order to be productive you need a lot of context. What am I trying to achieve? What is the design of this part of the software? etc...

There is no easy solution. But, you will get better at context switching by practicing it. Here are also some hints that may help you.

The last thing you need to do when you are about to finish for the day is to provide yourself with some nice hints for yourself the next time you sit down to work. This becomes more important just before a several day break like a weekend or holiday. The hint could be a failing test or a syntax error to remind you what you were working on. The first thing I do everytime I sit down is run the test suite. If the build fails, I fix it. If a test fails, I fix that.

![Workbench Software Project Screenshot]( {{ "/assets/workbench-software-project.png" | absolute_url }})

I work on my pet project alone but I still act as if I work as part of a team. I use GitHub issue tracker assiduously and track my work in GitHub project. If I don't know what I'm working on, I just look at the project on GitHub and it will tell me which issue is **In Progress**. Due to the fact that I work alone and sparingly, I need an external *memory* of the project to help me speedily get productive each day.

With just one hour per day, you cannot afford more than a few minutes to understand what you are working on and what you need to do next. If you can optimise your daily start then you will go a long way to making your pet project a pleasurable experience.
