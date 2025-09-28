name: Generate pacman animation

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"

  workflow_dispatch:

  push:
    branches:
    - main

jobs:
  generate:
    permissions:
      contents: write
    runs-on: ubuntu-latest
    timeout-minutes: 5

    steps:
      - name: generate pacman-contribution-graph.svg
        uses: abozanona/pacman-contribution-graph@main
        with:
          github_user_name: ${{ github.repository_owner }}


      - name: push pacman-contribution-graph.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Tenebroon/Tenebroon/output/pacman-contribution-graph-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Tenebroon/Tenebroon/output/pacman-contribution-graph.svg">
  <img alt="pacman contribution graph" src="https://raw.githubusercontent.com/Tenebroon/Tenebroon/output/pacman-contribution-graph.svg">
</picture>

###

<h1 align="center">Hi 👋🏼, I'm Tenebroon</h1>

###

<br clear="both">

<h4 align="center">-- A Code Newbie 👊🏼 --</h4>

###

<h2 align="center"></h2>

###

<img align="right" height="220" src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExaHhheHNsbHM5cWpmaG90Z29lOWMxcmQ3Nm56Z2l1cmZ0NGxjN21tYiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/bGgsc5mWoryfgKBx1u/giphy.gif"  />

###

<h4 align="left">📚 Recently learned</h4>

###

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" height="30" alt="html5 logo"  />
  <img width="10" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="30" alt="css logo"  />
</div>

###

<h4 align="left">📖 Currently learning</h4>

###

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="30" alt="javascript logo"  />
  <img width="10" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="30" alt="python logo"  />
  <img width="10" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" height="30" alt="linux logo"  />
</div>

###

<h2 align="left"></h2>

###

<h5 align="left">📫 Connect with me</h5>

###

<div align="left">
  <a href="https://t.me/Tenebroon" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Telegram&logo=telegram&label=&color=2CA5E0&logoColor=white&labelColor=&style=flat" height="20" alt="telegram logo"  />
  </a>
  <a href="https://chat.google.com/room/AAQANQPw8wE?cls=7" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Gmail&logo=gmail&label=&color=D14836&logoColor=white&labelColor=&style=flat" height="20" alt="gmail logo"  />
  </a>
</div>

###

<h2 align="left"></h2>

###
