# Kommunalwahlen Niedersachsen 2026 – Ergebnisse

Interaktive Auswertung der niedersächsischen Kommunalwahlen vom 13. September 2026:
Kreiswahlen, Rats- und Samtgemeinderatswahlen sowie die Direktwahlen der Landräte,
Oberbürgermeister und Bürgermeister. Die Seite ist eine einzelne HTML-Datei ohne
Server, ohne Build-Schritt und ohne externe Abhängigkeiten außer den Schriften von
Google Fonts.

## Inhalt

```
index.html          die vollständige Auswertung (Daten sind eingebettet)
daten/page_data.json    die eingebetteten Daten als eigenständige Datei
daten/Kommunalwahl_Niedersachsen_2026.xlsx    dieselben Ergebnisse als Arbeitsmappe
.nojekyll           schaltet die Jekyll-Verarbeitung auf GitHub Pages ab
```

## Veröffentlichen über GitHub Pages

```bash
git init
git add .
git commit -m "Kommunalwahlen Niedersachsen 2026"
git branch -M main
git remote add origin git@github.com:BENUTZER/REPOSITORY.git
git push -u origin main
```

Anschließend im Repository unter *Settings → Pages* als Quelle „Deploy from a branch"
wählen, Branch `main` und Ordner `/ (root)`. Nach ein bis zwei Minuten liegt die Seite
unter `https://BENUTZER.github.io/REPOSITORY/`.

Für eine eigene Domain dort zusätzlich *Custom domain* eintragen; GitHub legt dann eine
Datei `CNAME` an.

## Datenstand und Quellen

Die Zahlen stammen aus den amtlichen Ergebnispräsentationen der Kommunen, überwiegend
aus dem System votemanager, für die Landkreise Celle und Uelzen aus deren eigenem
System. Der Stand der Auszählung steht im Kopf der Seite. Solange Ist- und
Soll-Wahlbezirke voneinander abweichen, handelt es sich um Zwischenstände.

Das ausgewiesene Gesamtergebnis ist die Summe der erfassten Kreiswahlen und der
Ratswahlen der kreisfreien Städte. Es ist **kein amtliches Landesergebnis**; dieses
veröffentlicht das Landesamt für Statistik unter
<https://wahlen.statistik.niedersachsen.de/KW2026/>.

Nicht enthalten ist der Heidekreis, dessen Ergebnisserver beim Abruf nicht erreichbar
war. Für Celle und Uelzen liegen Kreistags- und Landratswahl vor, aber keine
Einzelergebnisse der Gemeinden.

## Hinweise zur Darstellung

Bei den Listenwahlen hat jeder Wähler drei Stimmen. Ausgewiesen ist die Summe aus
Partei- und Kandidatenstimmen, wie sie die Kommunen veröffentlichen. Wählergemeinschaften,
Einzelbewerber und Kleinparteien sind unter „Sonstige" zusammengefasst.

## Vor der Veröffentlichung

Im Footer von `index.html` steht ein Platzhalter für Impressum und Datenschutzerklärung.
Für eine öffentlich zugängliche Seite sind diese Angaben zu ergänzen.

## Lizenz

Die Wahlergebnisse sind amtliche Daten der jeweiligen Kommunen. Für Code und
Aufbereitung ist eine Lizenz zu ergänzen, falls das Repository öffentlich sein soll.
