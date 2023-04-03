---
layout: page
title: Home
permalink: /
---

Welcome on my website! I am a PhD Candidate at the
[Programming Language Group](http://pl.ewi.tudelft.nl) at
[Delft University of Technology](http://www.tudelft.nl). Initially being
supervised by [Prof.Dr. Eelco Visser](http://eelcovisser.org)<sup>♱</sup>, I am
now supervised by [Prof.Dr. Arie van Deursen](https://avandeursen.com/) and
co-supervised by [Dr. Casper Bach Poulsen](http://casperbp.net/).

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

This work is in collaboration with [Hendrik van Antwerpen](https://hendrik.van-antwerpen.net),
and has resulted in a publication at [OOPSLA'22](/publications#journal-articles).


### Resolution Query Compilation

A significant part of the runtime of a Statix-based type checker is used for
name resolution queries (35 - 40%). Therefore, I am researching opportunities
for specification compile-time optimization of queries that reduce the overhead
of query resolution when analyzing an object language program.

This research has resulted in a publication at [SLE'22](/publications#conference-papers).


### Reference Retention

When moving code, references in the moved fragment can become unbound, or be
captured by another definition. In this project we are exploring how scope graph
can help fixing references automatically, for example by adding qualifiers. A
sound solution to this problem can become the backbone of robust
language-parametric transformations.

This work is in collaboration with [Daniël Pelsmaeker](https://pelsmaeker.net/).


### Incremental Unification

Many type checkers use constraints on first-order terms to implement type
inference. It is well-known how to do that efficiently using disjoint-set data
structures. However, this structure does not admit _incremental_ analysis, as
it is not possibly to 'undo' constraints (in non-linear order). This project
investigates how to support 'undo' operations efficiently.


## Teaching

I have been involved in teaching in the following ways:
- Teaching Assistant at the 2021 edition of the _Language Engineering Project_ course.
- Teaching Assistant at the 2021 edition of the _Compiler Construction_ course.
- Supervisor in the 2023 edition of the _Bachelor End Project: Building Type Checkers Using Scope Graphs_ (with [Casper Bach Poulsen](http://casperbp.net/)).
- Supervisor in the 2023 edition of the _Bachelor End Project: Literature survey on implementation techniques for type systems_ (with [Jesper Cockx](https://jesper.sikanda.be/)).

Morover, I am supervising two master theses:
- Boris Janssen on [_Bootstrapping Statix_](http://pl.ewi.tudelft.nl/master-projects/master/2021/05/15/bootstrapping-and-generics-in-statix/).
- [Jonathan Brouwer](http://jonathanb.nl) on [_Expressing Dependent Types in Statix_](http://pl.ewi.tudelft.nl/master-projects/master/2022/02/18/dependent-types-in-statix/) (together with [Jesper Cockx](https://jesper.sikanda.be/)).

Moreover, starting from spring 2023, I am looking for a master student to
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
