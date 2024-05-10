---
title: "PlÜS - Scheduling Tool for overlapping-free studying"
excerpt: "PlÜS is a timetable validation tool created with the goal of importing, validating and improving existing university timetables at the University of Düsseldorf. This project was an interdisciplinary joint work with the Faculty of Arts and Humanities at the University of Düsseldorf.<br/><br/><img width='30%' src='/images/plues.png'>"
collection: portfolio
---

The central feature of PlÜS is to validate the feasibility of timetables from a student’s perspective. In other words, the tool tries to decide if, based on the given data, it is possible to achieve a degree in the timeframe (e.g. four or six semesters) prescribed by the curriculum without having to attend two classes at the same time.

<img width='100%' src='/images/plues-timetable.png'>

# Features

The main features of the PlUES tool are to:
- check the feasibility of:
    - a single course
    - all courses at once
- generate PDF-timetables for:
    - a single feasible course
    - all courses at once
- detect a conflict source for infeasible courses.

# Architecture

The core validation logic is implemented using the B-Method and the ProB tool. The B model describes the constraints a curriculum must satisfy in order to be feasible for a student. ProB is used to solve these constraints and search for valid timetables that satisfy the curriculum rules.

# How it works

The tool provides a complete semester overview of all courses offered at a faculty. Individual courses can be postponed within one semester, and special study program combinations can then be tested for the possibility of studying. If a computational combination can be studied, one is able to create a specific curriculum as a PDF file. If students have special emphasis on the presentation of individual courses or have already completed them, it is also possible to take this into account when calculating the course of studies and to create a partial curriculum. Furthermore, all existing combinations can be checked automatically, or all curricula that are possible to study can be generated. Possible temporal conflicts and overlaps of individual courses and modules can be automatically identified during planning. In addition, such conflicts can be calculated step by step, allowing the user to more closely examine the cause of the conflict and thus make it easier to resolve them.

The data of a course is defined in the XML format. Using the provided Mincer tool, a corresponding SQLite database can be generated from this data. PlüS also offers a static analysis of the data of a course of studies. Here, errors in the data that lead to a course that can not be studied as required are described in a report. The report is divided into numerous categories so that the incorrect data can be identified as easily as possible and thus corrected. The report can also be exported as a PDF file and printed as required.

The planning tool is currently being used by the Faculty of Arts and Humanities, the Faculty of Business Administration and Economics and the Computer Science Department at the Faculty of Mathematics and Natural Sciences at the University of Düsseldorf.

For more information visit [https://plues.github.io/](https://plues.github.io/)
