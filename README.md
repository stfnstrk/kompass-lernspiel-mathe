# 🎃 Halloween in Heidelsheim – Mathe-Abenteuer

Browserbasiertes Halloween-Mathe-Lernspiel für Viertklässler zur Vorbereitung auf **Kompass 4** (Baden-Württemberg): Ein Kürbis hüpft durch das festlich geschmückte Heidelsheim, und an neun Orten gibt es bei richtigen Antworten Süßes und bei falschen Saures. Dazu zeigt das Spiel Lösungswege im Stil des Unterrichts.

## So wird gespielt

1. Auf der Karte von Heidelsheim ein Haus antippen, dann hüpft der Kürbis 🎃 dorthin.
2. An jedem Haus warten **5 Aufgaben**.
   - **Süßes:** Richtig beim ersten Versuch bringt **10 Süßigkeiten** 🍬, beim zweiten Versuch (mit Tipp) **5 Süßigkeiten**.
   - **Saures:** Bei einer falschen Antwort springt eine große saure Zitrone 🍋 ins Bild.
3. Nach jeder Aufgabe zeigt der Knopf **„📝 Lösungsweg“**, wie man rechnet.
4. Ein geschafftes Haus bekommt einen Haken ✅. Die Reihenfolge ist frei wählbar.
5. Hat **jedes Haus einen Haken**, öffnet sich der **große Kürbis-Kessel am Marktplatz**. Das sind maximal 450 Süßigkeiten, der Rekord wird gespeichert.

Die Zahlen werden bei jedem Spiel neu ausgewürfelt, sodass sich das Spiel beliebig oft wiederholen lässt.

## Die Orte

| Ort | Thema | Aufgaben |
|---|---|---|
| 🔢 Dietrich-Bonhoeffer-Schule | Zahlen | Nachbartausender und Nachbarhunderter, größte und kleinste Zahl aus Ziffern, Mitte zwischen zwei Zahlen, Runden, Bündeln (z. B. 8 H \| 4 Z \| 14 E) |
| ➕ Stadttor | Plus & Minus | Schriftliche Addition und Subtraktion, Restweg-Sachaufgabe, Ergänzen bis 10.000 |
| ✖️ Römerspielplatz | Malnehmen | Malnehmen mit Zerlegen, Zehnerzahlen, Einmaleins, passende Rechnung oder Zahlenstrahl zu einer Aussage |
| ➗ Katzenturm | Teilen | Teilen mit Zerlegen, Teilen mit Rest, Bonbons gerecht aufteilen |
| ⚖️ Freibad | Größen | Zeit (min/h), Längen ordnen (mm, cm, m), Euro und Cent vergleichen, kg/g, Zeitspannen |
| 🌀 Diebsturm | Muster | Zahlenreihen fortsetzen, Kartenpaare mit gleicher Summe, Karten tauschen, „Die größere Zahl ist das Doppelte“ |
| 📐 Ewin | Formen & Körper | Baupläne, Flächen, Umfang, Ecken, Kanten und Flächen von Körpern, Spiegelachsen, Würfelnetze |
| 🎲 Annie’s | Zufall & Daten | sicher, möglich, unmöglich; Glücksrad; Kombinatorik; Tabellen, Säulendiagramme, Strichlisten |
| 💰 Bäckerei | Geld & Sachaufgaben | Brezeln und Wechselgeld, Ausflug, Eisbahn, Gruppenticket |

Die Karte ist eine vereinfachte, Halloween-geschmückte Draufsicht mit Marktplatz, Brunnen und Saalbach. Sie zeigt nicht die echte Lage der Orte.

## Lösungswege wie im Unterricht

Die Lösungswege orientieren sich an der Musterlösung der Lehrkraft:

- **Schriftliches Rechnen** auf Kästchenpapier: beim Plus mit Übertrag, beim Minus mit **Entbündeln** (⑩ über der Ziffer)
- **Malnehmen und Teilen durch Zerlegen**, z. B. 4 · 80 + 4 · 6 oder 60 : 6 + 30 : 6
- **Zahlenreihen** mit Sprung-Bögen (+5, −3 …)
- **Mitte finden** über den Zahlenstrahl
- **Sachaufgaben** mit Rechenschritten und **Antwortsatz** („A: …“)
- **Tausendertrennung mit Punkt** (1.365, 22.251)

## Starten

Das Spiel besteht aus **einer einzigen HTML-Datei** und braucht weder Installation noch Internet noch Abhängigkeiten.

- **Computer:** `halloween-heidelsheim.html` per Doppelklick im Browser öffnen (Chrome, Edge, Firefox, Safari).
- **iPhone/iPad:** Die Datei läuft in der Dateien-App nicht, weil die Vorschau dort keine Skripte ausführt. Stattdessen das Spiel online bereitstellen, z. B. über **GitHub Pages** (Datei als `index.html` ablegen), und den Link in Safari öffnen. Über „Teilen → Zum Home-Bildschirm“ wird es wie eine App gestartet.

### GitHub Pages

1. `halloween-heidelsheim.html` in `index.html` umbenennen und ins Repository legen.
2. Unter **Settings → Pages** den Branch (z. B. `main`) und `/ (root)` auswählen.
3. Nach kurzer Zeit ist das Spiel unter `https://<benutzername>.github.io/<repository>/` erreichbar.

## Hinweise

- Der **Rekord** wird im Browser gespeichert (`localStorage`), also getrennt für jedes Gerät und jeden Browser.
- Der **Fortschritt** innerhalb einer Runde (die Haken) wird nicht gespeichert. Beim Neuladen beginnt eine neue Runde.
- Antworten dürfen mit oder ohne Tausenderpunkt eingegeben werden, Geldbeträge mit Komma (z. B. `3,75`).

## Technik

- Reines HTML, CSS und JavaScript in einer Datei, ohne Frameworks
- Karte, Glücksrad, Zahlenstrahl, Würfelnetze, Strichlisten und Diagramme werden als SVG bzw. CSS erzeugt
- Für Handy, Tablet und Computer geeignet

## Lizenz

Privates Lernprojekt. Die Aufgaben sind an schulisches Übungsmaterial zur Kompass-4-Vorbereitung angelehnt, die Zahlen werden zufällig erzeugt.
