---
name: ohoe-corporate-identity
description: Wendet das Corporate Identity Design von Open House of Energy (OHOE, www.ohoe.eu) konsequent auf jedes für OHOE erstellte Dokument an — PowerPoint, Word/PDF, HTML/React-Artifacts, Gamma-Präsentationen, Landingpages, One-Pager, E-Mails. Enthält die offiziellen Marken-Farben, Schriften, Logo-Regeln (inkl. Logo-Datei), Sprach-/Namensregeln (Langform/Kurzform, E³ngine-Schreibweise, Copyright, Disclaimer, Dokumenten-Klassifizierung) sowie Bildsprache-, Icon- und Formen-Richtlinien gemäß den offiziellen OHOE Brand Guidelines. IMMER konsultieren, sobald für OHOE irgendein Dokument, eine Präsentation, ein Artifact, ein Mockup, eine Website oder Marketing-/Kommunikationsmaterial erstellt wird — auch wenn "CI" oder "Corporate Identity" nicht explizit erwähnt wird, sondern nur "OHOE", "Open House of Energy" oder ein konkreter Firmenname/Kunde von OHOE im Kontext steht. Bei PowerPoint-Dateien zusätzlich immer den `pptx-creator`-Skill laden.
---

# OHOE Corporate Identity

Quelle: offizielle **OHOE_BrandGuidelines_2021.pptx** (Version 1.1, März 2021, `assets/OHOE_BrandGuidelines_2021.pptx`) plus das aktuelle Logo (`assets/logo_ohoe_lang.png`). Bei Widersprüchen zu älteren Annahmen (z.B. abweichende Akzentfarben in älteren Skills/Decks) gilt **dieses Dokument als Quelle der Wahrheit**.

## Checkliste — bei jedem OHOE-Dokument

1. Nur die Farben aus `references/farben-schriften.md` verwenden — kein anderes Farbprofil.
2. Nur Arial (Überschriften) / Arial Narrow (Fließtext) — siehe `references/farben-schriften.md`.
3. Logo aus `assets/logo_ohoe_lang.png` einbinden, Mindestgröße & Freiraum beachten — siehe `references/logo.md`.
4. Erste Erwähnung "Open House of Energy", danach "OHOE" — Details in `references/sprache-copy.md`.
5. Klare, flächige Formen ohne Outline/Schatten/Verlauf; max. 2 Linienstärken pro Seite — siehe `references/bildsprache-formen.md`.
6. Akzentfarben (Grün/Blau/Gelb) sparsam, max. 1 pro Seite/Ansicht.

## Referenzdateien

| Datei | Inhalt |
|---|---|
| `references/farben-schriften.md` | Hex-Codes Haupt-/Akzentfarben, Schriftarten & -größen, CSS-Variablen für HTML/Artifacts/Gamma |
| `references/logo.md` | Logo-Datei, Mindestgröße, Freiraum, Varianten, Don'ts |
| `references/sprache-copy.md` | Lang-/Kurzform, juristischer Name, E³ngine-Schreibweise, Copyright-Zeile, Disclaimer-Text, Dokumenten-Klassifizierung |
| `references/bildsprache-formen.md` | Formen/Schatten/Linien, Icon-Stil, Foto-/Bildsprache |

## Format-spezifisches Vorgehen

- **PowerPoint (.pptx):** Immer zusätzlich den `pptx-creator`-Skill laden — der enthält fertige PptxGenJS-Layouts, Logo als Base64 und ist bereits auf dieselben CI-Werte abgeglichen (siehe Hinweis unten).
- **Word/PDF/Berichte:** Farben, Schriften und Logo-Regeln aus den Referenzdateien direkt übernehmen (Deckblatt mit Logo oben rechts, Überschriften Arial, Fließtext Arial Narrow, Fußzeile mit Copyright-Zeile).
- **HTML/React-Artifacts, Web-Mockups, Landingpages, Gamma:** CSS-Variablen aus `references/farben-schriften.md` nutzen; Logo als `<img>` mit Pfad `assets/logo_ohoe_lang.png` bzw. dessen Base64 einbetten (Web nutzt laut Guidelines die Schriftart **Roboto**, nicht Arial — siehe Referenzdatei).
- **E-Mails/Sales-Assets/One-Pager:** Copy-Regeln aus `references/sprache-copy.md` (Langform zuerst, Copyright-Zeile bei Dokumenten) plus Farben/Logo wie oben.

## Abgleich mit bestehendem `pptx-creator`-Skill

Der `pptx-creator`-Skill enthielt bislang eigene, leicht abweichende Akzentfarben (Grün/Blau/Gelb). Dieser Skill korrigiert sie anhand der offiziellen Brand Guidelines auf `36D663` / `008ED6` / `FFBE00`. Rot (`D63636`), Grau (`333333`), Schwarz (`242424`) und Hellgrau (`EDEDED`) waren bereits korrekt. Der `pptx-creator`-Skill wurde entsprechend aktualisiert, sodass beide Skills konsistent dieselben Werte verwenden.
