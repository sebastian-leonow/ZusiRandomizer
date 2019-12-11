# ZusiRandomizer
Konsolenprogramm um Fahrpläne von Zusi3 mit Verspätungen durch längere Bahnsteigaufenthalte zu versehen.

Benutzung:
1. ZusiRandomizer.exe muss im Zug-Verzeichnis liegen, z.B. Zusi3\Timetables\Deutschland\Koeln_Duesseldorf\Koeln-Duesseldorf_2016_00Uhr-08Uhr\
2. Nach dem Starten meldet ZusiRandomizer die Zahl der gefundenen Züge.
3. Über die Auswahl von [v] kann die Generierung von zufälligen Verspätungen begonnen werden, über [u] wird der Grundzustand der Zug-Dateien wiederhergestellt.
4. ZusiRandomizer sichert zuerst die Zug-Dateien (legt Kopien mit der Endung _orig an). Anschließend werden die Verspätungen erzeugt.
5. Bei jeder Ausführung wird zuerst der Grundzustand wiederhergestellt (aus den _orig Dateien)

Hinweise:
- Unbedingt vorher eine Sicherung der Zug-Dateien machen!
- Die Verspätungen sind für alle Halte gleichverteilt im Intervall zwischen 0 und 10 Minuten (anpassbar).
- Jeder Zug wird zusätzlich mit einem "Grundrauschen", d.h. Verspätungen im Sekundenbereich versehen.
- S-Bahnen werden aktuell nur mit dem Grundrauschen versehen, um die Fahrpläne nicht komplett zusammenbrechen zu lassen.
- Getestet habe ich auf Köln-Düsseldorf und Augsburg-Donauwörth.
- Der Zusi interne Zufallsfaktor sollte gering (ggf. auf 0) eingestellt werden, sonst wird sich der Fahrplan schnell zufahren.