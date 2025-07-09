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

<div class="container">
  <div class="hero">
    <div class="info">
      <h1>Hi, I'm Carey Harrell</h1>
      <p>
        I'm a data analyst with a passion for interactive dashboards and AI-powered insights. I specialize in Power BI,
        Tableau, and Streamlit — turning data into intuitive visual stories.
      </p>
      <p>
        <a href="resume.pdf">📄 Resume</a> |
        <a href="mailto:carey.harrell@outlook.com">📧 Email</a> |
        <a href="https://www.linkedin.com/in/carey-harrell/">🔗 LinkedIn</a>
      </p>
    </div>
    <img src="profile.jpg" alt="Your Photo" />
  </div>

  <div class="buttons">
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

  <div id="tableau" class="section">
    <h2>NBA Award Predictions (Tableau)</h2>
    <p>Machine learning-driven predictions for NBA awards presented via Tableau dashboards.</p>
    <iframe
      title="Test"
      src="https://public.tableau.com/views/NBAAwardsPrediction/PlayerOverTime?:embed=y&:display_count=yes&:toolbar=yes"
      width="1000"
      height="4000"
      frameborder="0"
      allowFullScreen="true">
    </iframe>
  </div>

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
