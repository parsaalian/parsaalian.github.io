---
layout: default
title: Research
weight: 1
group: research
---

I am a Ph.D. candidate in Computer Software Engineering from University of British Columbia under the supervision of Dr. Ali Mesbah. My research focuses on utilizing large language models (LLMs) and deep learning techniques to automate the End-to-End (E2E) software testing process.

---

### News

<table style="margin-bottom: 15px">
  <tr>
    <td style="vertical-align: top;">Jan,&nbsp;2025</td>
    <td>
    🧑🏻‍💻 I am invited to a review journal articles for <a href="https://www.computer.org/csdl/journal/ts" target="_blank">Transactions on Software Engineering</a>.
    </td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Jan,&nbsp;2025</td>
    <td>
    🎉🎉 Our paper <a href="https://www.computer.org/csdl/proceedings-article/icse/2025/056900a678/251mGE6xELC" target="_blank">Flakidock</a> got accepted at <a href="https://conf.researchr.org/home/icse-2025" target="_blank">ICSE 2025</a>!
    </td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Oct,&nbsp;2024</td>
    <td>
    🎉🎉 Our paper <a href="https://www.computer.org/csdl/proceedings-article/icse/2025/056900a678/251mGE6xELC" target="_blank">AutoE2E</a> got accepted at <a href="https://conf.researchr.org/home/icse-2025" target="_blank">ICSE 2025</a>!
    </td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Oct,&nbsp;2024</td>
    <td>
    🙏🏻 I successfully passed my PhD qualifying exam. Thanks to my advisor Dr. Ali Mesbah for everything.
    </td>
  </tr>
  <tr>
    <td style="vertical-align: top;">Sep,&nbsp;2024</td>
    <td>
    🎙️ I gave a talk at <a href="https://conf.researchr.org/home/issta-2024" target="_blank">ISSTA 2024</a> on <a href="https://dl.acm.org/doi/abs/10.1145/3650212.3680332" target="_blank">Automated Web Form Testing</a>.
    </td>
  </tr>
  <tr>
    <td style="vertical-align: top;">May,&nbsp;2024</td>
    <td>
    🎉🎉 Our paper <a href="https://dl.acm.org/doi/abs/10.1145/3650212.3680332" target="_blank">FormNexus</a> got accepted at <a href="https://conf.researchr.org/home/issta-2024" target="_blank">ISSTA 2024</a>!
    </td>
  </tr>
</table>

---

<p style="margin-top: 30px">Below is a list of my current and inactive projects.</p>

### Current Projects
{% assign current = site.data.projects | where_exp: "project", "project.end == nil" %}
{% include projects.html data=current %}

### Inactive Projects
{% assign inactive = site.data.projects | where_exp: "project", "project.end != nil" %}
{% include projects.html data=inactive %}
