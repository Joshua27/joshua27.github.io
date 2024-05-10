---
title: "ConString - A string constraint solver for SWI-Prolog"
excerpt: "In this project, we introduced a new string constraint solver for SWI-Prolog having interfaces to CLP(FD), CLP(B) and CLP(R) for generating strings containing integers, booleans and reals. This project was a joint work with the Niederrhein University of Applied Sciences and the periplus instruments GmbH & Co. KG.<br/><br/><img width='30%' src='/images/clpstr-iban.png'>"
collection: portfolio
---

Gaining test data for software tests is notoriously hard. Typical limitations include lack of properly formulated requirements or the combinatorial blowup causing an impractically large amount of test cases needed to cover the system under test (SUT).
When testing applications such as data warehouses, difficulties stem from the amount and quality of test data available and the volume of data needed for realistic testing scenarios. Artificial test data might not be diverse enough to enable desired test cases, whereas the use of real data might be prohibited due to security or privacy concerns or other regulations, e.g, the ISO/IEC 27001.
In consequence, to properly test applications one often has to resort to artificial test data generation. However, existing tools are limited as they
- generate data that does not cover the desired scenarios,
- are specialized and lack options for configuration and adaptation, and
- generate an amount of data that is unrealistic for the SUT.

In this project, we evaluated to what extent constraint logic programming could be used for test data generation, in particular for generating strings. We are not concerned with software testing itself.

<center><img width='50%' src='/images/clpstr-iban.png'></center><br>

The International Software Testing Qualifications Board (ISTQB) describes test data as data created or selected to satisfy the preconditions and inputs to execute one or more test cases.
Test data may belong to the following categories:
- status data, files or surrounding systems required for a reusable start state,
- input data transferred to a test object during test execution,
- output data returned by a test object after execution,
- production data, which is deducted from the production system.

Production data is often used for testing as it provides obvious test cases and can be gathered easily.
However, using production data does not lead to thorough testing, e.g., it never contains dates in the future.
While production data can be anonymized, it is hard to guarantee that de-anonymization is impossible.
Furthermore, production data may be biased.
Those problems can be solved by generating synthetic data.
The implementation of a test data generator for each specific problem is cumbersome.
One just wants to describe the problem at hand without implementing the actual data generation.
We therefore consider constraint programming to be appropriate for implementing general test data generators.
However, generating synthetic data remains a complex task as it involves thoroughly specifying constraints the data needs to fulfill in order to derive high quality test data.

This project was a joint work of the University of Düsseldorf, the Niederrhein University of Applied Sciences and the [periplus instruments GmbH & Co. KG](https://www.periplus.eu/).

The code can be found on Github: [https://github.com/wysiib/clpstr](https://github.com/wysiib/clpstr)
