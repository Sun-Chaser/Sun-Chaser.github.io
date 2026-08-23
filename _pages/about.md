---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi — I’m **Honghao Yang (杨洪浩)**, and I also go by **Jack**. I’m pursing a **M.S.** in **Computer Science** at **Washington University in St. Louis**, after finishing my **Bachelor's** study at **WashU** earlier in **May 2026**.

I’m interested in **parallel system** and **graph theory** and have previouse research experience on those fields:
- **Bottleneck Profiling**
- **Algorithm Designing**
- **Statistical Learning**

On this site, I share **projects**, **experiences**, and **classes** as I learn more about **parallel systems** and **performance engineering**. Also, I'd love to keep it as an archive of my past life and experience. Feel free to explore different sections!

<h3>TL;DR:</h3> Here is a current <a href="/files/AcademicCV.pdf">resume/CV</a> (Last Updated: 2026-02-11) of me. But trust me, this website will give you more than that :).

Education
===
<div class="education-entry">
  <h3>Washington University in St. Louis</h3>
  <p><strong>M.S. in Computer Science</strong></p>
  <p>Aug. 2026 – Dec. 2027 (Expected) · St. Louis, MO</p>
  <p>GPA: NA</p>
  <p>Honors: Half Scholarship</p>
</div>

<div class="education-entry">
  <h3>Washington University in St. Louis</h3>
  <p><strong>B.S. in Computer Science</strong> — Minor in Statistics</p>
  <p>Aug. 2023 – May. 2026 · St. Louis, MO</p>
  <p>GPA: 3.99/4.0 (Major GPA 4.0/4.0)</p>
  <p>Honors: Dean's List, Summa Cum Laude</p>
</div>

<div class="education-entry">
  <h3>Beijing Luhe International Academy</h3>
  <p><strong>Focused on Natural Science like Physics and Biology</strong></p>
  <p>Aug 2020 – June 2023 · Tongzhou, Beijing, China</p>
  <p>GPA: 96/100</p>
  <p>Honors: Three-Year's Full Scholarship (About $43K)</p>
</div>


Recent Activities
===
<ul class="recent-activities-list" data-expandable-list data-batch-size="5" data-item-selector=".recent-activity">
  <li class="recent-activity">2026 Aug. - Student Life Newspaper wensite new theme has been online. Check <a href="https://www.studlife.com/" target="_blank">here</a> for more information!</li>
  <li class="recent-activity">2026 Jun. - Start as Research Assistant in <a href="https://ramanlab.wustl.edu/" target="_blank">Raman Lab</a> for improving experiment APP functions</li>
  <li class="recent-activity">2026 Jun. - Start the Master Project mentored by Professor <a href="https://engineering.washu.edu/faculty/Kunal-Agrawal.html" target="_blank">Kunal Agrawal</a></li>
  <li class="recent-activity">2026 May. - Graduated from WashU Bachelor of Science in CS</li>
  <li class="recent-activity">2026 Feb. - Actively looking for programs and summer interns</li>
  <li class="recent-activity">2026 Jan. — Spring 2026 Semester Begins!</li>
  <li class="recent-activity">2025 Dec. — Fall 2025 Semester Ends! 6 course all A+ 🏆</li>
  <li class="recent-activity">2025 Aug. — Start the <a href="/experience/2025-08-01-independent-researcher-washu">independent study</a> mentored by Professor <a href="https://sds.washu.edu/people/robert-lunde" target="_blank">Robert Lunde</a> </li>
  <li class="recent-activity">2025 Aug. — Ending of the <a href="/experience/2025-01-01-undergraduate-research-assistant-sbs">REU Summer Research</a>!</li>
  <li class="recent-activity">2025 May. — CSE REU Summer Research started!</li>
</ul>
<div class="recent-activities__controls">
  <button class="recent-activities__more expandable__more" type="button">Expand</button>
  <button class="recent-activities__collapse expandable__collapse" type="button">Collapse</button>
</div>

<script>
  (function () {
    function initExpandableLists() {
    var lists = document.querySelectorAll("[data-expandable-list]");

    for (var j = 0; j < lists.length; j++) {
      (function (list) {
        var controls = list.nextElementSibling;
        while (controls && !controls.classList.contains("recent-activities__controls")) {
          controls = controls.nextElementSibling;
        }
        if (!controls) return;

        var moreButton = controls.querySelector(".expandable__more");
        var collapseButton = controls.querySelector(".expandable__collapse");
        if (!moreButton || !collapseButton) return;

        var itemSelector = list.getAttribute("data-item-selector") || "li";
        var items = list.querySelectorAll(itemSelector);
        var batchSize = parseInt(list.getAttribute("data-batch-size") || "5", 10);
        var visibleCount = 0;

        function updateVisibility() {
          for (var i = 0; i < items.length; i++) {
            items[i].style.display = i < visibleCount ? "" : "none";
          }
          moreButton.style.display = visibleCount >= items.length ? "none" : "";
          collapseButton.style.display = visibleCount > batchSize ? "" : "none";
          controls.style.display = items.length > batchSize ? "" : "none";
        }

        visibleCount = Math.min(batchSize, items.length);
        updateVisibility();

        moreButton.addEventListener("click", function () {
          visibleCount = Math.min(visibleCount + batchSize, items.length);
          updateVisibility();
        });

        collapseButton.addEventListener("click", function () {
          visibleCount = Math.min(batchSize, items.length);
          updateVisibility();
        });
      })(lists[j]);
    }
    }

    if (document.readyState === "loading") {
      document.addEventListener("DOMContentLoaded", initExpandableLists);
    } else {
      initExpandableLists();
    }
  })();
</script>


Programming Languages
===
<div class="skill-bars" data-expandable-list data-batch-size="5" data-item-selector=".skill-bar">
  <div class="skill-bar">
    <div class="skill-bar__header">
      <span class="skill-bar__name">C++</span>
      <span class="skill-bar__value">95%</span>
    </div>
    <div class="skill-bar__track">
      <div class="skill-bar__fill" style="width: 95%;"></div>
    </div>
    <p class="skill-bar__comment"> std::cout << "I used this a lot in research" << std::endl; </p>
  </div>

  <div class="skill-bar">
    <div class="skill-bar__header">
      <span class="skill-bar__name">C</span>
      <span class="skill-bar__value">90%</span>
    </div>
    <div class="skill-bar__track">
      <div class="skill-bar__fill" style="width: 90%;"></div>
    </div>
    <p class="skill-bar__comment"> printf("I am %.1f%% confidence with this in class", 90.001f); </p>
  </div>

  <div class="skill-bar">
    <div class="skill-bar__header">
      <span class="skill-bar__name">Git</span>
      <span class="skill-bar__value">90%</span>
    </div>
    <div class="skill-bar__track">
      <div class="skill-bar__fill" style="width: 90%;"></div>
    </div>
    <p class="skill-bar__comment">git commit -a -m "I solved a lot of git conflicts on cmd and IDE."</p>
  </div>

  <div class="skill-bar">
    <div class="skill-bar__header">
      <span class="skill-bar__name">Java</span>
      <span class="skill-bar__value">90%</span>
    </div>
    <div class="skill-bar__track">
      <div class="skill-bar__fill" style="width: 90%;"></div>
    </div>
    <p class="skill-bar__comment">System.out.println("My old friend from high school.");</p>
  </div>

  <div class="skill-bar">
    <div class="skill-bar__header">
      <span class="skill-bar__name">Python</span>
      <span class="skill-bar__value">90%</span>
    </div>
    <div class="skill-bar__track">
      <div class="skill-bar__fill" style="width: 90%;"></div>
    </div>
    <p class="skill-bar__comment">print("Using a lot in research and plotting")</p>
  </div>

  <div class="skill-bar">
    <div class="skill-bar__header">
      <span class="skill-bar__name">R</span>
      <span class="skill-bar__value">85%</span>
    </div>
    <div class="skill-bar__track">
      <div class="skill-bar__fill" style="width: 85%;"></div>
    </div>
    <p class="skill-bar__comment">cat("Used a lot in my stats course") </p>
  </div>

  <div class="skill-bar">
    <div class="skill-bar__header">
      <span class="skill-bar__name">CUDA</span>
      <span class="skill-bar__value">80%</span>
    </div>
    <div class="skill-bar__track">
      <div class="skill-bar__fill" style="width: 80%;"></div>
    </div>
    <p class="skill-bar__comment">printKernel<<<1, 1>>>("I'm learning right now.");</p>
  </div>

  <div class="skill-bar">
    <div class="skill-bar__header">
      <span class="skill-bar__name">Bash</span>
      <span class="skill-bar__value">80%</span>
    </div>
    <div class="skill-bar__track">
      <div class="skill-bar__fill" style="width: 80%;"></div>
    </div>
    <p class="skill-bar__comment">echo "Simple and easy tool"</p>
  </div>

  <div class="skill-bar">
    <div class="skill-bar__header">
      <span class="skill-bar__name">HTML, CSS, Javascript</span>
      <span class="skill-bar__value">70%</span>
    </div>
    <div class="skill-bar__track">
      <div class="skill-bar__fill" style="width: 70%;"></div>
    </div>
    <p class="skill-bar__comment">console.log("Konwing the majors, but need instruction");</p>
  </div>

  <div class="skill-bar">
    <div class="skill-bar__header">
      <span class="skill-bar__name">Ruby, SML, Racket</span>
      <span class="skill-bar__value">60%</span>
    </div>
    <div class="skill-bar__track">
      <div class="skill-bar__fill" style="width: 60%;"></div>
    </div>
    <p class="skill-bar__comment">puts "Family programming languages from 425 course: Love SML"</p>
  </div>
</div>

<div class="recent-activities__controls">
  <button class="recent-activities__more expandable__more" type="button">Expand</button>
  <button class="recent-activities__collapse expandable__collapse" type="button">Collapse</button>
</div>

Interesting Facts:
===
<ul class="interest-list" data-expandable-list data-batch-size="5" data-item-selector=".interest-list__item">
  <li class="interest-list__item">I only celebrate birthday on Lunar Calendar so it's hard to remember my birthday which differs every year.</li>
  <li class="interest-list__item">I couldn't cook before coming to U.S.A. But now I can cook really well.</li>
  <li class="interest-list__item">I like role-playing game and watched <em>Wichter III Concert</em> in 2025. Yayyyyyyy!!!</li>
  <li class="interest-list__item">I enjoy hiking and playing frisbee.🥏</li>
  <li class="interest-list__item">Sun-Chaser is my GitHub name while my Steam name is Star-Chaser. Why they are not consistent? Sun-Chaser is taken on Steam!!!😵</li>


</ul>
<div class="recent-activities__controls">
  <button class="recent-activities__more expandable__more" type="button">Expand</button>
  <button class="recent-activities__collapse expandable__collapse" type="button">Collapse</button>
</div>
