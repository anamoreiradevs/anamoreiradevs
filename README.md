<div id="header" align="center">
  <img src="https://media.giphy.com/media/EcqCKYnrHiAgwpGqme/giphy.gif" width="150"/>
</div>

<div id="header" align="center">
  <a href="https://www.linkedin.com/in/ana-lydia-moreira-6a79571a6/">
    <img src="https://img.shields.io/badge/LinkedIn-purple?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
  </a>
</div>
<div id="badges" align="center">
 <img src="https://komarev.com/ghpvc/?username=analydiamoreira&style=flat-square&color=yellow" alt=""/>
</div>

<h1>
</h1>


---

### :woman_technologist: About Me :

I am a programming student <img src="https://media.giphy.com/media/SYHz66JfYHbBtZXjHy/giphy.gif" width="30"> from Brazil.

- :telescope: I have been studying programming since 2021.

- :seedling: Exploring new ways.

- :zap: In my free time, i study English by myself.

- :mailbox:How to reach me: [![Linkedin Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/ana-lydia-moreira-6a79571a6/)  

###  :fire: My Stats :


[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com?user=anamoreiradevs&theme=tokyonight_duo)](https://git.io/streak-stats)
---
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=anamoreiradevs&layout=compact&theme=tokyonight_duo)](https://github.com/anamoreiradevs/github-readme-stats)



### :hammer_and_wrench: Languages and Tools :
<div>
  <img src="https://github.com/devicons/devicon/blob/master/icons/csharp/csharp-original.svg" width="40" height="40"/>&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" widht="40" height="40"/>&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" widht="40" height="40"/>&nbsp;
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" width="40" height="40"/>&nbsp;
                    
  
  - ![Snake animation](https://github.com/anamoreiradevs/anamoreiradevs/blob/output/github-contribution-grid-snake.svg)

---






name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: anamoreiradevs
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
