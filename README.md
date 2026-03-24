# IT in der Energiewirtschaft

Dieses Repository enthält Materialien und Übungen für den Kurs [**IT in der Energiewirtschaft (Präsentationslink)**](https://obermarco.github.io/IT-in-Energy/#1).

## Voraussetzungen

- [Anaconda](https://www.anaconda.com/) oder [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
- Git
- VScode

## Installation für private Laptops

### Windows

Powershell öffnen und folgende Befehle ausführen:
```powershell
winget install --id Anaconda.Miniconda3        --silent --accept-package-agreements --accept-source-agreements
winget install --id Git.Git                    --silent --accept-package-agreements --accept-source-agreements
winget install --id Notepad++.Notepad++        --silent --accept-package-agreements --accept-source-agreements
winget install --id Microsoft.VisualStudioCode --silent --accept-package-agreements --accept-source-agreements
```

### Ubuntu

```bash
sudo apt update
sudo apt install -y python3 python3-pip git code
```

### MacOS

Homebrew (Paketmanager ähnlich wie der App Store bei einem iPhone) installieren
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Befehl zum Installieren der benötigten Software ausführen
```bash
brew install --cask miniconda
brew install --cask git
brew install --cask visual-studio-code
```

### GitHub Repository klonen und Conda-Umgebung erstellen

```bash
# Repository klonen
git clone https://github.com/OberMarco/IT-in-Energy-pub.git
git clone gh repo clone OberMarco/IT-in-Energy-pub # Alternative mit GitHub CLI
git clone git@github.com:OberMarco/IT-in-Energy-pub.git # Alternative mit SSH
cd 5_IT-in-Energy # in das geklonte Repository wechseln

# Conda-Umgebung erstellen und aktivieren
conda env create -f environment.yml 
conda activate environment_it_energy
```

### In VSCode öffnen

```bash
code
```

# Installation testen
```bash
code 00_Test_Installation.ipynb
```

# Ordnerstruktur

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
