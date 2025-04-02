---
layout: default
title: Research
weight: 1
group: research
---

I am a Ph.D. candidate in Computer Software Engineering from University of British Columbia under the supervision of Dr. Ali Mesbah. My research focuses on utilizing large language models (LLMs) and deep learning techniques to automate the End-to-End (E2E) software testing process.

Below is a list of my current and inactive projects.

### Current Projects
{% assign current = site.data.projects | where_exp: "project", "project.end == nil" %}
{% include projects.html data=current %}

### Inactive Projects
{% assign inactive = site.data.projects | where_exp: "project", "project.end != nil" %}
{% include projects.html data=inactive %}
