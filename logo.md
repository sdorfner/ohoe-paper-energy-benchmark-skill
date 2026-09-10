# Logo — Open House of Energy

Quelle: OHOE Brand Guidelines V1.1, Folie "Logo".

## Logo-Datei

`assets/logo_ohoe_lang.png` — aktuelle, freigestellte Logo-Datei (668×110px, transparenter Hintergrund). Dies ist die **"Lange Version"** des Logos (volle Schriftzug-Breite "Open House of Energy").

Laut Guidelines gibt es eine **Standard-Version** (kompakter, für die meisten Anwendungen) und die **Lange Version** (nur verwenden, wenn für die Standard-Version nicht genug Platz vorhanden ist, z.B. sehr schmale Kopfzeilen). Liegt nur die lange Version vor, diese verwenden — aber bei knappem Platz in Betracht ziehen, sie stärker zu verkleinern statt zu stauchen.

## Pflicht-Regeln

- **Bevorzugte Farbgebung:** Standardversion in OHOE Grau & Rot, idealerweise auf weißem Hintergrund.
- **Andere Hintergründe:** nur wenn der Hintergrund ruhig genug ist, dass das Logo klar erkennbar bleibt.
- **Niemals verändern:** nicht stauchen, strecken, verzerren, umfärben oder anderweitig verändern.
- **Immer freigestellt** darstellen (keine eigene Box/kein Rahmen um das Logo).
- **Mindesthöhe:** 15 mm (≈ 0.59" in PowerPoint bei 16:9-Folien).
- **Mindestabstand zu anderen Elementen:** eine Höhe der Logo-Großbuchstaben ("Clearspace" = 1× Cap-Height).

## Platzierung (Standard, 16:9-Folie/Dokument)

Oben rechts, z.B. in PowerPoint: `x: 8.3, y: 0.08, w: 1.55, h: 0.72` (Zoll).

Für Dokumente/Web: oben rechts oder oben links in der Kopfzeile, mit ausreichend Weißraum gemäß Clearspace-Regel.

## Verwendung je Ausgabeformat

- **PowerPoint:** über `pptx-creator`-Skill einbinden (dort liegt das Logo bereits als Base64-Konstante vor, abgeglichen mit dieser Datei).
- **Word/PDF:** `assets/logo_ohoe_lang.png` als Bild in Kopfzeile/Deckblatt einfügen.
- **HTML/React-Artifacts, Gamma, Web:** Datei als `<img src="...">` einbinden oder zu Base64 konvertieren, wenn eine einzelne portable Datei benötigt wird.

## Don'ts (laut Guidelines)

- Logo nicht verzerren/stauchen/strecken
- Logo nicht einfärben oder mit Farbverlauf versehen
- Logo nicht auf unruhigen/kontrastarmen Hintergründen platzieren
- Logo nicht kleiner als die Mindesthöhe abbilden
- Keinen eigenen Rahmen/Schlagschatten um das Logo legen
