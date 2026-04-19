---
layout: page
permalink: /publications/
title: publications
description: 
nav: true
nav_order: 2

---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<!-- View Toggle Buttons -->
<div class="pub-view-toggle">
  <button id="btn-year"     class="pub-toggle-btn active" onclick="pubSwitchView('year')">By Year</button>
  <button id="btn-topic"    class="pub-toggle-btn"        onclick="pubSwitchView('topic')">By Topic</button>
  <button id="btn-selected" class="pub-toggle-btn"        onclick="pubSwitchView('selected')">Selected</button>
</div>

<!-- ── Year View ─────────────────────────────────── -->
<div id="pub-view-year" class="publications">
{% bibliography %}
</div>

<!-- ── Topic View ────────────────────────────────── -->
<div id="pub-view-topic" class="publications" style="display:none">

<!-- TOC: JavaScript가 빈 섹션 제외 후 동적으로 채움 -->
<div id="pub-topic-toc"></div>

<h2 id="topic-A" class="pub-topic-heading">[A] Disturbance Observer</h2>
<div class="topic-section">
{% bibliography --query @*[groups~=Disturbance Observer] --sort_by year --order descending %}
</div>

<h2 id="topic-B" class="pub-topic-heading">[B] Multi-agent System</h2>
<div class="topic-section">
{% bibliography --query @*[groups~=Multi-agent System] --sort_by year --order descending %}
</div>

<h2 id="topic-C" class="pub-topic-heading">[C] Nonlinear Observer</h2>
<div class="topic-section">
{% bibliography --query @*[groups~=Nonlinear Observer] --sort_by year --order descending %}
</div>

<h2 id="topic-D" class="pub-topic-heading">[D] Output Feedback Stabilization</h2>
<div class="topic-section">
{% bibliography --query @*[groups~=Output Feedback Stabilization] --sort_by year --order descending %}
</div>

<h2 id="topic-E" class="pub-topic-heading">[E] Stability Analysis</h2>
<div class="topic-section">
{% bibliography --query @*[groups~=Stability Analysis] --sort_by year --order descending %}
</div>

<h2 id="topic-F" class="pub-topic-heading">[F] Control Method</h2>
<div class="topic-section">
{% bibliography --query @*[groups~=Control Method] --sort_by year --order descending %}
</div>

<h2 id="topic-G" class="pub-topic-heading">[G] Security of Control System</h2>
<div class="topic-section">
{% bibliography --query @*[groups~=Security of Control System] --sort_by year --order descending %}
</div>

<h2 id="topic-H" class="pub-topic-heading">[H] Switched/Hybrid System</h2>
<div class="topic-section">
{% bibliography --query @*[groups~=Switched/Hybrid System] --sort_by year --order descending %}
</div>

<h2 id="topic-I" class="pub-topic-heading">[I] Parallel Feedforward Compensator</h2>
<div class="topic-section">
{% bibliography --query @*[groups~=Parallel Feedforward Compensator] --sort_by year --order descending %}
</div>

<h2 id="topic-J" class="pub-topic-heading">[J] Biological Dynamics and Control</h2>
<div class="topic-section">
{% bibliography --query @*[groups~=Biological Dynamics and Control] --sort_by year --order descending %}
</div>

<h2 id="topic-K" class="pub-topic-heading">[K] Data-Driven/Learning</h2>
<div class="topic-section">
{% bibliography --query @*[groups~=Data-Driven/Learning] --sort_by year --order descending %}
</div>

<h2 id="topic-L" class="pub-topic-heading">[L] Others</h2>
<div class="topic-section">
{% bibliography --query @*[groups~=Others] --sort_by year --order descending %}
</div>


</div><!-- /pub-view-topic -->

<!-- ── Selected View ──────────────────────────────── -->
<div id="pub-view-selected" class="publications" style="display:none" markdown="1">

{%- comment -%}
  ★★★ 추천 논문 목록을 여기서 편집하세요 ★★★

  papers.bib의 entry key(cite key)를 아래 {% cite ... %} 줄에 나열하면 됩니다.
  나열한 순서대로 표시됩니다.

  예시:
    {% cite Back2004Nonlinea %}
    {% cite Back2006Discussi %}
    {% cite Back2007Nonsmoot %}

  <span style="display:none">
  {% cite Back2004Nonlinea %}
  {% cite Back2006Discussi %}
  {% cite Back2007Nonsmoot %}
  </span>

  {% bibliography --cited_in_order %}
{%- endcomment -%}

# Tutorial style articles

## Disturbance observer

> "Disturbance Observers"  
> H. Shim  
> in *Encyclopedia of Systems and Control*, Springer, 2020  
> doi:[10.1007/978-1-4471-5102-9_100068-1](https://doi.org/10.1007/978-1-4471-5102-9_100068-1)  
> also available at arxiv:[2101.02859](http://arxiv.org/abs/2101.02859)

> "Yet another tutorial of disturbance observer: Robust stabilization and recovery of nominal performance"  
> H. Shim, G. Park, Y. Joo, J. Back, and  N.H. Jo  
> Special Issue on Disturbance Rejection: A Snapshot, A Necessity, and A Beginning  
> *Control Theory and Technology*, vol. 14, issue 3, pp. 237-249, Aug 2016  
> doi:[10.1007/s11768-016-6006-9](http://dx.doi.org/10.1007/s11768-016-6006-9)  
> also available at arxiv:[1601.02075](http://arxiv.org/abs/1601.02075)


## Multi-agent Systems

> "Design of heterogeneous multi-agent system for distributed computation"  
> Jin Gyu Lee, Hyungbo Shim  
> In: Jiang ZP., Prieur C., Astolfi A. (eds) *Trends in Nonlinear and Adaptive Control*. Lecture Notes in Control and Information Sciences, Springer, 2022  
> doi:[10.1007/978-3-030-74628-5_4](https://doi.org/10.1007/978-3-030-74628-5_4)  
> also available at arxiv:[2101.00161](https://arxiv.org/abs/2101.00161)

## Security of Control Systems

> "Zero-dynamics Attack, Variations, and Countermeasures"  
> Hyungbo Shim, Juhoon Back, Yongsoon Eun, Gyunghoon Park, Jihan Kim  
> In: Ishii H., Zhu Q. (eds) *Security and Resilience of Control Systems*. Lecture Notes in Control and Information Sciences, Springer, 2022  
> doi:[10.1007/978-3-030-83236-0_2](https://doi.org/10.1007/978-3-030-83236-0_2)  
> also available at arxiv:[2101.00556](https://arxiv.org/abs/2101.00556)

## Control based on homomorphic encryption

> "Comprehensive Introduction to Fully Homomorphic Encryption for Dynamic Feedback Controller via LWE-Based Cryptosystem"  
> Junsoo Kim, Hyungbo Shim and Kyoohyung Han  
> Privacy in Dynamical Systems, Springer, 2020  
> doi:[10.1007/978-981-15-0493-8](http://doi.org/10.1007/978-981-15-0493-8)  
> draft version available at arxiv:[1904.08025](https://arxiv.org/abs/1904.08025)

> "Comparison of encrypted control approaches and tutorial on dynamic systems using Learning With Errors-based homomorphic encryption"  
> Junsoo Kim, Dongwoo Kim, Yongsoo Song, Hyungbo Shim, Henrik Sandberg, and Karl H. Johansson  
> *Annual Reviews in Control*, Volume 54, pp. 200-218, 2022  
> doi:[10.1016/j.arcontrol.2022.10.002](https://doi.org/10.1016/j.arcontrol.2022.10.002)


# Selected publication

{% include selected_papers.liquid %}



</div><!-- /pub-view-selected -->

<script>
(function () {
  // ── 빈 토픽 섹션 숨기기 + TOC 생성 ─────────────────────────────────
  function initTopicView() {
    var visibleHeadings = [];

    document.querySelectorAll('.topic-section').forEach(function (sec) {
      var heading = sec.previousElementSibling;
      if (sec.querySelectorAll('li').length === 0) {
        // 논문 없는 섹션: h2와 함께 숨김
        if (heading && heading.classList.contains('pub-topic-heading')) {
          heading.style.display = 'none';
        }
        sec.style.display = 'none';
      } else {
        // 논문 있는 섹션: TOC 항목으로 수집
        if (heading && heading.id) {
          visibleHeadings.push({ id: heading.id, text: heading.textContent.trim() });
        }
      }
    });

    // TOC 렌더링
    var toc = document.getElementById('pub-topic-toc');
    if (!toc || visibleHeadings.length === 0) return;

    var html = '<p class="toc-title">Topics</p><ul>';
    visibleHeadings.forEach(function (h) {
      html += '<li><a href="#' + h.id + '">' + h.text + '</a></li>';
    });
    html += '</ul>';
    toc.innerHTML = html;

    // 클릭 시 navbar 높이 고려한 부드러운 스크롤
    toc.querySelectorAll('a').forEach(function (a) {
      a.addEventListener('click', function (e) {
        e.preventDefault();
        var target = document.getElementById(this.getAttribute('href').slice(1));
        if (!target) return;
        var navH = document.querySelector('.navbar') ? document.querySelector('.navbar').offsetHeight : 60;
        var top  = target.getBoundingClientRect().top + window.pageYOffset - navH - 12;
        window.scrollTo({ top: top, behavior: 'smooth' });
      });
    });
  }

  // ── 뷰 전환 (3-way) ──────────────────────────────────────────────────
  var VIEWS = ['year', 'topic', 'selected'];

  function pubSwitchView(view) {
    VIEWS.forEach(function (v) {
      var el  = document.getElementById('pub-view-' + v);
      var btn = document.getElementById('btn-' + v);
      if (el)  el.style.display = (v === view) ? 'block' : 'none';
      if (btn) btn.classList.toggle('active', v === view);
    });
    try { sessionStorage.setItem('pubView', view); } catch(e) {}
  }

  // expose to onclick attributes
  window.pubSwitchView = pubSwitchView;

  // 페이지 로드 후 실행
  document.addEventListener('DOMContentLoaded', function () {
    initTopicView();
    try {
      var saved = sessionStorage.getItem('pubView');
      if (saved && VIEWS.indexOf(saved) !== -1) pubSwitchView(saved);
    } catch(e) {}
  });
})();
</script>
                                                                                        