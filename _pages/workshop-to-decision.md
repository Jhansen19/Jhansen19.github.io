---
permalink: /workshop-to-decision/
title: "Workshop-to-Decision: Demo"
layout: single
---

<style>
  .demo-video { width: 100%; border-radius: 8px; border: 1px solid rgba(255,255,255,0.3); background: #000; }
  .chapters { list-style: none; padding: 0; margin: 16px 0 32px; display: grid;
              grid-template-columns: repeat(auto-fill, minmax(220px, 1fr)); gap: 8px; }
  .chapters button { width: 100%; text-align: left; cursor: pointer; padding: 8px 12px;
                     background: transparent; color: inherit; border: 1px solid rgba(255,255,255,0.4);
                     border-radius: 8px; font: inherit; font-size: 0.85em; }
  .chapters button:hover, .chapters button:focus-visible { border-color: #fff; }
  .chapters .t { font-variant-numeric: tabular-nums; opacity: 0.75; margin-right: 8px; }
  .demo-links a { display: inline-block; margin: 0 12px 12px 0; padding: 8px 16px; text-decoration: none;
                  border: 1px solid currentColor; border-radius: 8px; }
</style>

An AI-assisted workflow that turns raw workshop notes into a one-page decision summary, gets a
manager's approval, and only then saves the decisions, tasks and risks to a shared tracker.
All company names, people and data in the demo are fictional.

<video class="demo-video" id="demo" controls preload="metadata"
       poster="{{ site.baseurl }}/assets/images/workshop-to-decision.jpg">
  <source src="{{ site.baseurl }}/assets/videos/workshop-to-decision-demo.mp4" type="video/mp4">
  Your browser can't play this video.
  <a href="{{ site.baseurl }}/assets/videos/workshop-to-decision-demo.mp4">Download it instead</a>.
</video>

**Chapters**: click to jump.

<ul class="chapters">
  <li><button type="button" data-t="0"><span class="t">0:00</span>The problem and the project</button></li>
  <li><button type="button" data-t="100"><span class="t">1:40</span>The meeting notes</button></li>
  <li><button type="button" data-t="120"><span class="t">2:00</span>Submitting the notes</button></li>
  <li><button type="button" data-t="160"><span class="t">2:40</span>How the workflow works</button></li>
  <li><button type="button" data-t="240"><span class="t">4:00</span>The draft summary</button></li>
  <li><button type="button" data-t="320"><span class="t">5:20</span>Approval and the tracker</button></li>
  <li><button type="button" data-t="460"><span class="t">7:40</span>Test results</button></li>
  <li><button type="button" data-t="530"><span class="t">8:50</span>How it's built</button></li>
  <li><button type="button" data-t="600"><span class="t">10:00</span>Trade-offs and what's next</button></li>
</ul>

<div class="demo-links">
  <a href="https://github.com/Jhansen19/workshop-to-decision-n8n" target="_blank">
    <i class="fab fa-github" aria-hidden="true" style="margin-right:8px;"></i>Code, results and README on GitHub
  </a>
  <a href="{{ site.baseurl }}/projects/">
    <i class="fas fa-arrow-left" aria-hidden="true" style="margin-right:8px;"></i>Back to projects
  </a>
</div>

<script>
  document.querySelectorAll('.chapters button').forEach(function (b) {
    b.addEventListener('click', function () {
      var v = document.getElementById('demo');
      v.currentTime = Number(b.dataset.t);
      v.play();
      v.scrollIntoView({ behavior: 'smooth', block: 'center' });
    });
  });
</script>
