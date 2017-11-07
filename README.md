# Scientific Computing (for the rest of us)

<p align="center">
    <b><a href="https://gitter.im/ScientificComputingForTheRestOfUs/Lobby" title="Chat room">Come talk with us on gitter</a>!</b>
</p>

One specific challenge, when writing code as a scientist, is that we care *a
lot* about getting the *right* answer; but of course, the *right* answer is not
always obvious. So we should be very careful with the code we write. A piece of
code that crashes is annoying; but a piece of code that runs, and give you the
wrong answer can compromise your science and your career. This guide will help
you adopt practices that make it less likely to introduce mistakes in your code,
and more likely to catch them. Hopefully, this will let all of us write code we
can trust more.

Good principles in scientific computing can help you write code that is easier
to maintain, easier to reproduce, and easier to debug. But it can be difficult
to find an introduction to get you started. The goal of this project is to
provide reproducible documents you can use to get started on the most important
points. You can use these lessons on your own, or as a group.

This material is aimed at people who have already interacted with a computer
using a programming language, but want to adopt best practices that make their
code more robust. It can also be used to facilitate the onboarding of new people
in your lab or in your project.

Scientific computing can be very diverse, ranging from a few-step analysis
of small data sets to simulations running for weeks on supercomputers.
We focus on the most common situations that every scientist encounters
at some stage of a research project: data analyses performed on a standard
desktop computer. The general ideas and principles that we expose carry over
to other situations as well, but the concrete tools and methods may not
be suitable for tasks requiring special hardware such as GPUs or supercomputers,
or for projects requiring a significant software development effort.

And do you want good news? You don't need to install anything! We rely on [the
Binder project][binder], a cloud-based service to run reproducible documents. We
will use the [Julia][jl] language; but you don't need to know anything about it
either. We will keep the discussion very general, and not use any of the (very
cool!) language-specific features and syntax.

In fact, you will see that good practices for scientific computing have very
little to do with tools and technical things; instead, they rely on thinking
about programming in a slightly different way. You will be able to apply these
principles to any language you prefer to use.

[binder]: https://beta.mybinder.org/
[jl]: http://julialang.org/

## Table of contents

### :notebook: [Lesson 1][l1binder] - using notebooks

- :checkered_flag: [Start the lesson!][l1binder]
- :triangular_flag_on_post: [Report issues or give feedback][l1issues]
- Contents:
    1. cells and states
    2. order of execution
    3. exporting and saving your work
- :clock1: approx. 10 minutes

### :arrows_clockwise: [Lesson 2][l2binder] - the flow of execution

- :checkered_flag: [Start the lesson!][l2binder]
- :triangular_flag_on_post: [Report issues or give feedback][l2issues]
- Contents:
    1. programming as a language (with only three words!)
    1. if, for, while - what do they do?
    1. arrays
    1. moving across loops
- :clock1: approx. 25 minutes
- :information_source: early draft

### :computer: Lesson 3 - writing functions

- Contents:
    1. advantages of modular code
    1. writing functions (and commenting them)
    1. arguments
    1. type stability

### :bug: Lesson 4 - preventing errors with defensive programming

- Contents:
    1. defensive programming
    1. using types as input control
    1. testing

### :hammer: Lesson 5 - debugging our way out of errors we forgot to prevent

- Contents:
    1. using print
    1. debugging strategies
    1. messages, warnings, and errors

[l1binder]: https://beta.mybinder.org/v2/gh/tpoisot/ScientificComputingForTheRestOfUs/master?filepath=lessons%2F01_introduction_to_notebooks.ipynb
[l2binder]: https://beta.mybinder.org/v2/gh/tpoisot/ScientificComputingForTheRestOfUs/master?filepath=lessons%2F02_flow_of_execution.ipynb

[l1issues]: https://github.com/tpoisot/ScientificComputingForTheRestOfUs/issues?q=is%3Aopen+is%3Aissue+label%3Alesson%3A1
[l2issues]: https://github.com/tpoisot/ScientificComputingForTheRestOfUs/issues?q=is%3Aopen+is%3Aissue+label%3Alesson%3A2
[l3issues]: https://github.com/tpoisot/ScientificComputingForTheRestOfUs/issues?q=is%3Aopen+is%3Aissue+label%3Alesson%3A3
[l4issues]: https://github.com/tpoisot/ScientificComputingForTheRestOfUs/issues?q=is%3Aopen+is%3Aissue+label%3Alesson%3A4
[l5issues]: https://github.com/tpoisot/ScientificComputingForTheRestOfUs/issues?q=is%3Aopen+is%3Aissue+label%3Alesson%3A5

## Contributing

There are a number of ways to contribute. Before you start, please have a look
at our [Code of Conduct][coc]. It boils down to *be nice and respectful* -- no
contribution, no matter how amazing it may be, justifies or excuses bad
behaviour.

[coc]: https://github.com/tpoisot/ScientificComputingForTheRestOfUs/blob/master/CODE_OF_CONDUCT.md

The first thing you can do is comment on Issues that have the ["Request for
feedback"][feedback] label. They represent situations for which we are actively
seeking community feedback, and anyone is always welcome to chime in.

[feedback]: https://github.com/tpoisot/ScientificComputingForTheRestOfUs/labels/request%20for%20feedback

If you are not sure about opening an issue, you can use the
[chatroom][gitterlink]. We'll be glad to have a more informal conversation with
you!

[gitterlink]: https://gitter.im/ScientificComputingForTheRestOfUs/Lobby

If there is a more specific point you would like to raise, you can [create a new
Issue][new_issue], and explain your idea, critique, or comment. And of course,
you can always browse the [current Issues][issues], to get a sense of what is
being discussed.

[new_issue]: https://github.com/tpoisot/ScientificComputingForTheRestOfUs/issues/new
[issues]: https://github.com/tpoisot/ScientificComputingForTheRestOfUs/issues

If you want to contribute more, then great! Have a look at the [contribution
guidelines][cguid] first, to get you started with setting up a development
environment. You can have a look at ["Good first issues"][first], if you want
some inspiration.

[cguid]: https://github.com/tpoisot/ScientificComputingForTheRestOfUs/blob/master/CONTRIBUTING.md
[first]: https://github.com/tpoisot/ScientificComputingForTheRestOfUs/labels/good%20first%20issue

## Contributors

**Comments, ideas, feedback**: Hao Ye, Philipp Bayer, Tim Head, Ethan White

## Want to read more?

In a rush? Yes you are. We suggest ["Good enough practices in scientific
computing"][goodenough] to get you started.

A little bit more time? We think ["Best practices in scientific
computing"][best] might suit you.

Want a more complete thing to read? ["The pragmatic programmer"][pragm] is a
masterpiece. I have also heard great things about ["Clean code"][cleanc].

If you still have some time, you can read something about [ways to improve user confidence
in your software][userconf], or ways to [elevate code as a research output][elevate].

[userconf]: https://queens.scholarsportal.info/ojs-archive/index.php/IEE/article/download/5644/5463
[elevate]: http://www.cell.com/trends/ecology-evolution/abstract/S0169-5347(15)00290-6

[goodenough]: http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1005510
[best]: http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001745
[pragm]: https://www.amazon.ca/Pragmatic-Programmer-Journeyman-Master/dp/020161622X/ref=as_li_ss_tl?ie=UTF8&linkCode=sl1&tag=&linkId=0ff8cca36522d8539b26e536778bbb5e
[cleanc]: https://www.amazon.ca/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882

## Other information

[![license](https://img.shields.io/github/license/tpoisot/ScientificComputingForTheRestOfUs.svg?style=flat-square)]()
[![Binder](https://img.shields.io/badge/launch-binder-ff69b4.svg?style=flat-square)](https://beta.mybinder.org/v2/gh/tpoisot/ScientificComputingForTheRestOfUs/master?filepath=lessons)
[![Gitter](https://img.shields.io/gitter/room/ScientificComputingForTheRestOfUs/Lobby.svg?style=flat-square)](https://gitter.im/ScientificComputingForTheRestOfUs/Lobby)
