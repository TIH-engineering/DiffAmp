# DiffAmp

[![release](https://img.shields.io/github/v/release/github.com/TIH-engineering/DiffAmp?label=release)](https://github.com/github.com/TIH-engineering/DiffAmp/releases)
[![Build](https://github.com/github.com/TIH-engineering/DiffAmp/actions/workflows/build.yml/badge.svg)](https://github.com/github.com/TIH-engineering/DiffAmp/actions/workflows/build.yml)
![Hardware](https://img.shields.io/badge/Hardware-KiCad-blue)
![License](https://img.shields.io/badge/License-CC--BY--NC--SA--4.0-lightgrey)

## 🔌 Leiterplattenbeschreibung

Die Leiterplatte **DiffAmp** dient zur praktischen Untersuchung von **Differenzverstärkern**. Sie ermöglicht den Vergleich einer diskret mit Transistoren aufgebauten Differenzverstärkerstufe mit einem Differenzverstärker auf Basis eines **Operationsverstärkers**.

Die Leiterplatte enthält zwei unterschiedliche Schaltungsvarianten:

- **Differenzverstärker mit zwei Bipolartransistoren**
- **Differenzverstärker mit Operationsverstärker (Subtrahierer)**

Der diskrete Differenzverstärker kann über Jumper in unterschiedlichen Betriebsarten betrieben werden. Die gemeinsame Emitterbeschaltung der beiden Transistoren kann wahlweise mit einem **Emitterwiderstand** oder mit einer **Stromquelle** realisiert werden. Dadurch lässt sich der Einfluss der Stromquellenschaltung auf das Verhalten des Differenzverstärkers praktisch untersuchen.

Zusätzliche Jumper ermöglichen unterschiedliche Messkonfigurationen zur Bestimmung der

- **Gegentaktverstärkung**
- **Gleichtaktverstärkung**

Damit können aus den Messwerten auch die Unterschiede zwischen Gegentakt- und Gleichtaktansteuerung sowie die **Gleichtaktunterdrückung** des Differenzverstärkers untersucht werden.

Als Vergleichsschaltung ist zusätzlich ein Differenzverstärker mit einem **LM358-Operationsverstärker** aufgebaut. Dieser arbeitet als Subtrahierer und bildet die Differenz der beiden Eingangssignale `In1` und `In2`.

Die verschiedenen Ausgangssignale der Schaltungen stehen an separaten Anschlüssen zur Verfügung und können beispielsweise mit einem **Oszilloskop** vermessen und miteinander verglichen werden.

> **Einsatzgebiet:** Laborübungen und Unterricht zu Differenzverstärkern, Operationsverstärkern, Gegentakt- und Gleichtaktverstärkung sowie Gleichtaktunterdrückung

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
| **Projekt** | DiffAmp |
| **Software** | KiCad 10 |
| **Repository** | github.com/TIH-engineering/DiffAmp |
| **Autor** | TIH |
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