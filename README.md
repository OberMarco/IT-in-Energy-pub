# IT in der Energiewirtschaft

Dieses Repository enthält Materialien und Übungen für den Kurs [**IT in der Energiewirtschaft**](https://obermarco.github.io/IT-in-Energy/#1).

## Voraussetzungen

- [Anaconda](https://www.anaconda.com/) oder [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
- Git

## Installation

```bash
# Repository klonen
git clone https://github.com/OberMarco/IT-in-Energy-pub.git
git clone gh repo clone OberMarco/IT-in-Energy-pub
git clone git@github.com:OberMarco/IT-in-Energy-pub.git
cd 5_IT-in-Energy

# Conda-Umgebung erstellen und aktivieren
conda env create -f environment.yml
conda activate environment_it_energy
```

# Installation testen
```bash
code 00_Test_Installation.ipynb
```

# Struktur

```
5_IT-in-Energy/
│
├── 0_Wiederholung_Python/             ← Übung 0: Python-Wiederholung
├── 1_Intro_Git/                       ← Übung 1: Git-Befehle & Workflow
├── 2_KI_unterstuetze_Programmierung/  ← Übung 2: KI-gestütztes Programmieren
├── 3_Zeitreihen/                      ← Übung 3: Zeitreihen & Stromkosten
├── 4_Plots_in_Python/                 ← Übung 4: Visualisierung
├── 5_Optimimierung/                   ← Übung 5: Linopy & PyPSA
├── 6_Regression/                      ← Übung 6: Lineare Regression
│
├── 00_Test_Installation.ipynb         ← Installationstest 
├── README.md                          ← Diese Datei
└── environment.yml                    ← Conda-Umgebungsdefinition

```
