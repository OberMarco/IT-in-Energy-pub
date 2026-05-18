---
marp: true # marp 7_Praesentation/7_presentation.md --html --allow-local-files -o docs/index.html
theme: default
paginate: true
math: mathjax
style: |
  section {
    font-family: 'Segoe UI', Arial, sans-serif;
    font-size: 26px;
    padding-top: 70px;
  }
  section.lead {
    padding-top: 0;
  }
  h1 {
    color: #1565C0;
    border-bottom: 3px solid #1565C0;
    padding-bottom: 10px;
  }
  h2 {
    color: #2196F3;
  }
  code {
    background-color: #F5F5F5;
    border-radius: 4px;
    padding: 2px 6px;
  }
  table {
    font-size: 22px;
  }
  .highlight {
    background: linear-gradient(135deg, #E3F2FD, #BBDEFB);
    border-radius: 10px;
    padding: 15px;
    margin: 10px 0;
  }
  .warning {
    background: #FFF3E0;
    border-left: 5px solid #FF9800;
    padding: 10px 15px;
    margin: 10px 0;
  }
  .success {
    background: #E8F5E9;
    border-left: 5px solid #4CAF50;
    padding: 10px 15px;
    margin: 10px 0;
  }
  .columns {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 30px;
  }
  .quote {
    border-left: 4px solid #1565C0;
    padding: 10px 20px;
    margin: 15px 0;
    font-style: italic;
    background: #F5F5F5;
    border-radius: 0 8px 8px 0;
  }
  .source {
    position: absolute;
    bottom: 18px;
    left: 40px;
    right: 60px;
    font-size: 0.38em;
    color: #aaa;
    white-space: normal;
    line-height: 1.4;
  }
  .source a {
    color: #aaa;
    text-decoration: none;
    border-bottom: 1px dotted #ccc;
  }
  .plotly-frame {
    width: 100%;
    height: 380px;
    border: none;
    border-radius: 8px;
  }
  /* ── Kapitel-Header ── */
  header {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    height: 52px;
    background: #f8f9fb;
    border-bottom: 2px solid #1565C0;
    display: grid;
    grid-template-columns: repeat(8, 1fr);
    align-items: center;
    padding: 0 10px;
    z-index: 1000;
    box-sizing: border-box;
  }
  header .ch {
    text-align: center;
    font-size: 12px;
    color: #bbb;
    font-weight: 500;
    padding: 4px 2px;
    border-radius: 4px;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    cursor: pointer;
    transition: all 0.2s;
  }
  header .ch:hover {
    background: #e3f2fd;
    color: #1565C0;
  }
  header .ch.active {
    background: #1565C0;
    color: white;
    font-weight: 700;
  }
  header a {
    text-decoration: none;
    color: inherit;
    display: block;
    width: 100%;
    height: 100%;
  }
---

<!-- _class: lead -->
<!-- _paginate: false -->

# IT in der Energiewirtschaft

## Übungskurs – Sommersemester 2026

<br>

⚡ Praxisorientierte Programmierung für die Energiebranche

---
<!-- _header: '<div class="ch active"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡ 5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->

# Über mich

<div class="columns">
<div>

<!-- TODO: Bild einfügen -->
<!-- ![w:300](foto.jpg) -->

**[Marco Obermeier](https://www.linkedin.com/in/marco-obermeier-566057247/)**
Wissenschaftlicher Mitarbeiter – [Smart Battery](https://www.hswt.de/forschung/projekt/2563-smartbattery) [1]

**Ausbildung**
- Elektroniker für Automatisierungstechnik
- Staatlich geprüfter Elektrotechniker
- B. Sc. Technische Informatik, OTH Regensburg
- M. Sc. Data Engineering in Energietechnik
  – Masterarbeit bei [N-ERGIE](https://www.n-ergie.de) [2]
  – Forschungsassistent am [Energiecampus Feuchtwangen](https://www.campus-feuchtwangen.de/de/2023/09/01/9596/) [3]

</div>
<div>

**Beruflich**
- Programmierer im Sondermaschinenbau
- Werkstudent in Forschungs- & Entwicklungsteams
- Wiss. Mitarbeiter bei [Veronika Grimm](https://www.utn.de/person/veronika-grimm/), UTN Nürnberg [4]
- Wiss. Mitarbeiter bei [Sepp Hochreiter](https://www.jku.at/en/institute-for-machine-learning/about-us/team/), JKU Linz [5]

**Kontakt**
- 📧 Zoom oder [marco.obermeier@hswt.de](mailto:marco.obermeier@hswt.de)
- 🏢 Raum F9.356

</div>
</div>

<span class="source">
[1] <a href="https://www.hswt.de/forschung/projekt/2563-smartbattery">HSWT – Smart Battery Projekt</a> &nbsp;
[2] <a href="https://www.n-ergie.de">N-ERGIE AG</a> &nbsp;
[3] <a href="https://www.energiecampus-feuchtwangen.de">Energiecampus Feuchtwangen</a> &nbsp;
[4] <a href="https://www.utn.de/person/veronika-grimm/">UTN – Prof. Grimm</a> &nbsp;
[5] <a href="https://www.jku.at/en/institute-for-machine-learning/about-us/team/">JKU – Prof. Hochreiter</a>
</span>

---
<!-- _header: '<div class="ch active"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡ 5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->

# Das Ziel: Was ihr am Ende könnt

**Batterie-Optimierung am Day-Ahead-Markt**

<iframe
  class="plotly-frame"
  src="battery_optimization_results.html">
</iframe>

Marktpreise einlesen → Optimierungsmodell bauen → Fahrplan berechnen → Ergebnis visualisieren

---
<!-- _header: '<div class="ch active"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->

# Kursaufbau

| # | Datum | Thema | Inhalt |
|:-:|:-----:|-------|--------|
| 0 | 23.03. | **Python-Grundlagen** | Variablen, Funktionen, Klasse `Kraftwerk` |
| 1 | 30.03. | **Git** | Versionskontrolle & Zusammenarbeit |
| 2 | 13.04. | **KI-Programmierung** | Prompting, Copilot, KI-Agenten |
| 3 | 20.04. | **Zeitreihen** | CSV, pandas, Stromkosten berechnen |
| 4 | 27.04. | **Plotting** | Matplotlib, Plotly, Dashboards |
| 5 | 04.05. | **Optimierung** | Linopy → PyPSA → Batterie-Fahrplan |
| 6 | 18.05. | **Regression** | PV-Prognose, Heizlast-Vorhersage |
| F | 25.05.-29.06. | **Projekt-Feedback** | Sprechstunde & Zwischenstand |
| Z | 06.07. | **Abschlusspräsentation** | Projektvorstellung |

<div class="highlight">

📐 Die Übungen enthalten jeweils ein Jupyternotebook mit Beispielen und Übungen

</div>

---
<!-- _header: '<div class="ch active"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡ 5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->

# Prüfungsleistung

<div class="columns">
<div>

### Abschlussprojekt → 30% der Note

- 4er Gruppen
- Abgabe der Jupyter Notebooks in Github
- Vorstellung des Projekts und des Notebooks
    - Codesicht (Wie?)
    - Entwicklungssicht (Womit?)
    - Energiewirtschaftliche Sicht (Was?)
- Abschlusspräsentation: **[06.07./ 09.07.]**

</div>
<div>

### Klausur

- Enthält **Fragen zu Übungen und Projekt**
- Code lesen & verstehen
- Ergebnisse interpretieren
- Keine Programmierung am PC
- Fragen zu Git

</div>
</div>

<div class="warning">

⚠️ Die Übung zählt **30%** der Gesamtnote. Zusätzlich kommen Übungsinhalte in der Klausur dran!

</div>

---
<!-- _header: '<div class="ch active"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡ 5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->

<style scoped>
table { font-size: 18px; }
td, th { padding: 4px 8px; }
</style>

# Projektthemen

| # | Thema | Beschreibung | Kategorie |
|:-:|-------|--------------|-----------|
| 1 | **GreenGrid Compass API** [1] | EU-Stromdaten abrufen & visualisieren | 🌐 API & Zeitreihen & Visualisierung |
| 2 | **Europäische Analyse** [2] | Balkendiagramme für jährlichen europäischen Lastvergleich | 🌐 API & Zeitreihen & Visualisierung |
| 3 | **Open-Meteo Wetter-API** [3] | PV-Erzeugung mit Wetterdaten, Korrelationsanalyse | 🌐 API & Zeitreihen & Visualisierung |
| 4 | **Sankey-Diagramm Deutschland** [4][5][6] | Energieflüsse visualisieren: Primärenergie → Endenergie | 📊 Visualisierung |
| 5 | **7-Tages-Boxplot-Dashboard** | Lastprofil-Verteilungen, Wochentag-Vergleich | 📊 Zeitreihen & Visualisierung |
| 6 | **Batteriespeicher-Optimierung** | Day-Ahead-Markt mit PyPSA, Erlösmaximierung | ⚡ Optimierung |
| 7 | **Wärmepumpen-Optimierung** | COP-Modellierung + Optimierung, Stromkosten minimieren | ⚡ Optimierung |
| 8 | **PV-Ertragsprognose** | Regression mit Wetterdaten, Entscheidungsbaum vs. Linear | 🤖 Prognose & ML |
| 9 | **Netzanalyse** | Erstellung eines Netzanalyse Beispiels mit pandapower | 🔌 Netzanalyse |
| 10 | **Eigenes Thema** | Selbstgewählte Fragestellung mit energiewirtschaftlichem Bezug (nach Absprache) | 🎯 Freie Wahl |

<span class="source">
[1] <a href="https://www.greengrid-compass.eu/">GreenGrid Compass API</a> &nbsp;
[2] <a href="https://transparency.entsoe.eu">ENTSO-E Transparency Platform</a> &nbsp;
[3] <a href="https://open-meteo.com">Open-Meteo Weather API</a> &nbsp;
[4] <a href="https://www.data-to-viz.com/graph/sankey.html">Sankey Diagrams – data-to-viz.com</a> &nbsp;
[5] <a href="https://www.bdew.de/media/documents/2_Energieflussbild_Deutschland_2023_TWh_vereinfacht.svg">Sankey Diagram DE</a> &nbsp;
[6] <a href="https://www.energy-charts.info/charts/energy/chart.htm?l=de&c=DE&legendItems=0wk&interval=year&year=2025">Energy Charts DE 2025</a>
</span>

---
<!-- _header: '<div class="ch active"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡ 5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->

# Setup

```bash
git clone https://github.com/OberMarco/IT-in-Energy-pub.git
cd it-energiewirtschaft-kurs
conda env create -f environment.yml

code
--> Kernel "environment_it_energy" auswählen
```

<div class="success">

✅ Bitte **vor der ersten Übung** installieren und `00_Test_Installation.ipynb` ausführen!

</div>

<span class="source"><a href="https://github.com/OberMarco/IT-in-Energy-pub">https://github.com/OberMarco/IT-in-Energy-pub</a></span>

---

<!-- _class: lead -->

# Übung 0 – Python-Grundlagen
🐍

---
<!-- _header: '<div class="ch"><a href="#2">📋 Orga</a></div><div class="ch active"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡ 5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->

# Python: Die meistverwendete Programmiersprache

<div class="columns">
<div>

**TIOBE Index März 2026 – Top 5:** [1]

| # | Sprache | Anteil |
|:-:|---------|:------:|
| 1 | **Python** 🏆 | ~23% |
| 2 | C | ~11% |
| 3 | Java | ~9% |
| 4 | C++ | ~9% |
| 5 | C# | ~7% |

<div class="highlight">

Python ist seit 2021 die **#1** – getrieben durch Data Science, KI und Automatisierung.

</div>

</div>
<div>

**In der Energiewirtschaft:**
- Stadtwerk-Skripte für Analyse & Automatisierung
- Führende Open-Source-Bibliotheken wie [PyPSA](https://pypsa.org) [2], [pandapower](https://www.pandapower.org) [3] und [oemof](https://oemof.org) [4] bauen auf Python auf
- Marktdaten-Analyse & Zeitreihenverarbeitung
- Optimierung & Prognose

→ Notebook in `0_Wiederholung_Python`
</div>
</div>

<span class="source">
[1] <a href="https://www.tiobe.com/tiobe-index/">TIOBE Index</a>, März 2026 &nbsp;
[2] <a href="https://pypsa.org">pypsa.org</a> &nbsp;
[3] <a href="https://www.pandapower.org">pandapower.org</a> &nbsp;
[4] <a href="https://oemof.org">oemof.org</a>
</span>

---

<!-- _class: lead -->

# Übung 1 – Einführung in Git
📦


---
<!-- _header: '<div class="ch"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch active"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡ 5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->


# Git: Standard für Versionskontrolle & globale Kollaboration


<div class="columns">
<div>


<!-- ![w:280](linus_torvalds.jpg) -->
<!-- TODO: Bild einfügen -->


**Linus Torvalds** (*1969)


- Erfinder von [Linux](https://www.kernel.org) [1] (1991)
- Erfinder von [Git](https://git-scm.com) [2][3] (2005)
- Git entstand in 2 Wochen aus Frust über bestehende Tools


<div class="quote">


"I'm an egotistical bastard, and I name all my projects after myself. First Linux, now Git."


*("git" = brit. Slang für Idiot)* [4]


</div>

→ Notebook `1_Intro_Git` (Praxis im Terminal)

</div>
<div>


**Warum Git?**
- Industriestandard – überall genutzt
- Zusammenarbeit im Team
- Nachvollziehbarkeit jeder Änderung


**Bekannte Git-Repos:**
- [Linux Kernel](https://github.com/torvalds/linux) [1]
- [Python](https://github.com/python/cpython) [5]
- [Firefox (Mozilla)](https://github.com/mozilla/gecko-dev) [6]
- [Wikipedia (MediaWiki)](https://github.com/wikimedia/mediawiki) [7]
- [Android (AOSP)](https://android.googlesource.com/platform/superproject) [8]
- [PyPSA](https://github.com/PyPSA/pypsa) [9]


</div>
</div>


<span class="source">
[1] <a href="https://www.kernel.org">kernel.org</a> &nbsp;
[2] <a href="https://git-scm.com">git-scm.com</a> &nbsp;
[3] <a href="https://git-scm.com/book/de/v2">Chacon & Straub – Pro Git Book</a>, 2014 &nbsp;
[4] <a href="https://archive.kernel.org/oldwiki/git.wiki.kernel.org/index.php/GitFaq.html#Why_the_.27Git.27_name.3F">Why the 'Git' name?</a> &nbsp;
[5] <a href="https://github.com/python/cpython">github.com/python/cpython</a> &nbsp;
[6] <a href="https://github.com/mozilla/gecko-dev">github.com/mozilla/gecko-dev</a> &nbsp;
[7] <a href="https://github.com/wikimedia/mediawiki">github.com/wikimedia/mediawiki</a> &nbsp;
[8] <a href="https://android.googlesource.com/platform/superproject">android.googlesource.com</a> &nbsp;
[9] <a href="https://github.com/PyPSA/pypsa">github.com/PyPSA/pypsa</a>
</span>


---

<!-- _class: lead -->

# Übung 2 – KI-Programmierung
🤖

---
<!-- _header: '<div class="ch"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch active"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡ 5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->

# Andrej Karpathy & die Zukunft des Programmierens

<div class="columns">
<div>

<!-- ![w:280](andrej_karpathy.jpg) -->
<!-- TODO: Bild einfügen -->

**Andrej Karpathy** (*1986)

- Ex-Director of AI bei Tesla
- Gründungsmitglied von [OpenAI](https://openai.com) [1]
- Stanford PhD, [YouTuber](https://www.youtube.com/@AndrejKarpathy) [2]

<div class="quote">

"The hottest new programming language is English." [3]

</div>

<div class="quote">

"There's a new kind of coding I call 'vibe coding'..." [4]

</div>

</div>
<div>

**Die Stufen der KI-Programmierung:**

| Stufe | Beispiel |
|:-----:|----------|
| 1 | Copilot vervollständigt Zeilen |
| **2** | **ChatGPT schreibt Funktionen** |
| 3 | KI-Agenten bauen ganze Projekte |

⚠️ Ihr müsst den Code trotzdem **verstehen**!

→ Notebook in `2_KI_unterstuetzte_Programmierung`

</div>
</div>

<span class="source">
[1] <a href="https://openai.com">openai.com</a> &nbsp;
[2] <a href="https://www.youtube.com/@AndrejKarpathy">youtube.com/@AndrejKarpathy</a> &nbsp;
[3] <a href="https://x.com/karpathy/status/1617979122625712128">Karpathy, X/Twitter</a>, 2023 &nbsp;
[4] <a href="https://x.com/karpathy/status/1886192184808149383">Karpathy, X/Twitter</a>, 2025
</span>

---
<!-- _class: lead -->

# Übung 3 – Zeitreihen
📈

---

<!-- _header: '<div class="ch"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch active"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡ 5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->
<style scoped>
table { font-size: 17px; }
td, th { padding: 3px 6px; }
.ts-row { display: flex; gap: 14px; align-items: flex-start; margin-top: 6px; }
.ts-col-table { flex: 0 0 60%; min-width: 0; }
.ts-col-side  { flex: 0 0 40%; min-width: 0; }
.ts-svg-wrap {
  background: #f9f8f5;
  border: 1px solid #dcd9d5;
  border-radius: 6px;
  padding: 6px 8px 4px 8px;
}
.ts-svg-wrap svg { width: 100%; height: auto; display: block; }
.ts-cap { font-size: 10px; color: #6b7280; text-align: center; margin-top: 3px; line-height: 1.25; }
.callout-warning {
  background: #fffbeb;
  border: 1px solid #f59e0b;
  border-left: 3px solid #f59e0b;
  border-radius: 5px;
  padding: 6px 8px;
  margin-top: 8px;
  font-size: 11px;
  line-height: 1.35;
}
.callout-warning strong { color: #92400e; display: block; margin-bottom: 2px; font-size: 11px; }
.callout-warning ul { margin: 2px 0 2px 14px; padding: 0; }
.callout-warning ul li { margin-bottom: 1px; }
.callout-warning code { background: #fef3c7; padding: 0 3px; border-radius: 2px; font-size: 0.9em; }
.callout-warning .cw-source { margin-top: 3px; font-size: 10px; color: #78716c; }
.callout-warning .cw-source a { color: #92400e; }
</style>
# Energiewirtschaft = System gekoppelter Zeitreihen
Aus Sicht der IT ist die Energiewirtschaft eine **riesige Zeitreihen-Datenbank**:

<div class="ts-row">
<div class="ts-col-table">

| Zeitreihe | Quelle | Granularität |
|-----------|--------|:-------------------:|
| Netzfrequenz | [Netzfrequenzmessung.de](https://netzfrequenzmessung.de/) [1] | ms – sekündlich |
| Haushaltslast | [Quaschning, HTW Berlin](https://solar.htw-berlin.de/wp-content/uploads/HTW-Repraesentative-elektrische-Lastprofile-fuer-Wohngebaeude.pdf) [2] | sekündlich - 15 min |
| PV-Erzeugung | [Energy-Charts](https://www.energy-charts.info) [3] | 15 min |
| Strompreis DA & ID | [EPEX Spot](https://www.epexspot.com) [4] | 15 min / stündlich |
| Solare Einstrahlung | [PVGIS](https://re.jrc.ec.europa.eu/pvg_tools/) [5] / [renewables.ninja](https://www.renewables.ninja) [6] | stündlich |
| Temperatur & Wetter | [Open-Meteo](https://open-meteo.com) [7] | stündlich |
| CO₂-Zertifikate | [EEX](https://www.eex.com) [8] | täglich |
| Füllstand Gasspeicher | [GIE/AGSI](https://agsi.gie.eu) [9] | täglich |
| Inst. Leistung DE | [Energy-Charts](https://www.energy-charts.info) [3] / [ENTSO-E](https://transparency.entsoe.eu) [10] | monatl.-jährlich |
| Inst. Leistung global | [IEA](https://www.iea.org/data-and-statistics) [11] | jährlich |

</div>
<div class="ts-col-side">

<div class="ts-svg-wrap">
<svg viewBox="0 0 320 140" xmlns="http://www.w3.org/2000/svg" role="img" aria-labelledby="ts-title ts-desc">
  <title id="ts-title">Exemplarische Zeitreihe</title>
  <desc id="ts-desc">10 diskrete Messpunkte als Zeitreihe.</desc>
  <line x1="36" y1="10" x2="36" y2="108" stroke="#9ca3af" stroke-width="1"/>
  <line x1="36" y1="108" x2="308" y2="108" stroke="#9ca3af" stroke-width="1"/>
  <line x1="36" y1="35"  x2="308" y2="35"  stroke="#e5e7eb" stroke-width="0.7" stroke-dasharray="3,3"/>
  <line x1="36" y1="60"  x2="308" y2="60"  stroke="#e5e7eb" stroke-width="0.7" stroke-dasharray="3,3"/>
  <line x1="36" y1="85"  x2="308" y2="85"  stroke="#e5e7eb" stroke-width="0.7" stroke-dasharray="3,3"/>
  <text x="31" y="112" text-anchor="end" font-size="8" fill="#9ca3af">0</text>
  <text x="31" y="88"  text-anchor="end" font-size="8" fill="#9ca3af">.25</text>
  <text x="31" y="63"  text-anchor="end" font-size="8" fill="#9ca3af">.50</text>
  <text x="31" y="38"  text-anchor="end" font-size="8" fill="#9ca3af">.75</text>
  <text x="31" y="14"  text-anchor="end" font-size="8" fill="#9ca3af">1.0</text>
  <text x="8" y="62" text-anchor="middle" font-size="8" fill="#6b7280" transform="rotate(-90,8,62)">x(t)</text>
  <text x="172" y="130" text-anchor="middle" font-size="8" fill="#6b7280">Zeitpunkt t</text>
  <polyline points="54,64 80,47 106,30 132,54 158,20 184,71 210,37 236,49 262,25 288,59"
            fill="none" stroke="#01696f" stroke-width="1.5" stroke-linejoin="round" opacity="0.5"/>
  <line x1="54"  y1="64"  x2="54"  y2="108" stroke="#01696f" stroke-width="0.7" stroke-dasharray="2,2" opacity="0.4"/>
  <line x1="80"  y1="47"  x2="80"  y2="108" stroke="#01696f" stroke-width="0.7" stroke-dasharray="2,2" opacity="0.4"/>
  <line x1="106" y1="30"  x2="106" y2="108" stroke="#01696f" stroke-width="0.7" stroke-dasharray="2,2" opacity="0.4"/>
  <line x1="132" y1="54"  x2="132" y2="108" stroke="#01696f" stroke-width="0.7" stroke-dasharray="2,2" opacity="0.4"/>
  <line x1="158" y1="20"  x2="158" y2="108" stroke="#01696f" stroke-width="0.7" stroke-dasharray="2,2" opacity="0.4"/>
  <line x1="184" y1="71"  x2="184" y2="108" stroke="#01696f" stroke-width="0.7" stroke-dasharray="2,2" opacity="0.4"/>
  <line x1="210" y1="37"  x2="210" y2="108" stroke="#01696f" stroke-width="0.7" stroke-dasharray="2,2" opacity="0.4"/>
  <line x1="236" y1="49"  x2="236" y2="108" stroke="#01696f" stroke-width="0.7" stroke-dasharray="2,2" opacity="0.4"/>
  <line x1="262" y1="25"  x2="262" y2="108" stroke="#01696f" stroke-width="0.7" stroke-dasharray="2,2" opacity="0.4"/>
  <line x1="288" y1="59"  x2="288" y2="108" stroke="#01696f" stroke-width="0.7" stroke-dasharray="2,2" opacity="0.4"/>
  <circle cx="54"  cy="64"  r="3"   fill="#9ca3af" stroke="#fff" stroke-width="1"/>
  <circle cx="80"  cy="47"  r="3"   fill="#9ca3af" stroke="#fff" stroke-width="1"/>
  <circle cx="106" cy="30"  r="3"   fill="#9ca3af" stroke="#fff" stroke-width="1"/>
  <circle cx="132" cy="54"  r="3"   fill="#9ca3af" stroke="#fff" stroke-width="1"/>
  <circle cx="158" cy="20"  r="4.5" fill="#01696f" stroke="#fff" stroke-width="1.5"/>
  <circle cx="184" cy="71"  r="3"   fill="#9ca3af" stroke="#fff" stroke-width="1"/>
  <circle cx="210" cy="37"  r="3"   fill="#9ca3af" stroke="#fff" stroke-width="1"/>
  <circle cx="236" cy="49"  r="3"   fill="#9ca3af" stroke="#fff" stroke-width="1"/>
  <circle cx="262" cy="25"  r="3"   fill="#9ca3af" stroke="#fff" stroke-width="1"/>
  <circle cx="288" cy="59"  r="3"   fill="#9ca3af" stroke="#fff" stroke-width="1"/>
  <line x1="158" y1="108" x2="158" y2="113" stroke="#01696f" stroke-width="1.5"/>
  <text x="158" y="122" text-anchor="middle" font-size="8" fill="#01696f" font-weight="600">t₄</text>
  <line x1="158" y1="15" x2="158" y2="5"  stroke="#01696f" stroke-width="1" stroke-dasharray="2,2"/>
  <text x="163" y="13" text-anchor="start" font-size="8" fill="#01696f" font-weight="600">x(t₄)=0.90</text>
</svg>
</div>
<div class="ts-cap">Jeder <strong>t</strong> → genau ein <strong>x(t)</strong></div>

<div class="callout-warning">
<strong>⚠️ Zeitformate & Zeitzonen</strong>
<ul>
<li><strong>UTC</strong>: intern. Referenz, kein DST [12]</li>
<li><strong>CET</strong>=UTC+1, <strong>CEST</strong>=UTC+2 [13]</li>
<li>ISO 8601: <code>2024-01-15T14:00:00Z</code></li>
<li>DST-Tage: 23 / 25 h beachten</li>
</ul>
<div class="cw-source">
[12] <a href="https://www.ptb.de/cms/ptb/fachabteilungen/abt4/fb-44/ag-441/darstellung-der-gesetzlichen-zeit/koordinierte-weltzeitskala-utc.html">PTB UTC</a> &nbsp;
[13] <a href="https://www.ptb.de/cms/ptb/fachabteilungen/abt4/fb-44/ag-441/darstellung-der-gesetzlichen-zeit/zeitzonen.html">PTB Zeitzonen</a>
</div>
</div>

</div>
</div>

→ Notebook in `3_Zeitreihen`

<span class="source">
[1] <a href="https://netzfrequenzmessung.de/">netzfrequenzmessung.de</a> &nbsp;
[2] <a href="https://solar.htw-berlin.de/wp-content/uploads/HTW-Repraesentative-elektrische-Lastprofile-fuer-Wohngebaeude.pdf">Lastprofile Quaschning, HTW Berlin</a> &nbsp;
[3] <a href="https://www.energy-charts.info">energy-charts.info</a> – Fraunhofer ISE &nbsp;
[4] <a href="https://www.epexspot.com">epexspot.com</a> &nbsp;
[5] <a href="https://re.jrc.ec.europa.eu/pvg_tools/">PVGIS</a> – EU JRC &nbsp;
[6] <a href="https://www.renewables.ninja">renewables.ninja</a> &nbsp;
[7] <a href="https://open-meteo.com">open-meteo.com</a> &nbsp;
[8] <a href="https://www.eex.com">eex.com</a> &nbsp;
[9] <a href="https://agsi.gie.eu">agsi.gie.eu</a> – GIE &nbsp;
[10] <a href="https://transparency.entsoe.eu">transparency.entsoe.eu</a> &nbsp;
[11] <a href="https://www.iea.org/data-and-statistics">iea.org</a> – IEA, 2025 &nbsp;
[12] <a href="https://www.ptb.de/cms/ptb/fachabteilungen/abt4/fb-44/ag-441/darstellung-der-gesetzlichen-zeit/koordinierte-weltzeitskala-utc.html">PTB – UTC</a> &nbsp;
[13] <a href="https://www.ptb.de/cms/ptb/fachabteilungen/abt4/fb-44/ag-441/darstellung-der-gesetzlichen-zeit/zeitzonen.html">PTB – Zeitzonen</a>
</span>

---

<!-- _class: lead -->

# Übung 4 – Plotting
📊

---
<!-- _header: '<div class="ch"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch active"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡ 5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->

# Visualisierung in der Energiewirtschaft

<div class="columns">
<div>

**Plots sind überall:**
- Lastprofile & Preisverläufe
- Monatsverbräuche (Balken)
- Jahresdauerlinien
- Heatmaps (365 × 24)

**Gute Visualisierung = gute Entscheidung** –
von der Betriebsführung bis zur Netzplanung.

<div class="quote">

"Above all else, show the data."
– Edward Tufte [5]

</div>

</div>
<div>

**Inspiration & Tools:**
- [Python Graph Gallery](https://python-graph-gallery.com) [1] – 400+ Beispiele mit Code
- [Plotly Python](https://plotly.com/python/) [2] – Interaktive Charts
- [data-to-viz.com](https://www.data-to-viz.com) [3] – Welcher Chart für welche Daten?
- [Information is Beautiful Awards](https://www.informationisbeautifulawards.com) [4] – Jährlicher Wettbewerb

→ Notebook in `4_Plots_in_Python`
</div>
</div>

<span class="source">
[1] <a href="https://python-graph-gallery.com">python-graph-gallery.com</a> &nbsp;
[2] <a href="https://plotly.com/python/">plotly.com/python</a> &nbsp;
[3] <a href="https://www.data-to-viz.com">data-to-viz.com</a> &nbsp;
[4] <a href="https://www.informationisbeautifulawards.com">informationisbeautifulawards.com</a> &nbsp;
[5] <a href="https://medium.com/plotly/above-all-else-show-the-data-1b8bbf05c2ae">Five Laws of Data-Ink</a> &nbsp;
[6] <a href="https://www.edwardtufte.com/book/the-visual-display-of-quantitative-information/">Tufte – The Visual Display of Quantitative Information</a>, 1983
</span>

---
<!-- _header: '<div class="ch"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch active"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡ 5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->

# Plotly – Interaktive Diagramme

<!--
  Plotly HTML-Export einbinden:
  1. In Python erzeugen:
       import plotly.graph_objects as go
       fig = go.Figure(...)
       fig.write_html("assets/chart_strompreise.html",
                      include_plotlyjs="cdn",
                      full_html=False)
  2. Dann hier einbetten:
-->

<iframe
  class="plotly-frame"
  src="https://ai-energy-consumption.plotly.app/">
</iframe>

<span class="source">
[1] <a href="https://plotly.com/python/">Plotly Technologies Inc.</a> – Collaborative data science, Montréal, QC, 2015 &nbsp;
[2] <a href="https://ai-energy-consumption.plotly.app/">ai-energy-consumption.plotly.app</a>, abgerufen 2026
</span>

---

<!-- _class: lead -->

# Übung 5 – Optimierung
⚡🔋

---
<!-- _header: '<div class="ch"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch"><a href="#16">📊 4 Plotting</a></div><div class="ch active"><a href="#19">⚡ 5 Opt.</a></div><div class="ch"><a href="#21">📉 6 Reg.</a></div>' -->

<style scoped>
table { font-size: 16px; }
td, th { padding: 2px 6px; }
</style>

# Frameworks für Energiesystem-Optimierung

In der Energiewirtschaft gibt es zahlreiche Open-Source-Frameworks:

| Framework | Fokus | Entwickler |
|-----------|-------|------------|
| **[PyPSA](https://pypsa.org)** [1] | Strom- & Sektorenkopplung | TU Berlin / KIT |
| **[oemof.solph](https://oemof-solph.readthedocs.io)** [2] | Flexibles Energiesystem-Modell | Uni Bremen / DLR / RLI / Uni Flensburg |
| **[Linopy](https://linopy.readthedocs.io)** [3] | Generischer LP/MILP-Wrapper | TU Berlin |
| **[Pyomo](http://www.pyomo.org)** [4] | Allgemeines Optimierungsframework | Sandia National Labs / IDAES |
| **[pandapower](https://www.pandapower.org)** [5] | Lastfluss & Netzanalyse | Uni Kassel / Fraunhofer IEE |

<div class="highlight">

Wir nutzen **[Linopy](https://linopy.readthedocs.io)** [3] (einfaches Einstiegsbeispiel) und **[PyPSA](https://pypsa.org)** [1] (Batterie-Optimierung) – beide basieren auf Python und nutzen den [HiGHS-Solver](https://highs.dev) [6].

</div>

→ Notebook in `5_Optimierung`

<span class="source">
[1] <a href="https://doi.org/10.5334/jors.188">T. Brown et al.</a>, "PyPSA," <em>J. Open Res. Softw.</em>, 2018 &nbsp;
[2] <a href="https://doi.org/10.1016/j.simpa.2020.100028">U. Krien et al.</a>, "oemof.solph," <em>Software Impacts</em>, vol. 6, 2020 &nbsp;
[3] <a href="https://doi.org/10.21105/joss.04628">F. Hofmann et al.</a>, "Linopy," <em>J. Open Source Softw.</em>, 2023 &nbsp;
[4] <a href="https://doi.org/10.1007/978-3-319-58821-6">W. Hart et al.</a>, "Pyomo," Springer, 2017 &nbsp;
[5] <a href="https://doi.org/10.1109/TPWRS.2018.2829021">L. Thurner et al.</a>, "pandapower," <em>IEEE Trans. Power Syst.</em>, vol. 33, no. 6, 2018 &nbsp;
[6] <a href="https://doi.org/10.1287/ijoc.2017.0773">Q. Huangfu & J. Hall</a>, "HiGHS," <em>INFORMS J. Comput.</em>, 2018
</span>

---

<!-- _class: lead -->

# Übung 6 – Regression
📉

---
<!-- _header: '<div class="ch"><a href="#2">📋 Orga</a></div><div class="ch"><a href="#8">🐍 0 Python</a></div><div class="ch"><a href="#10">📦 1 Git</a></div><div class="ch"><a href="#12">🤖 2 KI</a></div><div class="ch"><a href="#14">📈 3 Zeitreihen</a></div><div class="ch"><a href="#16">📊 4 Plotting</a></div><div class="ch"><a href="#19">⚡ 5 Opt.</a></div><div class="ch active"><a href="#21">📉 6 Reg.</a></div>' -->

# Regression = das einfachste ML-Modell

Die lineare Regression ist der **Einstieg in Machine Learning** [1]:

```
Komplexität
        ▲                                   Foundation Models / LLMs 
hoch    │                              Deep Learning 
        │                        Neural Networks
mittel  │              Random Forest / Boosting
        │        Polynomiale Regression
niedrig │  Lineare Regression ◄── Übung
        └─────────────────────────────────────────────► Verständlichkeit
            hoch           mittel              niedrig
```

<div class="success">

✅ Wer lineare Regression versteht, hat das **Fundament für Machine Learning** gelegt – mathematisch, konzeptionell und im Code ([scikit-learn](https://scikit-learn.org/stable/modules/linear_model.html)) [2].

</div>

→ Notebook in `6_Regression`

<span class="source">
[1] Fig. 2 aus: <a href="https://doi.org/10.1016/j.joule.2024.11.002">GridFM – Overview of ML methods in energy systems</a>, <em>Joule</em>, 2024, doi: 10.1016/j.joule.2024.11.002 &nbsp;
[2] <a href="https://jmlr.org/papers/v12/pedregosa11a.html">F. Pedregosa et al.</a>, "scikit-learn," <em>JMLR</em>, vol. 12, 2011 – <a href="https://scikit-learn.org/stable/modules/linear_model.html">Linear Models Docs</a>
</span>
