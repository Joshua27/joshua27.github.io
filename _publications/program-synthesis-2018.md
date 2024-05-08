---
title: "Repair and Generation of Formal Models Using Synthesis"
collection: publications
permalink: /publication/program-synthesis-2018
excerpt: 'This paper is the follow-up work regarding the use of program synthesis for the interactive repair and generation of formal models using the B-Method.'
date: 2018-08-09
venue: 'Proceedings ABZ (International Conference on Rigorous State Based Methods)'
paperurl: 'https://link.springer.com/chapter/10.1007/978-3-319-91271-4_6'
citation: 'Joshua Schmidt, Sebastian Krings and Michael Leuschel. (2018). &quot;Repair and Generation of Formal Models Using Synthesis&quot; <i>Proceedings ABZ (International Conference on Rigorous State Based Methods)</i>.'
---

Writing a formal model is a complicated and time-consuming task. Usually, one successively refines a model with the help of proof, animation and model checking. In case an error such as an invariant violation is found, the model has to be adapted. However, finding the appropriate set of changes is often non-trivial.
We propose to partially automate the process by combining synthesis with explicit model checking and implement it in the context of the B method: Guided by examples of positive and negative behavior, we strengthen preconditions of operations or relax invariants of the model appropriately. Moreover, by collecting initial examples from the user, we synthesize new operations from scratch or adapt existing ones.
All this is done using user feedback, yielding an interactive assistant.
In this paper, we present the foundations of this technique, its implementation using constraint solving for B, and illustrate the technique by synthesizing the formal model of a process scheduler.
