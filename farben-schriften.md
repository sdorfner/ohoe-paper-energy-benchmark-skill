# Farben & Schriften — Open House of Energy

Quelle: OHOE Brand Guidelines V1.1 (März 2021), Folie "Brand colours" / "Fonts".

## Farben

### Basis (dominieren jede Seite)

| Name | Hex | RGB | Einsatz |
|---|---|---|---|
| OHOE Rot | `D63636` | 214, 54, 54 | Primärfarbe — Energie & Action |
| OHOE Grau | `333333` | 51, 51, 51 | Haupttextfarbe |
| Schwarz | `242424` | 36, 36, 36 | Fast-Schwarz, dunkle Flächen |
| Mid Grey | `515151` | 81, 81, 81 | Sekundärtext, Captions |
| Light Grey | `EDEDED` | 237, 237, 237 | Hintergründe, Trennlinien |
| Weiß | `FFFFFF` | 255, 255, 255 | Bright white — nie Cream/Off-White |

### Akzente (max. 1 pro Seite, sparsam einsetzen)

| Name | Hex | RGB |
|---|---|---|
| Grün | `36D663` | 54, 214, 99 |
| Blau | `008ED6` | 0, 142, 214 |
| Gelb | `FFBE00` | 255, 190, 0 |

**Hinweis:** Frühere Versionen des `pptx-creator`-Skills verwendeten leicht andere Akzentwerte (Grün `6BC66B`, Blau `80D3FF`, Gelb `FFDC4E`). Die Werte oben sind die offiziell dokumentierten und sollten ab sofort durchgängig verwendet werden.

**Farbgewichtung:** Rot + Grau dominieren. Nie mehrere Akzentfarben gleichzeitig auf einer Fläche.

### Als JS-Konstante (PptxGenJS o.ä.)

```javascript
const CI = {
  red:       "D63636",
  grey:      "333333",
  black:     "242424",
  midGrey:   "515151",
  lightGrey: "EDEDED",
  white:     "FFFFFF",
  green:     "36D663",
  blue:      "008ED6",
  yellow:    "FFBE00",
};
```

### Als CSS-Variablen (HTML/React-Artifacts, Gamma, Landingpages)

```css
:root {
  --ohoe-red: #D63636;
  --ohoe-grey: #333333;
  --ohoe-black: #242424;
  --ohoe-mid-grey: #515151;
  --ohoe-light-grey: #EDEDED;
  --ohoe-white: #FFFFFF;
  --ohoe-green: #36D663;
  --ohoe-blue: #008ED6;
  --ohoe-yellow: #FFBE00;
}
```

## Schriften

| Kontext | Font | Hinweis |
|---|---|---|
| MS Office — Überschriften | Arial | Fett so wenig wie möglich; lieber Größenstufen statt Bold nutzen |
| MS Office — Fließtext | Arial Narrow | Regular; auch kursiv vermeiden |
| Web — Fließtext/Überschriften | Roboto | Beste Lesbarkeit im Web |
| Web — Ergebnis-/Datentabellen | Roboto Mono | Kondensiert, Zahlen in gleicher Breite |

**Typografie-Grundregel laut Guidelines:** Fett und Kursiv so sparsam wie möglich einsetzen. Textstruktur lieber über unterschiedliche Schriftgrößen erzeugen als über Schriftschnitte.

**Größenempfehlung (aus pptx-creator-Praxis, für PowerPoint):**
- Folientitel: 28–36pt Arial
- Abschnittsüberschrift: 18–22pt Arial
- Fließtext: 12–14pt Arial Narrow
- Captions/Labels: 9–11pt Arial Narrow, Farbe `515151`
