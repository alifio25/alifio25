![alifio25](image/github-header-banner.png)

# 💻 Tech Stack:
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) ![Riot Games](https://img.shields.io/badge/riotgames-D32936.svg?style=for-the-badge&logo=riotgames&logoColor=white)
# 📊 GitHub Stats:
![](https://github-readme-stats.vercel.app/api?username=alifio25&theme=dark&hide_border=false&include_all_commits=false&count_private=false)<br/>
![](https://nirzak-streak-stats.vercel.app/?user=alifio25&theme=dark&hide_border=false)<br/>
![](https://github-readme-stats.vercel.app/api/top-langs/?username=alifio25&theme=dark&hide_border=false&include_all_commits=false&count_private=false&layout=compact)

### 🔝 Top Contributed Repo
![](https://github-contributor-stats.vercel.app/api?username=alifio25&limit=5&theme=dark&combine_all_yearly_contributions=true)

---
[![](https://visitcount.itsvg.in/api?id=alifio25&icon=0&color=0)](https://visitcount.itsvg.in)

name: Generate snake animation

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
      - name: generate snake.svg
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: dist/snake.svg?palette=github-dark


      - name: push snake.svg to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

<!-- ✨ Typing Animation
<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&pause=1000&color=2196F3&center=true&vCenter=true&width=1000&lines=Hi+%F0%9F%91%8B%2C+I'm+Alifio%20Eren%20Atmaja;college%20student%20%E2%94%82%20Newbie%20Progammer;Welcome+to+my+GitHub+profile!" alt="Typing SVG" width="100%" />
</p>

<p align="left"> 
  <img src="https://komarev.com/ghpvc/?username=alifio25&label=Profile%20views&color=0e75b6&style=flat" alt="alifio25" /> 
</p>

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://github.com/alifio25" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/github.svg" alt="github" height="30" width="40" /></a>
<a href="https://www.instagram.com/alifio_25" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="instagram" height="30" width="40" /></a>
<a href="alifioeren" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/discord.svg" alt="discord" height="30" width="40" /></a>
<a href="www.linkedin.com/in/alifio-eren-atmaja-08a82b332" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="linkedin" height="30" width="40" /></a>
</p>

### Languages and Tools:
![VS Code](https://img.shields.io/badge/VS_Code-%23007ACC?style=for-the-badge&logo=vscode&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-%23007ACC?style=for-the-badge&logo=mysql&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-%23007ACC?style=for-the-badge&logo=javascript&logoColor=white) ![Python](https://img.shields.io/badge/Python-%23007ACC?style=for-the-badge&logo=python&logoColor=white) ![HTML5](https://img.shields.io/badge/HTML5-%23007ACC?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/CSS3-%23007ACC?style=for-the-badge&logo=css3&logoColor=white) 

<h3 align="left">📊 GitHub Stats:</h3>
<p>
  <img width="48%" src="https://github-readme-stats.vercel.app/api?username=alifio25&show_icons=true&locale=en" />
  <img width="48%" src="https://github-readme-stats.vercel.app/api/top-langs?username=alifio25&show_icons=true&locale=en&layout=compact" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=alifio25&" alt="alifio25" />
</p>
 -->
