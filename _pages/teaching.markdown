---
layout: single
title: Teaching
permalink: /teaching
lang: en
lang-ref: teaching
author_profile: true
toc: true
toc_sticky: true


header:
  image: /assets/images/teaching/teaching3.jpg
  caption: "Photo credit: [**Sharon McCutcheon**](https://unsplash.com/@sharonmccutcheon?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [**Unsplash**](http://unsplash.com/)"

---

 <!-- image 2 caption: "Photo credit: [**Ivan Aleksic**](https://unsplash.com/@ivalex?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [**Unsplash**](http://unsplash.com/)" -->

<!-- semester is named as b{{ curentYear }}1 or 2 (winter or summer). Current year begins in september and ends in august (e.g. june 22 has currentyear 21) -->
{% capture currentMonth %}
  {{ 'now' | date: '%m' }}
{% endcapture %}
{% assign currentMonth = currentMonth | plus: 0 %}
{% capture currentYear %}
  {{ 'now' | date: '%y' }}
{% endcapture %}
{% if currentMonth < 9 %}
  {% assign currentYear = currentYear | minus: 1 %}
{% endif %}

<!-- Beginning of text -->

Semantic Web and Enterprise architectures are the main focus of our group. This reflects in the topics KBSS members offer for [bachelor and master thesis](#bachelor-and-master-theses) and our [main teaching activities](#main-teaching-activities). In addition, we [participate in the teaching](#support-teaching-activities) of Software Architectures and Database Systems.

## Main Teaching Activities

We are the guarantors of the following subjects.

###  Ontologies and Semantic Web (B4M36OSW)

The course guides students through current trends and technologies in the semantic web field. It takes place in the winter semester.

[Subject description from the faculty web](https://fel.cvut.cz/en/education/bk/predmety/58/33/p5833706.html){: .btn .btn--info}
[Details for students at CourseWare](https://cw.fel.cvut.cz/b{{ currentYear }}1/courses/b4m36osw/start){: .btn .btn--info}

### Enterprise Architecture (B6B36EAR)

The course offers an overview of the development of web and enterprise information systems. The practical part of the course focuses of Spring.
The course takes place in the winter semester.

[Subject description from the faculty web](https://fel.cvut.cz/en/education/bk/predmety/58/33/p5833906.html){: .btn .btn--info}
[Details for students at CourseWare](https://cw.fel.cvut.cz/b{{ currentYear }}1/courses/b6b36ear/start){: .btn .btn--info}

## Support Teaching Activities

In the following subjects, we just help with teaching, subjects are guaranteed by someone else.

### Software Architectures (BE4M36SWA)

In this course students become familiar with the general requirements for software architecture and related quality parameters. Takes place in summer semester.

[Subject description from the faculty web](https://fel.cvut.cz/en/education/bk/predmety/48/79/p4879206){: .btn .btn--info}

### Database Systems (B0B36DBS)

The course is designed as a basic database course mainly aimed at the students' ability to design a relational data model and to use the SQL language for data definition as well as for data querying and to choose the appropriate degree of transaction isolation. Takes place in summer semester.

[Subject description from the faculty web](https://fel.cvut.cz/en/education/bk/predmety/50/10/p5010606.html){: .btn .btn--info}
[Details for students at CourseWare](https://cw.fel.cvut.cz/b{{ currentYear }}2/courses/b0b36dbs/start){: .btn .btn--info}

## Bachelor and Master Theses

Topics for student theses are published on the [faculty website](https://fel.cvut.cz/en/education/semestral-projects.html?dept=14), where they may be filtered by title, supervisor etc.
