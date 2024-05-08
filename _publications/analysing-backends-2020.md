---
title: "Analysing ProB&apos;s Constraint Solving Backends"
collection: publications
permalink: /publication/analysing-backends-2020
excerpt: 'We evaluate the strengths and weaknesses of different backends of the ProB constraint solver. For this, we train a random forest over a database of constraints to classify whether a backend is able to find a solution within a given amount of time or answers unknown.'
date: 2020-05-22
venue: 'Proceedings ABZ (International Conference on Rigorous State Based Methods)'
paperurl: 'https://link.springer.com/chapter/10.1007/978-3-030-48077-6_8'
citation: 'Jannik Dunkelau, Joshua Schmidt and Michael Leuschel. (2020). &quot;Analysing ProB&apos;s Constraint Solving Backends&quot; <i>Proceedings ABZ (International Conference on Rigorous State Based Methods)</i>.'
---

We evaluate the strengths and weaknesses of different backends of the ProB constraint solver. For this, we train a random forest over a database of constraints to classify whether a backend is able to find a solution within a given amount of time or answers unknown. The forest is then analysed in regards of feature importances to determine subsets of the B language in which the respective backends excel or lack for performance. The results are compared to our initial assumptions over each backend's performance in these subsets based on personal experiences. While we do employ classifiers, we do not aim for a good predictor, but are rather interested in analysis of the classifiers' learned knowledge over the utilised B constraints. The aim is to strengthen our knowledge of the different tools at hand by finding subsets of the B language in which a backend performs better than others.
