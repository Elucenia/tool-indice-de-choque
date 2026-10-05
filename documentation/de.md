<!-- ELUCENIA technical documentation · indice-de-choque · de · no clinical/professional/rights approval -->

# Schockindex (und modifizierter Schockindex)

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/indice-de-choque)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Herzfrequenz

`fc`

bpm · Bereich: 20–250

### Systolischer Blutdruck

`pas`

mmHg · Bereich: 30–300

### Diastolischer Druck (für den modifizierten Index)

`pad`

mmHg · optional · Bereich: 10–200

## Fassung der Methode

Schockindex/Allgöwer 1967 HF/SBD und modifizierter Schockindex/Liu 2012 HF/MAP

## Dokumentierte Formel

Schockindex = HF ÷ SBD (normal: 0,5–0,7).

Modifizierter Schockindex = HF ÷ MAP, mit MAP = DBD + (SBD − DBD) ÷ 3 (normal: 0,7–1,3).

## Grenzen und Population

Der Schockindex ist die Herzfrequenz geteilt durch den systolischen Blutdruck; der modifizierte Index verwendet den mittleren arteriellen Druck. Dies sind unterschiedliche Verhältnisse und sie diagnostizieren allein weder einen Schock noch einen Transfusionsbedarf. Mutschler 2013 untersuchte den Index bei Notaufnahmeankunft von 21.853 erwachsenen Traumapatienten; Liu 2012 untersuchte retrospektiv 22.161 Patienten im Alter von 10 bis 100 Jahren mit intravenöser Flüssigkeitsgabe und schloss reanimierte Herz-Kreislauf-Stillstände ohne Triage aus. Diese Kohorten belegen keine universellen Grenzwerte für Kinder aller Altersgruppen, Schwangere oder andere Situationen. Dokumentieren Sie Zeitpunkt und Messbedingungen; Zusammenhänge einer Kohorte mit der Krankenhausmortalität sind keine automatischen individuellen Vorhersagen.

## Referenzen

- [Allgöwer M, Burri C. „Schockindex". Dtsch Med Wochenschr, 1967.](https://doi.org/10.1055/s-0028-1106070)

- [Mutschler M et al. The Shock Index revisited – a fast guide to transfusion requirement? A retrospective analysis on 21,853 patients derived from the TraumaRegister DGU. Crit Care, 2013.](https://doi.org/10.1186/cc12851)

- [Liu YC et al. Modified shock index and mortality rate of emergency patients. World J Emerg Med, 2012.](https://doi.org/10.5847/wjem.j.issn.1920-8642.2012.02.006)

- [Liu2012](https://pmc.ncbi.nlm.nih.gov/articles/PMC4129788/)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026
