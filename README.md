<!-- ============= HEADER (animated gradient wave) ============= -->
<a href="https://github.com/ShellPayant">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:1F6FEB,100:58A6FF&height=220&section=header&text=ShellPayant&fontSize=58&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Solutions%20developer%20·%20systematic%20trading%20·%20data%20tooling&descAlignY=58&descAlign=50&descSize=18" width="100%"/>
</a>

<!-- ============= TYPING SVG ============= -->
<div align="center">
  <a href="https://github.com/ShellPayant">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=20&pause=1000&color=58A6FF&center=true&vCenter=true&width=720&lines=Building+AlphaFactory+%E2%80%94+a+systematic+lab+for+US+equities;Quant+first.+Not+quant+only.;Risk+before+entry.+Regime+before+signal.;Coffee+in.+Backtests+out."/>
  </a>
</div>

<!-- ============= TOP BADGES ============= -->
<div align="center">
  <img src="https://komarev.com/ghpvc/?username=ShellPayant&label=Profile+views&color=0E1116&style=for-the-badge"/>
  <a href="https://github.com/ShellPayant?tab=followers"><img src="https://img.shields.io/github/followers/ShellPayant?style=for-the-badge&color=0E1116&label=Followers&logo=github"/></a>
  <img src="https://img.shields.io/badge/Status-Building_in_public-1F6FEB?style=for-the-badge"/>
</div>

<br/>

<!-- ============= ABOUT ============= -->
## &nbsp;About

I design and build systems where rigor matters more than speed of shipping. My core focus is **systematic trading infrastructure** — but finance is one domain, not the only one. Data tooling, decision-support systems, and reproducible research pipelines are all fair game.

```yaml
role:        Solutions developer · quant first, not quant only
focus:       Systematic trading · data tooling · reproducible research
location:    Anywhere with low latency · UTC+1
currently:   Building AlphaFactory — research → paper → execution lab
philosophy:  Process before result · Risk before entry · Regime before signal
not_a_fan:   Auto-traded black boxes · over-engineered abstractions · vibes
fueled_by:   Espresso · curiosity · the occasional drawdown
```

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%"/>

<!-- ============= AlphaFactory FLAGSHIP ============= -->
## &nbsp;What I'm building

### `AlphaFactory` &nbsp;·&nbsp; *systematic equity research lab*

A modular platform for hunting **recent** edges in US equities. Not a strategy — a **search system** that runs nightly, scores candidates, and surfaces decisions for human review.

```mermaid
flowchart LR
    A[Market data] --> B[Regime detector]
    B --> C[Factor library]
    C --> D[Walk-forward backtest]
    D --> E[Paper trading]
    E --> F{Human review gate}
    F -->|approved| G[Live capital]
    F -->|rejected| H[Research journal]

    style F fill:#1F6FEB,color:#fff,stroke:#58A6FF
    style G fill:#238636,color:#fff,stroke:#3FB950
    style H fill:#30363D,color:#fff,stroke:#8B949E
```

**Engine:** Nautilus Trader &nbsp;·&nbsp; **Data:** Polars + DuckDB + Parquet  
**Validation:** Walk-forward, purged k-fold, deflated Sharpe  
**Human gate:** Mandatory. AI assists, AI does not allocate capital.

> Components publish to GitHub as they reach the publishable bar. Pinned repos update in lockstep.

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%"/>

<!-- ============= MODE CUISINE (FR · toggleable) ============= -->
<div align="center">

<details>
<summary><b>&nbsp;🥄&nbsp; Bonus FR : ouvrir si vous voulez me voir <i>cook</i>&nbsp;</b></summary>

<br/>

<div align="left">

> *Bon. Vous voulez vraiment savoir comment je travaille ? Asseyez-vous.*

Moi je suis pas un quant comme les autres. Moi je suis un **cuisinier franco-allemand exilé en Irlande**, et le marché c'est ma cuisine. Je m'en fous des slides. Je m'en fous des LinkedIn posts. Donnez-moi un terminal, un dataset propre, et **laissez-moi cook**.

Le tick-data, c'est mes oignons : tu les caramélises lentement, tu déglaces au volume bid-ask, tu réduis. La **régime detection** ? Une *réduction de jus de momentum* — tu laisses mijoter trois ans de S&P jusqu'à ce que ça nappe la cuillère. Le **risk sizing** c'est le sel : trop t'es mort, pas assez c'est fade — *et personne, jamais, n'a aimé un Sharpe fade*.

**AlphaFactory** c'est pas un restaurant. C'est une **brigade**. Le sous-chef regime envoie les tickets, le commis factor scanner épluche l'univers, et moi en passe je goûte tout au paper trading avant que ça parte en salle. *Si c'est pas bon ça repart au feu. Si c'est trop salé on jette.* Pas de pitié. La cuisine c'est de la rigueur, pas du vibes.

Les gens me disent *« mais tu peux pas juste utiliser un LSTM comme tout le monde ? »* — **non**. Le LSTM c'est le micro-ondes du quant. Ça réchauffe mais ça cuit rien. Moi je fais à l'ancienne : **GARCH au beurre noisette**, **isolation forest en croûte de sel**, **random forest petit, comme un macaron** — pas un gâteau de mariage de 14 couches qui s'effondre au premier régime change.

Et la sauce, **toujours**, c'est la **walk-forward**. Réduite. Déglacée au purged k-fold. Montée au monte-carlo. Si elle tranche, ta stratégie tranche aussi. Pas de raccourci.

L'IA ? L'IA c'est mon plongeur. Elle nettoie, elle prépare, elle fait la mise en place. *Mais elle touche pas au capital.* Jamais. Le jour où ton plongeur sort un plat tout seul, ton restaurant ferme.

*Voilà. Maintenant fermez la porte de la cuisine et laissez-moi bosser.*

— ShellPayant, chef de partie · *Brigade AlphaFactory*

</div>

</details>

</div>

<br/>

<!-- ============= TECH STACK ============= -->
## &nbsp;Stack

<div align="center">

| Layer | Tools |
|:---|:---|
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white) |
| **Data** | ![Polars](https://img.shields.io/badge/Polars-CD792C?style=flat-square&logo=polars&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black) ![Parquet](https://img.shields.io/badge/Parquet-50ABF1?style=flat-square&logo=apacheparquet&logoColor=white) |
| **Quant** | ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white) ![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white) ![Nautilus](https://img.shields.io/badge/Nautilus_Trader-1E1E1E?style=flat-square&logoColor=white) |
| **Infra** | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) ![Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) |
| **Workflow** | ![VSCode](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white) ![Cursor](https://img.shields.io/badge/Cursor-000000?style=flat-square&logo=cursor&logoColor=white) ![Notion](https://img.shields.io/badge/Notion-000000?style=flat-square&logo=notion&logoColor=white) |

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
    <img alt="github contribution snake" src="https://raw.githubusercontent.com/ShellPayant/ShellPayant/output/github-snake.svg"/>
  </picture>
</div>

<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%"/>

<!-- ============= QUOTE ============= -->
<div align="center">
  <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=github-dark"/>
</div>

<!-- ============= CONTACT ============= -->
## &nbsp;Get in touch

<div align="center">

<a href="https://github.com/ShellPayant"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>
<a href="https://github.com/ShellPayant?tab=repositories"><img src="https://img.shields.io/badge/Repositories-0E1116?style=for-the-badge&logo=git&logoColor=white"/></a>
<img src="https://img.shields.io/badge/DMs-open_on_GitHub-1F6FEB?style=for-the-badge"/>

</div>

<br/>

<!-- ============= FOOTER ============= -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:58A6FF,50:1F6FEB,100:0D1117&height=120&section=footer"/>

<div align="center">
  <sub><i>Built quietly · Documented openly · Reviewed weekly</i></sub>
</div>
