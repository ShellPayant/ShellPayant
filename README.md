<!-- ============= HEADER ============= -->
<a href="https://github.com/ShellPayant">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:238636,100:58A6FF&height=220&section=header&text=ShellPayant&fontSize=58&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=REI%20Milano%20%C2%B7%20property%20intelligence%20%C2%B7%20public%20real-estate%20data&descAlignY=58&descAlign=50&descSize=18" width="100%"/>
</a>

<!-- ============= TYPING SVG ============= -->
<div align="center">
  <a href="https://github.com/ShellPayant">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=20&pause=1000&color=58A6FF&center=true&vCenter=true&width=760&lines=Building+REI+Milano+for+Italian+property+intelligence;Turning+public+data+into+usable+market+estimates;OMI+zones+%C2%B7+Milano+civici+%C2%B7+PVP+auctions+%C2%B7+Wayback;Clear+estimates.+Honest+ranges.+Source+context."/>
  </a>
</div>

<!-- ============= TOP BADGES ============= -->
<div align="center">
  <img src="https://komarev.com/ghpvc/?username=ShellPayant&label=Profile+views&color=0E1116&style=for-the-badge"/>
  <a href="https://github.com/ShellPayant?tab=followers"><img src="https://img.shields.io/github/followers/ShellPayant?style=for-the-badge&color=0E1116&label=Followers&logo=github"/></a>
  <img src="https://img.shields.io/badge/Status-Building_REI_Milano-238636?style=for-the-badge"/>
</div>

<br/>

<!-- ============= ABOUT ============= -->
## &nbsp;About

I build data products where messy public records need to become something useful. My current focus is **REI Milano**: a Milan property-intelligence project that combines official real-estate data, civic address data, auction records, and market evidence into practical property estimates.

```yaml
role:        Data product builder · real-estate systems · applied research
focus:       REI Milano · Italian property data · public-source valuation tooling
location:    Europe-facing work · Milan market focus
currently:   Building a Milan estimator with OMI, civici, PVP auctions, and asking history
philosophy:  Source context before confidence · ranges before false precision
not_a_fan:   Black-box valuations · stale market assumptions · undocumented datasets
fueled_by:   Espresso · maps · clean pipelines · stubborn source validation
```

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%"/>

<!-- ============= REI MILANO FLAGSHIP ============= -->
## &nbsp;What I'm building

### `REI Milano` &nbsp;·&nbsp; *property intelligence for Milan*

<div align="center">

<img src="assets/rei-banner.png" alt="REI — Real Estate Intelligence" width="100%"/>

<p>
<img alt="Coverage" src="https://img.shields.io/badge/coverage-~8%2C000%20comuni-2F6BD6?style=flat-square&labelColor=1F3A6B"/>
<img alt="Pilot" src="https://img.shields.io/badge/pilot-Milano-3E7BD4?style=flat-square&labelColor=1F3A6B"/>
<img alt="Median held-out error" src="https://img.shields.io/badge/median%20%7Cerr%7C-24.0%25-4A7BD4?style=flat-square&labelColor=1F3A6B"/>
<img alt="Data" src="https://img.shields.io/badge/data-100%25%20public-6FA0E0?style=flat-square&labelColor=1F3A6B"/>
<img alt="Stack" src="https://img.shields.io/badge/stack-FastAPI%20%2B%20SQLite-9CC0E8?style=flat-square&labelColor=1F3A6B"/>
<img alt="Live market" src="https://img.shields.io/badge/live-rates%20%C2%B7%20equities%20%C2%B7%20short--let%20%C2%B7%20news-2F6BD6?style=flat-square&labelColor=1F3A6B"/>
</p>

</div>

REI Milano estimates apartment values in Milan from public and official data. The goal is not to pretend the Italian market has perfect transparency. The goal is to make the available signals usable: OMI micro-zones, Milan civic addresses, PVP auction records, asking-price history, and a clear uncertainty range.

```mermaid
flowchart LR
    A[Milano civici] --> D[Address resolver]
    B[OMI zones] --> E[Market anchor]
    C[PVP auctions] --> F[Property evidence]
    G[Asking history] --> F
    D --> H[REI estimate]
    E --> H
    F --> H
    H --> I[Value range]
    H --> J[Source breakdown]

    style H fill:#1F6FEB,color:#fff,stroke:#58A6FF
    style I fill:#238636,color:#fff,stroke:#3FB950
    style J fill:#30363D,color:#fff,stroke:#8B949E
```

**Current pilot:** Milan  
**Core sources:** Agenzia Entrate OMI, Comune di Milano civici, PVP auctions, Wayback captures  
**Live market layer:** an operator terminal aggregating ECB rates, Italian RE-sector equities, short-let (Airbnb) pressure, and real-estate news — context only, it never moves the estimate  
**Output:** property estimate, 80% range, and explainable source context  
**Demo modes:** FastAPI backend and static browser demo

> The public repo is [`rei-data-engine`](https://github.com/ShellPayant/rei-data-engine): the pipeline, API, validation work, and demo behind REI Milano.

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%"/>

<!-- ============= REI DATA ============= -->
## &nbsp;Milano data spine

<div align="center">

| Layer | What it contributes |
|:---|:---|
| **OMI zones** | Registered-transaction EUR/m² ranges by micro-zone |
| **Milano civici** | Address resolution, coordinates, and neighborhood context |
| **PVP auctions** | Real auction outcomes and perizia-derived property evidence |
| **Asking history** | Open-market listing signals over time |
| **Static demo bundle** | Browser-side REI Milano estimate flow for easy sharing |
| **Money & markets** | ECB rates (Euribor · BTP-10Y · €STR · HICP) + Italian RE-sector equities — affordability & sentiment |
| **Short-let** | Inside Airbnb → per-zone density, entire-home share, implied STR yield |
| **Live feed** | Italian RE/economy news rail + an engine event-tape (new lots, price cuts, macro prints) |

</div>

The estimate is designed to show uncertainty directly. Italian public data has gaps, so REI Milano presents a range and the evidence behind it instead of a single overconfident number.

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%"/>

<!-- ============= TECH STACK ============= -->
## &nbsp;Stack

<div align="center">

| Layer | Tools |
|:---|:---|
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white) |
| **Data** | ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white) ![PostGIS](https://img.shields.io/badge/PostGIS-336791?style=flat-square&logo=postgresql&logoColor=white) |
| **Backend** | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=black) |
| **Geo / web** | ![OpenStreetMap](https://img.shields.io/badge/OpenStreetMap-7EBC6F?style=flat-square&logo=openstreetmap&logoColor=white) ![Leaflet](https://img.shields.io/badge/Leaflet-199900?style=flat-square&logo=leaflet&logoColor=white) ![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-222222?style=flat-square&logo=githubpages&logoColor=white) |
| **Workflow** | ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white) |

</div>

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%"/>

<!-- ============= FEATURED WORK ============= -->
## &nbsp;Featured work

<div align="center">

| Project | Focus |
|:---|:---|
| [`rei-data-engine`](https://github.com/ShellPayant/rei-data-engine) | Milan property estimate pipeline, API, and static demo |
| `docs/` static demo | Browser-side REI Milano estimate flow for GitHub Pages / Netlify |
| PVP + OMI validation work | Auction-label checks and public-source estimate calibration |
| `REI Terminal` (Mercato) | Live Milano market console — rates, RE equities, short-let, news + event feed |

</div>

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%"/>

<!-- ============= GITHUB STATS ============= -->
## &nbsp;By the numbers

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=ShellPayant&show_icons=true&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=58A6FF&icon_color=58A6FF&text_color=C9D1D9&include_all_commits=true"/>
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ShellPayant&layout=compact&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=58A6FF&text_color=C9D1D9&langs_count=8"/>

<br/>

<img width="92%" src="https://github-readme-activity-graph.vercel.app/graph?username=ShellPayant&bg_color=0D1117&color=58A6FF&line=58A6FF&point=FFFFFF&area=true&hide_border=true&custom_title=Contribution%20Activity"/>

<br/>

<img src="https://streak-stats.demolab.com?user=ShellPayant&theme=github-dark-blue&hide_border=true&background=0D1117&ring=58A6FF&fire=58A6FF&currStreakLabel=58A6FF"/>

</div>

<br/>

<!-- ============= SNAKE ANIMATION ============= -->
<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ShellPayant/ShellPayant/output/github-snake-dark.svg"/>
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ShellPayant/ShellPayant/output/github-snake.svg"/>
    <img alt="github contribution graph" src="https://raw.githubusercontent.com/ShellPayant/ShellPayant/output/github-snake.svg"/>
  </picture>
</div>

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%"/>

<!-- ============= CONTACT ============= -->
## &nbsp;Get in touch

<div align="center">

<a href="https://github.com/ShellPayant"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
<a href="https://github.com/ShellPayant?tab=repositories"><img src="https://img.shields.io/badge/Repositories-0E1116?style=for-the-badge&logo=git&logoColor=white"/></a>
<img src="https://img.shields.io/badge/DMs-open_on_GitHub-1F6FEB?style=for-the-badge"/>

</div>

<br/>

<!-- ============= FOOTER ============= -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:58A6FF,50:238636,100:0D1117&height=120&section=footer"/>

<div align="center">
  <sub><i>Built quietly · sourced carefully · revised often</i></sub>
</div>
