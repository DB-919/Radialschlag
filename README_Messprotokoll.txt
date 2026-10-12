BECKER TOOLS – MESSPROTOKOLL (WEB-APP)
====================================

INHALT
- index.html             Vollständige Messwert-App mit Excel- und CSV-Export
- manifest.webmanifest  Web-App-Konfiguration
- sw.js                  Offline-Unterstützung bei Veröffentlichung über HTTPS
- icon-192.png          App-Icon
- icon-512.png          App-Icon

EINFACH AM PC STARTEN
Die Datei index.html per Doppelklick im Browser öffnen.
Für den reinen PC-Einsatz genügt die einzelne HTML-Datei.

IPHONE-APP ÜBER GITHUB PAGES
1. ZIP-Datei entpacken.
2. Die fünf Dateien index.html, manifest.webmanifest, sw.js,
   icon-192.png und icon-512.png in das GitHub-Repository hochladen.
3. Unter Settings > Pages die Veröffentlichung aus dem main-Branch
   (Root-Verzeichnis) aktivieren bzw. die vorhandenen Pages-Einstellungen verwenden.
4. Die GitHub-Pages-Adresse in Safari auf dem iPhone aufrufen.
5. Safari > Teilen > Zum Home-Bildschirm.
6. Die App einmal online laden, damit sie für spätere Offline-Nutzung
   zwischengespeichert werden kann.

VERWENDUNG
- 'Projekt / Bauteil', 'Prüfzustand' (z.B. nach T7) und Soll-Ø eintragen.
- Standard-Messverfahren Radius: Referenz = Soll-Durchmesser / 2.
- Alternativ 'Durchmesser messen' wählen: Referenz = Soll-Durchmesser.
- Abweichung = Messwert - Referenz.
- Soll-Ø kann je Position separat überschrieben werden.
- Optional Untergrenze und Obergrenze der zulässigen Abweichung
  eintragen, damit 'i.O.' und 'n.i.O.' automatisch berechnet werden.
- Messwerte in Tabelle oder über die große Schnellerfassung eingeben.
- Mit 'Beispieldaten' lassen sich die 16 Messwerte aus der Beispielabbildung laden.
- Excel (.xlsx) exportiert die Blätter Messprotokoll, Auswertung und Einstellungen.
  Referenz, Abweichung und Bewertung sind dort weiterhin als Formeln hinterlegt.
- CSV eignet sich zum Austausch; JSON zur Wiederherstellung eines Projekts.

DATENSCHUTZ UND DATENSICHERUNG
Die App sendet keine Messwerte an einen Server. Messdaten werden nur
im lokalen Browserspeicher des jeweiligen Geräts abgelegt. Safari kann
Websitedaten löschen oder App-Daten verlieren. Für dauerhaftes Archivieren
immer Excel und vorzugsweise eine JSON-Sicherung exportieren.

WICHTIG
- Zahlen mit Komma oder Punkt sind zulässig.
- Eine leere Messzelle erzeugt KEINE Abweichung (nicht fälschlich -Soll/2).
- Für die Toleranzbewertung müssen beide Grenzen ausgefüllt sein.
- Excel-Dateien werden im Browser erzeugt, ohne externe JavaScript-Bibliothek.
