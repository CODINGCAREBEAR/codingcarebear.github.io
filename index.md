---
layout: default
title: Home
---

<style>
.container {
  max-width: 1150px;
  margin: 0 auto;
  padding: 0 1em;
}

.hero {
  background-color: #cce5ff;
  padding: 1.2em 1.5em;
  margin-top: 1em;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  border-radius: 8px;
}
.hero .info {
  max-width: 60%;
}
.hero img {
  width: 160px;
  height: 160px;
  border-radius: 10px;
  border: 3px solid #0056b3;
}
.buttons {
  margin: 2em 0;
  text-align: center;
}
.buttons button {
  margin: 0.5em;
  padding: 0.5em 1.5em;
  border: 2px solid #0056b3;
  border-radius: 25px;
  background-color: white;
  color: #0056b3;
  font-weight: bold;
  cursor: pointer;
}
.buttons button.active,
.buttons button:hover {
  background-color: #0056b3;
  color: white;
}
.section {
  display: none;
  padding: 1em;
  background-color: white;
  border-radius: 8px;
  margin-bottom: 2em;
  box-shadow: 2px 2px 6px rgba(0, 0, 0, 0.05);
}
.section.active {
  display: block;
}
</style>
<!-- Modified section inside your existing HTML -->

<div class="container">
  <div class="hero">
    <div class="info">
      <h1>Hi, I'm Carey Harrell</h1>
      <p>
        <a href="resume.pdf">📄 Resume</a> |
        <a href="mailto:carey.harrell@outlook.com">📧 Email</a> |
        <a href="https://www.linkedin.com/in/carey-harrell/">🔗 LinkedIn</a>
      </p>
      <p>
        I'm a data analyst with a passion for interactive dashboards and AI-powered insights. I specialize in Power BI,
        Tableau, and Streamlit — turning data into intuitive visual stories.
      </p>
    </div>
    <img src="profile.jpg" alt="Your Photo" />
  </div>

  <div class="buttons" style="margin-bottom: 1em;">
    <button onclick="showSection('powerbi')" id="btn-powerbi" class="active">Power BI</button>
    <button onclick="showSection('tableau')" id="btn-tableau">Tableau</button>
    <button onclick="showSection('streamlit')" id="btn-streamlit">Streamlit</button>
  </div>

  <div id="powerbi" class="section active">
    <h2>NBA Player Comparison (Power BI)</h2>
    <p>Interactive analysis of NBA players using data from PostgreSQL hosted on AWS.</p>
    <iframe
      title="NBA_Analysis_Player_Stats_Final"
      style="width: 100%; height: 2000px;"
      src="https://app.powerbi.com/view?r=eyJrIjoiMzRlMjMxZjktMWRjZi00ZmQxLWJkYmQtMmY1ZGEzNzExM2NkIiwidCI6IjljZjNkNGIxLTBiZTYtNGI4NS1iOTVkLWY4NjRkMmUxN2Q2OCIsImMiOjF9"
      frameborder="0"
      allowFullScreen="true"
    ></iframe>
  </div>
</div>


<!-- Tableau Section -->
<div id="tableau" class="section" style="max-width: 1000px; margin: 1em auto;">
  <h2>NBA Tableau Dashboards</h2>

  <!-- Dashboard Selector Buttons -->
  <div style="text-align: center; margin-bottom: 1.5em;">
    <button onclick="showTableau('viz1')" class="tableau-btn active">2024 Award Predictions</button>
    <button onclick="showTableau('viz2')" class="tableau-btn">Historical Award Analysis</button>
    <button onclick="showTableau('viz4')" class="tableau-btn">League Trends Over Time</button>
    <button onclick="showTableau('viz3')" class="tableau-btn">Player Career and Stats Analysis</button>
  </div>

  <!-- Moved Tableau description to here -->
  <p id="tableau-description" style="text-align: center; max-width: 900px; margin: 0 auto 1em;">
    Interactive predictions for the 2024 NBA season awards, driven by advanced statistics and machine learning models.
  </p>

  <!-- Dashboard Containers -->
  <div id="viz1" class="tableau-viz" style="width:1000px; height:4027px;">
    <div class='tableauPlaceholder' id='viz1752075142061' style='width:1000px; height:4027px;'>
      <noscript><a href='#'><img alt='Player Over Time' src='https://public.tableau.com/static/images/NB/NBAAwardsPrediction/PlayerOverTime/1_rss.png' style='border: none' /></a></noscript>
      <object class='tableauViz' style='display: none;'>
        <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
        <param name='embed_code_version' value='3' />
        <param name='site_root' value='' />
        <param name='name' value='NBAAwardsPrediction/PlayerOverTime' />
        <param name='tabs' value='no' />
        <param name='toolbar' value='yes' />
        <param name='static_image' value='https://public.tableau.com/static/images/NB/NBAAwardsPrediction/PlayerOverTime/1.png' />
        <param name='animate_transition' value='yes' />
        <param name='display_static_image' value='yes' />
        <param name='display_spinner' value='yes' />
        <param name='display_overlay' value='yes' />
        <param name='display_count' value='yes' />
        <param name='language' value='en-US' />
      </object>
    </div>
  </div>

  <script>
  var divElement = document.getElementById('viz1752075142061');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width = '1000px';
  vizElement.style.height = '4027px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
  </script>


  <div id="viz2" class="tableau-viz" style="display:none; width:1000px; height:4027px;">
    <div class='tableauPlaceholder' id='viz1752074946639' style='width:1000px; height:4027px;'>
      <noscript><a href='#'><img alt='Player Over Time' src='https://public.tableau.com/static/images/NB/NBAAwardsAnalysis/PlayerOverTime/1_rss.png' style='border: none' /></a></noscript>
      <object class='tableauViz' style='display: none;'>
        <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
        <param name='embed_code_version' value='3' />
        <param name='site_root' value='' />
        <param name='name' value='NBAAwardsAnalysis/PlayerOverTime' />
        <param name='tabs' value='no' />
        <param name='toolbar' value='yes' />
        <param name='static_image' value='https://public.tableau.com/static/images/NB/NBAAwardsAnalysis/PlayerOverTime/1.png' />
        <param name='animate_transition' value='yes' />
        <param name='display_static_image' value='yes' />
        <param name='display_spinner' value='yes' />
        <param name='display_overlay' value='yes' />
        <param name='display_count' value='yes' />
        <param name='language' value='en-US' />
      </object>
    </div>
  </div>

  <script>
  var divElement = document.getElementById('viz1752074946639');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width = '1000px';
  vizElement.style.height = '4027px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
  </script>


  <div id="viz3" class="tableau-viz" style="display:none; width:1000px; height:4027px;">
    <div class='tableauPlaceholder' id='viz1752075073721' style='width:1000px; height:4027px;'>
      <noscript><a href='#'><img alt='Player Over Time' src='https://public.tableau.com/static/images/NB/NBAPlayerAnalysis_17104712376710/PlayerOverTime/1_rss.png' style='border: none' /></a></noscript>
      <object class='tableauViz' style='display: none;'>
        <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
        <param name='embed_code_version' value='3' />
        <param name='site_root' value='' />
        <param name='name' value='NBAPlayerAnalysis_17104712376710/PlayerOverTime' />
        <param name='tabs' value='no' />
        <param name='toolbar' value='yes' />
        <param name='static_image' value='https://public.tableau.com/static/images/NB/NBAPlayerAnalysis_17104712376710/PlayerOverTime/1.png' />
        <param name='animate_transition' value='yes' />
        <param name='display_static_image' value='yes' />
        <param name='display_spinner' value='yes' />
        <param name='display_overlay' value='yes' />
        <param name='display_count' value='yes' />
        <param name='language' value='en-US' />
      </object>
    </div>
  </div>

  <script>
  var divElement = document.getElementById('viz1752075073721');
  var vizElement = divElement.getElementsByTagName('object')[0];
  vizElement.style.width = '1000px';
  vizElement.style.height = '4027px';
  var scriptElement = document.createElement('script');
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
  vizElement.parentNode.insertBefore(scriptElement, vizElement);
  </script>


  <div id="viz4" class="tableau-viz" style="display:none; width:1000px; height:4027px;">
    <div class='tableauPlaceholder' id='viz1752075033715' style='width:1000px; height:4027px;'>
      <noscript><a href='#'><img alt='Player Over Time' src='https://public.tableau.com/static/images/NB/NBALeagueTrends/PlayerOverTime/1_rss.png' style='border: none' /></a></noscript>
      <object class='tableauViz' style='display: none;'>
        <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
        <param name='embed_code_version' value='3' />
        <param name='site_root' value='' />
        <param name='name' value='NBALeagueTrends/PlayerOverTime' />
        <param name='tabs' value='no' />
        <param name='toolbar' value='yes' />
        <param name='static_image' value='https://public.tableau.com/static/images/NB/NBALeagueTrends/PlayerOverTime/1.png' />
        <param name='animate_transition' value='yes' />
        <param name='display_static_image' value='yes' />
        <param name='display_spinner' value='yes' />
        <param name='display_overlay' value='yes' />
        <param name='display_count' value='yes' />
        <param name='language' value='en-US' />
      </object>
    </div>
  </div>
  </div>

  <script>
    var divElement = document.getElementById('viz1752075033715');
    var vizElement = divElement.getElementsByTagName('object')[0];
    vizElement.style.width = '1000px';
    vizElement.style.height = '4027px';
    var scriptElement = document.createElement('script');
    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
    vizElement.parentNode.insertBefore(scriptElement, vizElement);
  </script>

<!-- Script to toggle dashboards and descriptions -->
<script>
const descriptions = {
  viz1: "Interactive predictions for the 2024 NBA season awards, driven by advanced statistics and machine learning models.",
  viz2: "Explore historical trends in NBA award voting to understand past patterns and standout seasons.",
  viz3: "Analyze individual NBA players’ careers, performance metrics, and evolution over time.",
  viz4: "Dive into league-wide trends over the years including pace, scoring, and position dynamics."
};

function showTableau(id) {
  document.querySelectorAll('.tableau-viz').forEach(el => el.style.display = 'none');
  document.getElementById(id).style.display = 'block';
  document.getElementById('tableau-description').textContent = descriptions[id];

  document.querySelectorAll('.tableau-btn').forEach(btn => btn.classList.remove('active'));
  const index = id.replace("viz", "") - 1;
  document.querySelectorAll('.tableau-btn')[index].classList.add('active');
}
</script>

<!-- Optional CSS for buttons -->
<style>
.tableau-btn {
  margin: 0.5em;
  padding: 0.5em 1.2em;
  border: 2px solid #0056b3;
  background-color: white;
  color: #0056b3;
  border-radius: 20px;
  font-weight: bold;
  cursor: pointer;
}
.tableau-btn.active, .tableau-btn:hover {
  background-color: #0056b3;
  color: white;
}
</style>



<!-- Streamlit goes back inside -->
<div class="container">
  <div id="streamlit" class="section">
    <h2>NHANES Health Dashboard (Streamlit)</h2>
    <p>AI-enhanced health recommendations based on NHANES data via a Streamlit web app.</p>
    <p><a href="https://your-streamlit-app.streamlit.app" target="_blank">Open Streamlit App →</a></p>
  </div>
</div>

<script>
function showSection(id) {
  document.querySelectorAll('.section').forEach(sec => sec.classList.remove('active'));
  document.querySelectorAll('.buttons button').forEach(btn => btn.classList.remove('active'));
  document.getElementById(id).classList.add('active');
  document.getElementById('btn-' + id).classList.add('active');
}
</script>
