# [PROJECT TITLE]

[![release](https://img.shields.io/github/v/release/[GITHUB_USER]/[REPOSITORY]?label=release)](https://github.com/[GITHUB_USER]/[REPOSITORY]/releases)
[![Build](https://github.com/[GITHUB_USER]/[REPOSITORY]/actions/workflows/build.yml/badge.svg)](https://github.com/[GITHUB_USER]/[REPOSITORY]/actions/workflows/build.yml)
![Hardware](https://img.shields.io/badge/Hardware-KiCad-blue)
![License](https://img.shields.io/badge/License-CC--BY--NC--SA--4.0-lightgrey)

## 🔌 Leiterplattenbeschreibung

Die Leiterplatte **[PROJECT TITLE]** wurde für [kurze Beschreibung des Einsatzzwecks] entwickelt.

[Hier 2–4 Sätze zur Funktion der Leiterplatte, zum Aufbau und zum vorgesehenen Einsatz.]

### Funktionen

- [Funktion / Schaltung 1]
- [Funktion / Schaltung 2]
- [Funktion / Schaltung 3]

[Optionaler Absatz zu besonderen Eigenschaften, Messpunkten, austauschbaren Bauteilen, Schnittstellen usw.]

> **Einsatzgebiet:** [Kurze Beschreibung des vorgesehenen Einsatzes]

---

## 📥 Downloads

| Datei | Beschreibung |
|---|---|
| 📄 [Schaltplan (PDF)](../../releases/latest/download/schematic.pdf) | Schaltplan der Leiterplatte |
| 🖨️ [Leiterplatte (PDF)](../../releases/latest/download/pcb.pdf) | Leiterplattenansicht als PDF |
| 🔩 [Bohrplan (PDF)](../../releases/latest/download/drill.pdf) | Bohrdaten / Bohrplan |
| 📋 [Stückliste (Excel)](../../releases/latest/download/bom.xlsx) | Bill of Materials |
| 🌐 [Interactive BOM](../../releases/latest/download/ibom.html) | Interaktive Bestückungsansicht |
| 📦 [Fertigungsdaten](../../releases/latest/download/kicad.zip) | Gerber- und Bohrdaten |
| 🧊 [STEP-Modell](../../releases/latest/download/pcb.step) | 3D-Modell der Leiterplatte |

Die Dateien werden automatisch durch den Release-Workflow erzeugt.

---

## 🖥️ Leiterplatte

### Vorschau

| Oberseite | Unterseite |
|:---:|:---:|
| ![PCB Top](../../releases/latest/download/top.kicad.thumbnail.png) | ![PCB Bottom](../../releases/latest/download/bottom.kicad.thumbnail.png) |

### Oberseite

![PCB Top](../../releases/latest/download/top.kicad.png)

### Unterseite

![PCB Bottom](../../releases/latest/download/bottom.kicad.png)

---

## ℹ️ Projektinformationen

| Eigenschaft | Wert |
|---|---|
| **Projekt** | [PROJECT TITLE] |
| **Software** | KiCad 10 |
| **Repository** | [GITHUB_USER]/[REPOSITORY] |
| **Autor** | [NAME] |
| **Lizenz** | CC BY-NC-SA 4.0 |

---

## 🗂️ Repository-Struktur

```text
.
├── .github/
│   └── workflows/       # GitHub Actions
├── .kibot/              # KiBot-Konfiguration
├── pcb/
│   ├── lib/             # Projektspezifische Bibliotheken
│   └── ...              # KiCad-Projektdateien
├── .gitignore
├── LICENSE
└── README.md