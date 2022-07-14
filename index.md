---
layout: page
title: Home
permalink: /
---

Welcome on my website! I am a PhD Candidate at the
[Programming Language Group](http://pl.ewi.tudelft.nl) at
[Delft University of Technology](http://www.tudelft.nl). I was supervised by
[Prof.Dr. Eelco Visser](http://eelcovisser.org)<sup>♱</sup> and co-supervised by
[Dr. Casper Bach Poulsen](http://casperbp.net/).

## Research

My research focusses on deriving industry-quality type checkers from declarative
type system specifications. In particular, I am evaluating and improving the
operational aspects of [_Statix_](https://github.com/metaborg/nabl), while
collaborating with others to use typing results of Statix to develop
language-parametric transformations and editor services.

### Incremental Type Checking

I am currently working on improving the performance of the [concurrent _Statix_
solver](https://github.com/metaborg/nabl) by making it automatically incremental.
The goal of this work is to develop a framework for incremental type checkers that is:
- Language-independent: supports a wide range of name binding patterns.
- Type-checker paradigm independent: not bound to a particular type checker
  implementation strategy, such as constraint programming.
- Minimizes the effort type-checker writers need to incrementalize their type checkers.
- Sound and precise.

This work is in collaboration with [Hendrik van Antwerpen](https://hendrik.van-antwerpen.net).

### Resolution Query Compilation

A significant part of the runtime of a Statix-based type checker is used for
name resolution queries (35 - 40%). Therefore, I am researching opportunities
for specification compile-time optimization of queries that reduce the overhead
of query resolution when analyzing an object language program.

### Reference Retention

When moving code, references in the moved fragment can become unbound, or be
captured by another definition. In this project we are exploring how scope graph
can help fixing references automatically, for example by adding qualifiers. A
sound solution to this problem can become the backbone of robust
language-parametric transformations.

This work is in collaboration with [Daniël Pelsmaeker](https://pelsmaeker.net/).

## Teaching

I have been involved in teaching in the following ways:
- Teaching Assistant at the 2021 edition of the _Language Engineering Project_ course.
- Teaching Assistant at the 2021 edition of the _Compiler Construction_ course.

Moreover, starting from november 2023, I am looking for a master student to
collaborate with. Especially, I want add parametric polymorphism and (a limited
form of) higher-order constraints to [Statix](http://www.spoofax.dev/references/statix/).
That will significantly improve the user experience of Statix, as it allows
removal of a lot of duplication in language specifications. I expect this project
to be interesting, varied (involving design, implementation and evaluation) and
certainly doable.

## Contact

When you are interested in a teaching or research project, have another idea
for collaboration, or just have a question, feel free to drop a line. My contact
details are shown on the left of this page.
