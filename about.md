---
layout: about
title: "About"
---

{% assign dateStart = '15-05-1997' | date: '%s' %}
{% assign nowTimestamp = 'now' | date: '%s' %}
{% assign diffSeconds = nowTimestamp | minus: dateStart %}
{% assign diffDays = diffSeconds | divided_by: 3600 | divided_by: 24 | divided_by: 365 %}

Hello, my name is **Göktuğ Öcal** and I am {{ diffDays }} years old **Data Scientist** from Istanbul. This is a personal blog about my interests.

These days, I’m exploring the intersection of industrial systems and intelligent algorithms as a Data Scientist at [**Daikin Europe N.V.**](https://www.daikin.eu/en). My work focuses on leveraging data to drive innovation in sustainable climate solutions.

My perspective is shaped by a deep background in rigorous engineering. Before moving into applied data science, I specialized in bridging the gap between physical dynamics and software logic, earning my M.S. in Computer Engineering from [**Bogazici University**](http://www.boun.edu.tr/en-US/Index) and my B.S. in Control & Automation Engineering from [**Istanbul Technical University**](https://www.itu.edu.tr/en/homepage).

<!-- I am a **MSc student in Computer Engineerging** program of [**Bogazici University**](http://www.boun.edu.tr/en-US/Index) and I a recently working as a **Data Scientist** at [**Ford Otosan**](https://www.fordotosan.com.tr/en). I have graduated from Control and Automation Engineering undergraduate program of [**Istanbul Technical University**](https://www.itu.edu.tr/en/homepage). -->