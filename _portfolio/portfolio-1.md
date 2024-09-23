---
title: "The ProB Animator and Model Checker"
excerpt: "ProB is an animator, constraint solver and model checker for the B-Method. The constraint-solving capabilities of ProB can be used for animation, model finding, constraint-based symbolic checking and test-case generation.<br/><br/><img width='30%' src='/images/prob-logo.png'>"
collection: portfolio
---

ProB is an animator, constraint solver and model checker for the B-Method. The constraint-solving capabilities of ProB can be used for animation, model finding, constraint-based symbolic checking and test-case generation.

<center><img width='90%' src='/images/prob2-ui.png'></center><br>

The B language is rooted in predicate logic, arithmetic and set theory and provides support for data structures such as (higher-order) relations, functions and sequences. In addition to the B language, ProB also supports Event-B, CSP-M, TLA+, Alloy, and Z. ProB can be installed within [Rodin](http://sourceforge.net/projects/rodin-b-sharp/). ProB can also be used as a [Jupyter kernel](https://gitlab.cs.uni-duesseldorf.de/general/stups/prob2-jupyter-kernel) to generate interactive notebooks.

ProB is being used within Alstom, ClearSy, Siemens, Thales and several other companies for [data validation](http://www.data-validation.fr/) of complicated properties for safety critical systems. It was used, e.g., for Paris Line 1, Sao Paulo line 4, Barcelona line 9 and many more. ProB is certified T2 SIL4 according to the Cenelec EN 50128 standard for use at Thales. In this [video from the Deutsche Bahn](https://www.youtube.com/watch?v=K6mS6akRmvA) you can see ProB animating a formal B model of the ETCS hybrid-level 3 principles in real-time, controlling two trains. Michael Leuschel and his group have won the first edition of the [AlainColmerauer Prize](https://prologyear.logicprogramming.org/ColmerauerPrize.html) for ProB. For commercial support contact [Michael Leuschel](https://www.cs.hhu.de/lehrstuehle-und-arbeitsgruppen/softwaretechnik-und-programmiersprachen/unser-team/team/leuschel).

During my time at the chair of software engineering and programming languages at the University of Düsseldorf I implemented and improved different parts of ProB including
- a fuzzer for generating B and Event-B constraints including a search for minimal examples (shrinking),
- an interactive workflow for the repair and generation of formal models using program synthesis,
- the support of Alloy models in ProB by translating Alloy to B including different extension of Alloy such as integers or sequences,
- an improved and extended interface to the Z3 SMT solver for solving B constraints,
- a custom conflict-driven clause learning (CDCL(T)) solver for the B-Method using ProB's constraint solver as its theory solver (SMT solving), and
- static symmetry breaking for B and Event-B constraints by computing graph automorphisms including a new C++ interface to Bliss.

For more information visit [https://prob.hhu.de](https://prob.hhu.de).
