<h1 align="left">Hi There 👋! I am Rishi</h1>

<p align="left">
  I’m a software developer who enjoys building practical, user-focused applications
  and exploring how technology can solve real-world problems. My interests include
  full-stack web development, system design, and continuously improving my
  problem-solving skills through hands-on projects and collaborative work.
</p>

<img
  align="right"
  height="150"
  src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExcmpmbjN2azlzN2RxN2ltdzBjN2c0dG9kNGR6N3cybW1hZGo2NGlzZyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/bGgsc5mWoryfgKBx1u/giphy.gif"
  alt="Coding animation"
/>

<h2 align="left">About Me</h2>

<p align="left">
🚀 <b>Currently building:</b> Sanjeevani 2.0 — a healthcare management platform
with appointment booking, SOS alerts, and medical records.
<br><br>

🧩 <b>Projects:</b> Developed complete web applications such as Sanjeevani
and DappRush Studios, working across UI design, frontend development,
backend integration, and overall project structure.
<br><br>

🛠️ <b>Tech focus:</b> Full-stack web development, responsive UI,
API integration, and database-driven systems.
<br><br>

🏆 <b>Hackathons & Activities:</b> Participated in multiple hackathons
and technical events, gaining experience in teamwork and rapid development.
<br><br>

📚 <b>Learning:</b> Machine learning fundamentals, web technologies,
system design, and software engineering best practices.
<br><br>

🤝 <b>Communities:</b> Active contributor and promoted associate in
college technical clubs.
<br><br>

⚡ <b>Fun fact:</b> I enjoy building creative tech projects and refining
user experiences.
</p>

<p align="left">
  🌐 <b>Portfolio:</b>
  <a href="https://portfolio-beta-nine-eaus9jwxk6.vercel.app/">
    Visit my portfolio
  </a>
</p>

<h2 align="left">Skills & Tools</h2>

<p align="left">
  <b>Languages:</b>
  Java, Go, Python, C++, C, JavaScript, TypeScript, SQL
  <br>

  <b>Frameworks & Platforms:</b>
  React, Node.js, Express, Tailwind CSS, AWS (Basics), Git, GitHub
  <br>

  <b>Web & Databases:</b>
  REST APIs, MySQL, MongoDB, HTML, CSS
  <br>

  <b>Data Science / ML:</b>
  Python, NumPy, Pandas, Machine Learning Fundamentals
  <br>

  <b>Certifications:</b>
  NPTEL – Machine Learning | Web Development Certification |
  Programming in C / C++
</p>

name: GitHub Profile Stats

on:
  schedule:
    - cron: "0 0 * * *"

  workflow_dispatch:

  push:
    branches:
      - main

jobs:
  stats:
    runs-on: ubuntu-latest

    permissions:
      contents: write

    steps:
      - name: Generate GitHub Stats
        uses: readme-tools/github-readme-stats-action@v1
        with:
          card: stats
          options: username=${{ github.repository_owner }}&show_icons=true&hide_border=true&theme=dark
          path: profile/stats.svg
          token: ${{ secrets.GITHUB_TOKEN }}

      - name: Generate Top Languages
        uses: readme-tools/github-readme-stats-action@v1
        with:
          card: top-langs
          options: username=${{ github.repository_owner }}&layout=compact&langs_count=8&hide_border=true&theme=dark
          path: profile/top-langs.svg
          token: ${{ secrets.GITHUB_TOKEN }}

      - name: Commit generated cards
        run: |
          git config user.name "github-actions"
          git config user.email "github-actions@users.noreply.github.com"

          git add profile/*.svg

          git commit -m "Update GitHub profile stats" || exit 0

          git push

<br>

<h2 align="left">GitHub Contribution Snake</h2>

<div align="center">

  <picture>
    <source
      media="(prefers-color-scheme: dark)"
      srcset="https://raw.githubusercontent.com/Rishi122005/Rishi122005/output/github-snake-dark.svg"
    />

    <source
      media="(prefers-color-scheme: light)"
      srcset="https://raw.githubusercontent.com/Rishi122005/Rishi122005/output/github-snake.svg"
    />

    <img
      alt="GitHub contribution snake"
      src="https://raw.githubusercontent.com/Rishi122005/Rishi122005/output/github-snake.svg"
    />
  </picture>

</div>

<h2 align="left">Connect With Me</h2>

<p align="left">
  📧 <b>Email:</b>
  <a href="mailto:codrishiriengs@gmail.com">
    codrishiriengs@gmail.com
  </a>
  <br><br>

  💼 <b>LinkedIn:</b>
  <a href="https://www.linkedin.com/in/rishi122005/">
    linkedin.com/in/rishi122005
  </a>
  <br><br>

  🌐 <b>Portfolio:</b>
  <a href="https://portfolio-beta-nine-eaus9jwxk6.vercel.app/">
    portfolio
  </a>
</p>

<p align="center">
  Thanks for visiting! If you’re interested in collaborating on projects,
  discussing ideas, or building something meaningful together, feel free to reach out.
  <br><br>
  <b>Let's connect 🚀</b>
</p>
