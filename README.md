# Stundenerfassung
Kernfunktionen

Tageserfassung: Eingabe von Datum, Mitarbeitern, Baustellen (mit KTR-Nummer), Arbeitszeiten (bis zu 3 Zeitfenster pro Einsatz) und Zusatzdaten (Reisezeit, Fahrer, Mittagszulage, Begründungen).

Automatische Berechnung: Berechnet die Einsatz- und Tagesgesamtzeiten sowie Ist-Stunden in Echtzeit.

Wochen-Speicher: Speichert einzelne Tage im Browser-Speicher (localStorage) ab, um eine komplette Arbeitswoche zu sammeln.

Wochen-Archiv & Nachbearbeitung: Zeigt bereits abgeschlossene Wochen in einem digitalen Archiv an. Archivierte Wochen können wieder geladen, nachträglich bearbeitet und erneut abgespeichert werden.

PDF-Generierung: Erstellt beim Wochenabschluss für jeden beteiligten Mitarbeiter automatisch eine eigene, im Querformat formatierte PDF-Stundenkarte inklusive Soll/Ist-Vergleich und Legendenschlüssel.

Funktionsweise

Frontend: Die Anwendung besteht aus HTML, CSS und JavaScript und läuft ohne eigenen Server direkt im Webbrowser.

Lokaler Speicher (localStorage): Speichert automatisch Stammdaten (Mitarbeiterliste, Baustellen-KTR-Zuordnungen), Entwürfe, die aktuelle Woche sowie das Archiv auf dem Gerät des Nutzers.

PDF-Bibliothek: Verwendet jsPDF und jspdf-autotable, um aus den erfassten Daten direkt im Browser druckfähige PDF-Dateien im Layout der Firma Ghelma AG Spezialtiefbau zu generieren.

Tag kann erst abgelegt werden, wenn mindestens eine Baustelle erfasst ist und ein Zeitfenster.
