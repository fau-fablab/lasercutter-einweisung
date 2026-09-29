Lasercutter Einweisung
======================

Einweisung des [FAU FabLab](https://fablab.fau.de) für die [Lasercutter](https://fablab.fau.de/tool/lasercutter/) LTT iLaser 4000 und Epilog Zing.

Inhalt
------

- Was du dir merken musst: Regeln, Verhalten bei Flammen und im Brandfall
- Erlaubte und verbotene Materialien
- Datei erstellen und senden: Inkscape mit VisiCut, Corel/Illustrator, Windows-Treiber
- Job ausführen: Fokus, Absaugung, Air Assist, Nullpunkt, Bezahlung
- Betriebsanweisung (BA-LC-01) als eigene Seite
- Tipps zur Konstruktion (Toleranzen, Steckverbindungen, Boxen)
- Wartung und Fehlerbehebung für Betreuer, Rotationseinheit

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/lasercutter-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/lasercutter-einweisung/Einweisung_Lasercutter.pdf)
- [Betriebsanweisung](https://brain.fablab.fau.de/build/lasercutter-einweisung/Betriebsanweisung_Lasercutter.pdf) (Aushang am Gerät)
- [Einweisungsliste](https://brain.fablab.fau.de/build/lasercutter-einweisung/Einweisungsliste_Lasercutter.pdf)
- [Wartungsliste LTT](https://brain.fablab.fau.de/build/lasercutter-einweisung/Wartungsliste_Lasercutter_LTT.pdf)
- [Wartungsliste Epilog Zing](https://brain.fablab.fau.de/build/lasercutter-einweisung/Wartungsliste_Lasercutter_Epilog_Zing.pdf)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/lasercutter-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/lasercutter-einweisung.git
cd lasercutter-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/lasercutter-einweisung/status.svg)](https://brain.fablab.fau.de/build/lasercutter-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/lasercutter-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/lasercutter-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/lasercutter-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/lasercutter-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
