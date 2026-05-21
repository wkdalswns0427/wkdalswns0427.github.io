---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
  - /resume/
---

{% include base_path %}

[Download as PDF](/assets/files/Curriculum_Vitae_Minjun.pdf){: .btn}

Education
======
* Ph.D., Civil Engineering (Robotics in Construction), Georgia Institute of Technology, 2025 -- present
* B.S., Mechanical Engineering, Yonsei University, 2019 -- 2025

Research Experience
======
See the [Research](/research/) page for full details.

* **2024.06 -- 2024.12** — Undergraduate Intern, Dynamic Robotic Systems Laboratory, Seoul National University.
* **2022.07 -- 2023.01** — Undergraduate Intern, Machine Learning and Control System Laboratory, Yonsei University.
* **2020.07 -- 2021.06** — Undergraduate Intern, Mechanobiology and Soft Materials Laboratory, Yonsei University.
* **2020.07 -- 2021.06** — Undergraduate Intern, BioMedical & Energy System Lab, Yonsei University.

Work Experience
======
See the [Work](/work/) page for full details.

* **2025.01 -- 2025.05** — Satellite Software Engineer, Hanwha Systems (Space & Defense).
* **2024.04 -- 2024.06** — Robotics Engineer (Intern), GoLe Robotics.
* **2022.10 -- 2024.03** — Junior Embedded Software Engineer, DRIMAES.
* **2022.02 -- 2022.10** — Junior Embedded Software Engineer, ToysMyth (SIOT Infotech).
* **2021.06 -- 2021.07** — AI Lab Member (Intern), Alsemy.

<h2>Skills</h2><hr />
<ul class="publication-list">
  <li><b>Programming Languages:</b> Python, C, C++, MATLAB, JavaScript.</li>
  <li><b>Frameworks / Tools:</b> ROS1 &amp; 2, Docker, IsaacGym, MuJoCo, PyTorch, FastAPI, SolidWorks.</li>
  <li><b>Hardware:</b> Jetson Xavier, Jetson Nano, RaspberryPi, Arduino, ESP32, STM32, Bolt10, ScoutMini, WeGoERP42.</li>
  <li><b>Languages:</b> Korean (Native), English (Fluent, TOEFL 108 / personal best 111).</li>
</ul>

<h2>Awards &amp; Honors</h2><hr />
<p>See the <a href="/achievements/">Achievements</a> page for the full list, including licenses.</p>
<ol reversed start="10" class="publication-list">
  <li><a href="https://www.digitalopenlab.or.kr/main/index.php">National ICT Smart Device Competition</a>, <b>Grand Prize (1st place)</b>, 2024, Ministry of Science and ICT.</li>
  <li><a href="http://m.irobotnews.com/news/articleView.html?idxno=30037">Autonomous Robot Racing Competition, 2nd Match 2022</a>, <b>Grand Prize (1st place)</b>, 2022, Korea Robot Society.</li>
  <li>IHEI Show Off Festa 2, <b>Best Choice Award</b>, 2021, IHEI Yonsei.</li>
  <li><a href="http://www.hanium.or.kr/">Hanium Competition</a>, <b>Selection</b>, 2021, Federation of Korea Information Industries.</li>
  <li><a href="https://www.all-con.co.kr/uni_contest/467239">MEDICAL HACK 2021</a>, <b>Excellence Prize</b>, 2021, Busan City.</li>
  <li>Yonsei IHEI Workstation, <b>Impact Solution Award</b>, 2021, IHEI Yonsei.</li>
  <li><a href="http://biosku.konkuk.ac.kr/medical/main/main.php">KU Medical Hackathon</a>, <b>Excellence Prize</b>, 2020, Konkuk Univ. Hospital.</li>
  <li><a href="https://cfd.edison.re.kr/web/challenge/10th_design">EDISON Computer Aided Design Competition</a>, <b>Top 8</b>, 2020, K-MOOC.</li>
  <li>IHEI Summer Workstation &mdash; ACUOUS, <b>Excellence Award</b>, 2020, IHEI Yonsei.</li>
  <li>YonseiXNexon Creative Platform, <b>Excellence Prize</b>, 2019, RC Committee.</li>
</ol>

{% if site.publication_category %}
{% for category in site.publication_category %}
{% assign category_posts = site.publications | where: 'category', category[0] | sort: 'date' %}
{% if category_posts.size > 0 %}
<h2>{{ category[1].title }}</h2><hr />
{% assign total = category_posts.size %}
{% assign display_order = category_posts | reverse %}
<ol reversed start="{{ total }}" class="publication-list">
{% for post in display_order %}<li>{{ post.citation }}</li>
{% endfor %}
</ol>
{% endif %}
{% endfor %}
{% else %}
{% assign sorted_posts = site.publications | sort: 'date' %}
{% assign total = sorted_posts.size %}
{% assign display_order = sorted_posts | reverse %}
<h2>Publications</h2><hr />
<ol reversed start="{{ total }}" class="publication-list">
{% for post in display_order %}<li>{{ post.citation }}</li>
{% endfor %}
</ol>
{% endif %}
