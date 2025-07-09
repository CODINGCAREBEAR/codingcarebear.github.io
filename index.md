---
layout: default
title: Home
---

<style>
.hero {
  background-color: #cce5ff;
  padding: 2em;
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
  width: 140px;
  height: 140px;
  border-radius: 10px;
  border: 3px solid #0056b3;
}
.buttons {
  margin: 2em 0;
  text-align: center;
}
.buttons a {
  display: inline-block;
  margin: 0.5em;
  padding: 0.5em 1.5em;
  border: 2px solid #0056b3;
  border-radius: 25px;
  text-decoration: none;
  color: #0056b3;
  font-weight: bold;
}
.buttons a:hover {
  background-color: #0056b3;
  color: white;
}
.card-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 1.5em;
  justify-content: center;
}
.card {
  border: 1px solid #ddd;
  padding: 1em;
  width: 280px;
  border-radius: 8px;
  background: white;
  box-shadow: 2px 2px 6px rgba(0,0,0,0.05);
}
.card h3 {
  margin-top: 0.5em;
}
</style>

<div class="hero">
  <div class="info">
  <h1>Hi, I'm CodingCareBear</h1>
  <p>I'm a data analyst with a passion for interactive dashboards and AI-powered insights. I specialize in Power BI, Tableau, and Streamlit — turning data into intuitive visual stories.</p>
  <p>
    <a href="resume.pdf">📄 Resume</a> |
    <a href="mailto:carey.harrell@outlook.com">📧 Email</a> |
    <a href="https://www.linkedin.com/in/carey-harrell/">🔗 LinkedIn</a>
  </p>
  </div>
  <img src="profile.jpg" alt="Your Photo" />
</div>

<div class="buttons">
  <a href="#powerbi">Power BI</a>
  <a href="#tableau">Tableau</a>
  <a href="#streamlit">Streamlit</a>
</div>

<div class="card-grid">
  <div class="card" id="powerbi">
    <h3>NBA Player Comparison (Power BI)</h3>
    <p>Interactive analysis of NBA players using data from PostgreSQL hosted on AWS.</p>
    <p><a href="https://app.powerbi.com/view?r=eyJrIjoiMzRlMjMxZjktMWRjZi00ZmQxLWJkYmQtMmY1ZGEzNzExM2NkIiwidCI6IjljZjNkNGIxLTBiZTYtNGI4NS1iOTVkLWY4NjRkMmUxN2Q2OCIsImMiOjF9" target="_blank">View Dashboard →</a></p>
  </div>

  <div class="card" id="tableau">
    <h3>NBA Award Predictions (Tableau)</h3>
    <p>Machine learning-driven predictions for NBA awards presented via Tableau dashboards.</p>
    <p><a href="https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;NB&#47;NBAAwardsPrediction&#47;PlayerOverTime&#47;1_rss.png" target="_blank">View Dashboard →</a></p>
  </div>

  <div class="card" id="streamlit">
    <h3>NHANES Health Dashboard (Streamlit)</h3>
    <p>AI-enhanced health recommendations based on NHANES data via a Streamlit web app.</p>
    <p><a href="https://your-streamlit-app.streamlit.app" target="_blank">Open App →</a></p>
  </div>
</div>