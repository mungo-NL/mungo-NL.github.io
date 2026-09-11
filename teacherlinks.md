---
layout: page
title: Teacher Links
---

### Teacher Links

Curriculum guides, professional resources, lesson plan databases, and more. For educators and coordinators.

<div style="margin: 1.5rem 0; padding: 1rem; background: #f7f7f7; border-radius: 8px;">
  <strong>Jump to:</strong>
  <a href="#elementary">Elementary</a> ·
  <a href="#intermediate">Intermediate</a> ·
  <a href="#high-school">High School</a> ·
  <a href="#all-grades">All Grades</a> ·

</div>

<input type="text" id="page-search" placeholder="Search this page for keywords..." 
  style="width: 100%; max-width: 500px; padding: 10px 14px; font-size: 1rem; border: 1px solid #ccc; border-radius: 6px; margin: 1.5rem 0; display: block;">

<script>
document.getElementById('page-search').addEventListener('input', function() {
  var query = this.value.toLowerCase();
  var cards = document.querySelectorAll('.link-card');
  var groups = document.querySelectorAll('.grade-group');

  cards.forEach(function(card) {
    var text = card.textContent.toLowerCase();
    var match = text.includes(query);
    card.style.display = match ? '' : 'none';

    var divider = card.previousElementSibling;
    if (divider && divider.classList.contains('section-divider')) {
      divider.style.display = match ? '' : 'none';
    }
  });

  groups.forEach(function(group) {
    var visibleCard = group.querySelector('.link-card:not([style*="display: none"])');
    group.style.display = visibleCard ? '' : 'none';
  });
});
</script>

<style>
.section-divider {
  border: none;
  border-top: 2px solid #ccc;
  margin: 3rem 0 2rem 0;
}
.link-card {
  display: flex;
  gap: 20px;
  align-items: flex-start;
  margin: 2rem 0;
  padding: 1.5rem;
  border-radius: 8px;
  background: #f7f7f7;
}
.link-thumb { 
  width: 120px; 
  height: 120px; 
  object-fit: scale-down; 
  padding: 12px;
  box-sizing: border-box;
  border-radius: 6px; 
  background: #fff; 
  box-shadow: 0 2px 6px rgba(0,0,0,0.15); 
  flex-shrink: 0; 
}
.link-title {
  font-weight: bold;
  font-size: 1.1rem;
  margin-bottom: 0.5rem;
}
.link-desc {
  margin-bottom: 0.75rem;
}
.link-grade {
  display: inline-block;
  background: #800000;
  color: #fff;
  font-weight: bold;
  font-size: 0.85rem;
  padding: 4px 12px;
  border-radius: 20px;
}
</style>

<div class="grade-group">
  <h3 id="elementary">Elementary</h3>

  <hr class="section-divider">
  <div class="link-card">
    <img class="link-thumb" src="/assets/img/science_world_logo.png">
    <div>
      <div class="link-title"><a href="https://science-world.e-learningforkids.org/en/grade-4/map" target="_blank">Science World</a></div>
      <div class="link-desc">
        <p>Science World includes simple, interactive activities for elementary school students introducing rocks and Earth materials. It features classification of rocks, material properties, etc.</p>
        <p>The “worlds” are divided by grades, featuring lots more lessons than just geophysics, but you can “Search Lesson” for specifics:</p>
        <ul>
          <li>Grade 2: Rocks, forces, materials</li>
          <li>Grade 4: Sound, magnets, motion</li>
          <li>Grade 5: Electricity, circuits, forces</li>
          <li>Grade 6: Energy, tectonic plates, earthquakes</li>
        </ul>
      </div>
      <div class="link-grade">Grades K-6</div>
    </div>
  </div>
</div>

<div class="grade-group">
  <h3 id="intermediate">Intermediate</h3>

  <hr class="section-divider">
  <div class="link-card">
    <img class="link-thumb" src="/assets/img/virtual_quake_logo.png">
    <div>
      <div class="link-title"><a href="https://www.sciencecourseware.org/VirtualEarthquake/" target="_blank">Virtual Earthquake</a></div>
      <div class="link-desc">
        <p>Virtual Earthquake is an interactive Web-based activity designed to introduce you to the concepts of how an earthquake EPICENTER is located and how the RICHTER MAGNITUDE of an earthquake is determined.</p>
        <p>Students locate earthquake epicentres using real seismic data. Demonstrates seismology, a key tool used to study Earth’s interior. (<strong>Bonus</strong>: you get a certificate at the end).</p>
      </div>
      <div class="link-grade">Grades 7-9</div>
    </div>
  </div>
</div>

<div class="grade-group">
  <h3 id="high-school">High School</h3>

  <hr class="section-divider">
  <div class="link-card">
    <img class="link-thumb" src="/assets/img/careers_science_logo.png">
    <div>
      <div class="link-title"><a href="https://careers.earthsciencescanada.com/what-can-you-be/ " target="_blank">What Can You Be?</a></div>
      <div class="link-desc">
        <p>A short quiz that introduces careers in Earth science and geophysics.</p>
        <p>You can be any number of things as an Earth Scientist. From the Earth’s core to the cosmos there is a career for you to discover! Earth Scientists have a wide range of job titles, working in one or many of the <strong>W.H.E.R.E.</strong> career sectors that make up the Earth Sciences:</p>

<div class="grade-group">
  <h3 id="all-grades">All Grades</h3>

  <hr class="section-divider">
  <div class="link-card">
    <img class="link-thumb" src="/assets/img/earthlinks_logo.png">
    <div>
      <div class="link-title"><a href="https://www.cgenarchive.org/earthlinks.html" target="_blank">EarthLinks</a></div>
      <div class="link-desc">
        <p>Earth Links is a collection of online resources selected by the members of CGEN, which is a national network of Canadian educators and professionals interested in promoting awareness of the Earth Sciences.</p>
        <p>All of the EarthLinks were submitted and/or suggested by CGEN members. The selection process focused on Canadian content so many links are available in both English and French.</p>
      </div>
      <div class="link-grade">All Grades</div>
    </div>
  </div>
</div>

