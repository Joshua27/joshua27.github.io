---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Dr. rer. nat. in Computer Science, University of Düsseldorf, 2023 (magna cum laude)
* M.S. in Computer Science, University of Düsseldorf, 2017
* B.S. in Computer Science, University of Düsseldorf, 2015

Work experience
======
* October 2017 until today: Researcher
  * Employer: University of Düsseldorf
  * Duties included: Research and teaching in formal methods, software engineering and artificial intelligence
  * Used skills: Scientific research and presentation, Java, Kotlin, Python, Prolog, C++, software testing, SMT-LIB, Z3, B-Method, Alloy, formal modeling, tensorflow, deep learning and computer vision 
  * Supervisor: Prof. Dr. Michael Leuschel

* September 2021 until December 2023: Technical Lead
  * Employer: University of Düsseldorf
  * Duties included: Project management and reporting, software development, data science and artificial intelligence
  * Project: "VertiGo", funded by the Federal Ministry of Education and Research
  * Website: 
    * [https://www.interaktive-technologien.de/projekte/vertigo](https://www.interaktive-technologien.de/projekte/vertigo)
    * [https://vertigo.stups.hhu.de](https://vertigo.stups.hhu.de)
  * Used skills: Android, Kotlin, Python, C, C++, software testing, tensorflow, deep learning, computer vision, rule-based expert systems, project management, technical documentation and medical device regulation
  * Supervisor: Prof. Dr. Michael Leuschel
  * joint work with the University Hospital of Düsseldorf, Prof. Dr. med. Dr. h.c. Jörg Schipper

* April 2018 - Juli 2018: Freelance Software Developer
  * Client: Orthomol pharmazeutische Vertriebs GmbH
  * Used skills: Kotlin, MySql, software testing and project management

* August 2016 - September 2017: Software Developer
  * Employer: University of Düsseldorf
  * Project: "Planungswerkzeug für überschneidungsfreies Studieren"
  * Website: [https://plues.github.io](https://plues.github.io)
  * Used skills: Java, JavaFX, software testing and Clojure

Patents
======
* a patent application was filed with the Deutsches Patent- und Markenamt (DPMA) in February 2023 with the file number 10 2023 104 370.6 and the title "Verfahren zum Erfassen und Auswerten der Pupillenbewegungen eines Lebewesens, mobiles Gerät, Computerprogrammprodukt und computerlesbares Medium"
* a PCT application to internationalize the above patent application was filed in February 2024

Skills
======
- languages
  - German, native
  - English, fluent
- software development
  - Java, JavaFX, Kotlin, Android
  - Python
  - Dart, Flutter
  - Prolog
  - C, C++
  - databases, SQL
  - constraint programming
  - Git, continuous deployment
- software testing
  - unit, widget and integration testing
  - End-to-End testing
  - fuzzing
  - mutation testing
  - Modified condition/decision coverage
  - continuous integration
- artificial intelligence
  - computer vision: object detection, augmented reality, face- and eye-tracking
  - supervised learning: deep learning, decision trees and random forests
  - unsupervised learning: clustering
  - rule-based expert systems
  - fairness-aware machine learning
  - explainable AI (XAI)
  - constraint solving
- formal software modeling
  - B-Method
  - Alloy
  - SMT-LIB, Z3
- technical software documentation
- medical device regulation (MDR)

Projects
======
  <ul>{% for post in site.portfolio %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
