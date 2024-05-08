---
title: "Improving SMT Solver Integrations for the Validation of B and Event-B Models"
collection: publications
permalink: /publication/prob-smt-2021
excerpt: 'In this paper, we substantially improve the translation from B to SMT-LIB by employing a more constructive rather than axiomatised style using Z3’s lambda functions. We further extend ProB’s interface to Z3 to run different solver configurations in parallel, e.g., either using the former or new translation.'
date: 2021-08-19
venue: 'Proceedings FMICS (International Conference on Formal Methods for Industrial Critical Systems)'
paperurl: 'https://link.springer.com/chapter/10.1007/978-3-030-85248-1_7'
citation: 'Joshua Schmidt and Michael Leuschel. (2021). &quot;Improving SMT Solver Integrations for the Validation of B and Event-B Models&quot; <i>Proceedings FMICS (International Conference on Formal Methods for Industrial Critical Systems)</i>.'
---

ProB provides a constraint solver for the B-Method written in Prolog and optionally can make use of different backends based on SAT or SMT solving. One such solver integration translates B and Event-B operators to SMT-LIB using the C interface of the Z3 solver. This translation uses quantifiers to axiomatise operators when translating to SMT-LIB, which are not well-handled by Z3. Several relational constraints such as the transitive closure are not supported since their translations were too involved.
In this paper, we substantially improve the translation to SMT-LIB by employing a more constructive rather than axiomatised style using Z3’s lambda functions. Thereby, we are able to translate more set-theoretic B and Event-B operators to SMT-LIB, and improve the overall performance. We further extend ProB’s interface to Z3 to run different solver configurations in parallel, e.g., either using the former or new translation. Empirical results show that the new translation to SMT-LIB and the parallel integration of different configurations of the Z3 solver have improved the performance of constraint solving.

The paper was nominated for the best paper award.