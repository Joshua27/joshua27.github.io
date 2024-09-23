---
title: "ProBramSynthesis - Program Synthesis for B in ProB"
excerpt: "In this project, I implemented a program synthesis technique in ProB using constraint logic programming for the interactive repair and generation of formal models including a graphical user interface.<br/><br/><img width='30%' src='/images/bsynthesis-example.png'>"
collection: portfolio
---

Program synthesis is the task of generating executable programs from a specification usually considering a domain specific language. There are many ways to specify the behavior of a program to be synthesized such as natural language, logical or mathematical formulas (e.g., in the form of pre- and post-conditions) or explicit input-output examples (called Inductive Program Synthesis or Programming by Examples).

The ProB Prolog core provides an implementation to synthesize B predicates or complete machine operations from explicit-state input-output examples. The ProB Java API provides an interface to utilize the program synthesis backend. The implemented synthesis technique is based on the work by [Susmit Jha, Sumit Gulwani et al.](https://people.eecs.berkeley.edu/%7esseshia/pubdir/icse10-TR.pdf). 
A synthesis task is encoded as a constraint satisfaction problem in B using the ProB constraint solver and its available backends to find valid solutions.

This work originates from my master's thesis at the chair of software engineering and programming languages at the University of Düsseldorf.

An exemplary use of program synthesis using ProB's Java API can be found on Github: [https://github.com/Joshua27/ProBramSynthesis](https://github.com/Joshua27/ProBramSynthesis)

Besides the actual implementation of program synthesis using constraint logic programming and the integration in ProB, I implemented a graphical user interface for the interactive repair and generation of formal models using ProB's Java API and JavaFX.

In the following, we can see a visualization of a trace of state changes (green side on the left) that leads to a state violating the invariant (red side on the right). The user can then decide whether the state violating the invariant should be removed from the model by synthesizing a stronger precondition for the operation leading to that invariant violating state, or to make the state valid by synthesizing a relaxed invariant.

<center><img width='90%' src='/images/bsynthesis-example.png'></center><br>

The GUI can be found on Github: [https://github.com/Joshua27/BSynthesis](https://github.com/Joshua27/BSynthesis)
