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
  <a href="#all-grades">All Grades</a>
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

<!--<div class="grade-group">
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
</div>-->

<!--<div class="grade-group">
  <h3 id="intermediate">Intermediate</h3>

  <hr class="section-divider">
  <div class="link-card">
    <img class="link-thumb" src="/assets/img/virtual_quake_logo.png">
    <div>
      <div class="link-title"><a href="https://www.sciencecourseware.org/VirtualEarthquake/" target="_blank">Virtual Earthquake</a></div>
      <div class="link-desc">
        <p>Educational activities and resources, high-quality Earth science teaching materials with real datasets.</p>
      </div>
      <div class="link-grade">Grades 7-9</div>
    </div>
  </div>
</div>-->

<div class="grade-group">
  <h3 id="high-school">High School</h3>

  <hr class="section-divider">
  <div class="link-card">
    <img class="link-thumb" src="/assets/img/educational_materials_logo.png">
    <div>
      <div class="link-title"><a href="https://serc.carleton.edu/ANGLE/educational_materials/materials.html" target="_blank">Educational Materials Collection</a></div>
      <div class="link-desc">
        <p>Educational activities and resources, high-quality Earth science teaching materials with real datasets.</p>
      </div>
      <div class="link-grade">Grades 10-12</div>
    </div>
  </div>

  <hr class="section-divider">
  <div class="link-card">
    <img class="link-thumb" src="/assets/img/teach_earth_logo.png">
    <div>
      <div class="link-title"><a href="https://serc.carleton.edu/NAGTWorkshops/geophysics/activities.html" target="_blank">Hands-on Seismology: Constructing a School Seismometer</a></div>
      <div class="link-desc">
        <p>A guide from Science in School for building a simple seismometer using affordable materials. Covers P- and S-wave detection, electromagnetic induction, and seismic data analysis using free software. Includes an instruction booklet. Suited for grades 9-12. **May need a laptop on all night.</p>
      </div>
      <div class="link-grade">Grades 10-12</div>
    </div>
  </div>

  <hr class="section-divider">
  <div class="link-card">
    <img class="link-thumb" src="/assets/img/science_school_logo.png">
    <div>
      <div class="link-title"><a href="https://scienceinschool.org/article/2022/constructing-school-seismometer/" target="_blank">Classroom, Lab, and Field Exercises in Geophysics</a></div>
      <div class="link-desc">
        <p>This collection of teaching materials allows for the sharing of ideas and activities within the community of geophysics teachers. You can search by subject (computer modeling, exploration methods, etc.) and resource type (problem set, classroom activity, etc.)</p>
      </div>
      <div class="link-grade">Grades 10-12</div>
    </div>
  </div>

  <hr class="section-divider">
  <div class="link-card">
    <img class="link-thumb" src="/assets/img/gplates_logo.png">
    <div>
      <div class="link-title"><a href="https://www.gplates.org/" target="_blank">GPlates (Plate Tectonics Software)</a></div>
      <div class="link-desc">
        <p>GPlates is a free desktop program for plate tectonics. Manipulate reconstructions of geological and paleogeographic features through geological time. Students and teachers can manipulate paleogeographic features, visualize raster and vector data, and see how the Earth's plates have moved over deep time.</p>
        <p>Also has an iPhone app and web portal version if you don't want to install the software.</p>
      </div>
      <div class="link-grade">Grades 10-12</div>
    </div>
  </div>
</div>

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
      <div class="link-grade">Grades K-12</div>
    </div>
  </div>

  <hr class="section-divider">
  <div class="link-card">
    <img class="link-thumb" src="/assets/img/exploring_seat_logo.png">
    <div>
      <div class="link-title"><a href="https://exploringbytheseat.com/" target="_blank">Exploring by the Seat of Your Pants</a></div>
      <div class="link-desc">
        <p>Virtual field trips that connect students with real scientists. Good for real-world science applications and students can see how Earth scientists work in the field.</p>
        <p>Exploring by the Seat of Your Pants opens the frontlines of our changing planet to all students through the passion, immersive technology and visual storytelling of the scientists, explorers, conservationists, and adventurers who are smashing the boundaries of what we thought was possible.</p>
        <p>Their events are free for classrooms everywhere. Students are introduced to important and challenging issues, exciting places, strong role models, and new STEM career paths.</p>
      </div>
      <div class="link-grade">Grades K-12</div>
    </div>
  </div>

  <hr class="section-divider">
  <div class="link-card">
    <img class="link-thumb" src="/assets/img/agu_logo.png">
    <div>
      <div class="link-title"><a href="https://connect.agu.org/gpe/teaching-resources" target="_blank">Teaching Resources (AGU)</a></div>
      <div class="link-desc">
        <p>Lesson plans and activities from the American Geophysical Society (AGU) that connect physics to real geophysics applications. Separated by grade/level.</p>
      </div>
      <div class="link-grade">Grades K-12</div>
    </div>
  </div>

  <hr class="section-divider">
  <div class="link-card">
    <img class="link-thumb" src="/assets/img/ras_logo.png">
    <div>
      <div class="link-title"><a href="https://ras.ac.uk/education-and-careers/for-everyone/145-geophysics-links" target="_blank">Geophysics Links (RAS)</a></div>
      <div class="link-desc">
        <p>A curated list from the Royal Astronomical Society (RAS) of groups and societies around the world that work with geophysics, with teaching materials.</p>
      </div>
      <div class="link-grade">Grades K-12</div>
    </div>
  </div>
</div>
