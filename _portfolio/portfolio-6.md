---
title: "Fuzzing of Prolog Programs"
excerpt: "In this project, I implemented a fuzzer for SICStus Prolog including an extension to generate classical B and Event-B predicates and expressions represented as abstract syntax trees.<br/><br/><img width='30%' src='/images/b-ast.png'>"
collection: portfolio
---

Nowadays, the security of software is of high importance, especially due to the increased global networking and increased exploitation of security gaps.
Software errors discovered after a software release can cost a company a lot of money and time.
This risk should thus be minimized.
As pointed out in the article ["How to Prevent the next Heartbleed"](https://dwheeler.com/essays/heartbleed.html), the "Heartbleed" security hole in the OpenSSL software, which was announced by the responsible developers in April 2014, could have been found using fuzzing methods. The extent of this security vulnerability was enormous and affected a large number of the world's most famous websites such as Google, Yahoo!, YouTube and Stack Overflow.

Continuous testing of software is therefore essential and forms the basis of a successful release.
Black box testing offers a way to evaluate the functionality of a software without having information about more precise program structures.
This includes the so-called fuzzing, in which a large number of randomly generated data are processed automatically using the system under test.
Fuzzing makes it possible to find data that lead to an error and thus possibly represent a security gap, as well as to gain a certain level of trust in your own software by running a large number of randomly generated tests.
A fuzzer is usually able to generate a wide variety of test data, including corner cases that one would probably not think of when writing unit tests.

<center><img width='60%' src='/images/b-ast.png'></center><br>

The aim of this work was to implement a fuzzer for SICStus Prolog, which generally checks Prolog programs for robustness, but also specifically supports some of the data types used in ProB. This means that additional test methods can be integrated into ProB's kernel to examine its functionality and stability.
Particular attention was paid to:
- easy integration into any Prolog programs
- covering a diverse range of data types
- individual and targeted generation of data
- a high degree of flexibility in terms of expanding with additional data types

The code can be found on Github: [https://github.com/Joshua27/SICStusPrologFuzzer](https://github.com/Joshua27/SICStusPrologFuzzer)
