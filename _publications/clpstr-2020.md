---
title: "Towards Constraint Logic Programming over Strings for Test Data Generation"
collection: publications
permalink: /publication/clpstr-2020
excerpt: 'In this paper, we evaluate to what extent constraint logic programming can be used to generate test data, focusing on strings in particular.'
date: 2020-05-05
venue: 'Proceedings WLP (Workshop on (Constraint) Logic Programming)'
paperurl: 'https://link.springer.com/chapter/10.1007/978-3-030-46714-2_10'
citation: 'Sebastian Krings, Joshua Schmidt, Patrick Skowronek, Jannik Dunkelau and Dierk Ehmke. (2020). &quot;Towards Constraint Logic Programming over Strings for Test Data Generation&quot; <i>Proceedings WLP (Workshop on (Constraint) Logic Programming)</i>.'
---

In order to properly test software, test data of a certain quality is needed. However, useful test data is often unavailable because existing or hand-crafted data might not be diverse enough to enable desired test cases. Furthermore, using production data might be prohibited due to security or privacy concerns or other regulations. At the same time, existing tools for test data generation are often limited.
In this paper, we evaluate to what extent constraint logic programming can be used to generate test data, focusing on strings in particular. To do so, we introduce a prototypical CLP solver over string constraints. As case studies, we use it to generate valid IBAN numbers, calendar dates and specific data in JSON.