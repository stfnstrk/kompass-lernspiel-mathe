# 🎃 Halloween in Heidelsheim – Mathe-Abenteuer

**Version 1.1.0**

Browserbasiertes Halloween-Mathe-Lernspiel für Viertklässler zur Vorbereitung auf **Kompass 4** (Baden-Württemberg): Ein Kürbis hüpft durch das festlich geschmückte Heidelsheim, und an neun Orten gibt es bei richtigen Antworten Süßes und bei falschen Saures. Dazu zeigt das Spiel Lösungswege im Stil des Unterrichts.

## So wird gespielt

1. Auf der Karte von Heidelsheim ein Haus antippen, dann hüpft der Kürbis 🎃 dorthin.
2. An jedem Haus warten **5 Aufgaben**.
   - **Süßes:** Richtig beim ersten Versuch bringt **10 Süßigkeiten** 🍬, beim zweiten **5**, beim dritten **2**.
   - **Saures:** Bei jeder falschen Antwort springt eine große saure Zitrone 🍋 ins Bild.
   - Nach dem 1. Fehler gibt es nur einen neuen Versuch, nach dem 2. Fehler einen **Tipp**, nach dem 3. Fehler die **Lösung mit Lösungsweg**. Bei Auswahlfragen mit nur zwei oder drei Antworten kommt die Lösung entsprechend früher.
3. Nach jeder Aufgabe zeigt der Knopf **„📝 Lösungsweg“**, wie man rechnet.
4. Ein geschafftes Haus bekommt einen Haken ✅. Die Reihenfolge ist frei wählbar.
5. Hat **jedes Haus einen Haken**, öffnet sich der **große Kürbis-Kessel am Marktplatz**. Das sind maximal 450 Süßigkeiten, der Rekord wird gespeichert.

Die Zahlen werden bei jedem Spiel neu ausgewürfelt, sodass sich das Spiel beliebig oft wiederholen lässt.

## Die Orte

| Ort | Thema | Aufgaben |
|---|---|---|
| 🔢 Dietrich-Bonhoeffer-Schule | Zahlen | Nachbartausender und Nachbarhunderter, größte und kleinste Zahl aus Ziffern, Mitte zwischen zwei Zahlen, Bündeln (z. B. 8 H \| 4 Z \| 14 E) |
| ➕ Stadttor | Plus & Minus | Schriftliche Addition und Subtraktion, Restweg-Sachaufgabe |
| ✖️ Römerspielplatz | Malnehmen | Malnehmen mit Zerlegen (z. B. 4 · 86), mal Zehnerzahl (5 · 20), passende Rechnung oder Zahlenstrahl zu einer Aussage |
| ➗ Katzenturm | Teilen | Teilen mit Zerlegen (z. B. 90 : 6, 60 : 5) |
| ⚖️ Freibad | Größen | Minuten in Stunden, Längen ordnen und vergleichen (mm, cm, m), Euro und Cent vergleichen |
| 🌀 Diebsturm | Muster | Zahlenreihen fortsetzen, Kartenpaare mit gleicher Summe, Karten tauschen, „Die größere Zahl ist das Doppelte“ |
| 📐 Ewin | Formen & Körper | Baupläne, Flächen (Kästchen), Ecken, Kanten und Flächen von Körpern, Spiegelachsen, Würfelnetze |
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
- Der **Spielstand** (Haken und Süßigkeiten) wird nach jedem geschafften Haus im Browser gespeichert. Nach dem Neuladen geht es dort weiter. Ein angefangenes Haus beginnt von vorn.
- „Neues Spiel“ fragt nach, bevor der Spielstand gelöscht wird. Der Rekord bleibt erhalten.
- Antworten dürfen mit oder ohne Tausenderpunkt eingegeben werden, Geldbeträge mit Komma (z. B. `3,75`).

## Technik

- Reines HTML, CSS und JavaScript in einer Datei, ohne Frameworks
- Karte, Glücksrad, Zahlenstrahl, Würfelnetze, Strichlisten und Diagramme werden als SVG bzw. CSS erzeugt
- Für Handy, Tablet und Computer geeignet

## Versionen

Die Versionsnummer steht unten im Spiel unter „Neues Spiel“. Bei jeder Änderung wird die letzte Stelle hochgezählt (1.1.0 → 1.1.1 …), bei neuen Funktionen nach Absprache die mittlere (1.0 → 1.1).

| Version | Änderung |
|---|---|
| 1.1.0 | Spielstand wird gespeichert (Haken und Süßigkeiten), „Willkommen zurück“ beim Neuladen, Rückfrage bei „Neues Spiel“ |
| 1.0.0 | Erste Version mit Versionsnummer: Halloween in Heidelsheim, 9 Orte, Süßes oder Saures, Lösungswege, Tipps in drei Stufen, Abbrechen-Knopf, nur Aufgabentypen aus den Übungsscans |

## Lizenz

Privates Lernprojekt. Alle Aufgabentypen stammen aus dem schulischen Übungsmaterial zur Kompass-4-Vorbereitung, die Zahlen werden zufällig erzeugt.
