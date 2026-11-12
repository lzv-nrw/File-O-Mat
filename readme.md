# File-O-Mat / Evaluate File Formats

https://www.lzv.nrw/file-o-mat/

Ein einfach zu bedienender Fragebogen, der hilft, Dateiformate auf ihre Eignung zur Langzeitverfügbarkeit zu evaluieren. Das Ergebnis ist eine nach Kriterien aufgeschlüsselte Risikoanalyse.

Einige der Fragen und Gewichtungen sind einem bash-Tool von Andreas Romeyke/[SLUB Dresden](https://git.slub-dresden.de/digital-preservation/judge_fileformats) übernommen. 

Die Web-Applikation basiert auf Mat-O-Wahl von Mathias Steudtner ([Webseite](https://www.mat-o-wahl.de/)/ [GitHub](https://github.com/msteudtn/Mat-O-Wahl)).

Alle Daten werden im Browser der Nutzenden verarbeitet. Nach Verlassen der Seite gehen sämtliche Eingaben verloren, sofern sie nicht lokal gesichert werden.

Der Fragenkatalog liegt in Form einer Tabelle bei und kann mit jedem Textverarbeitungsprogramm leicht an eigene Bedürfnisse angepasst werden.

🚧 Dieses Tool befindet sich noch in der Testphase. Fragen, Anregungen und inhaltliche Hinweise bitte an christian.sievers@hbz-nrw.de 🚧

## Lokales Starten der Applikation

```
cd {Verzeichnis}
python3 -m http.server 8002
```

Im Browser [http://localhost:8002/](http://localhost:8002/) aufrufen.




## Voraussetzungen
- einfacher Webspace
- Wissen, wie man eine Textdatei und/oder eine Tabellenkalkulation öffnet
- kein PHP oder Datenbank benötigt
- kein npm, yarn oder eine andere Paketverwaltung benötigt

## DSGVO
- Keine Datenerhebung auf dem Server (Ausnahme: Je nach Konfiguration Erfassung der Zugriffe durch den Webhosting-Anbieter, z.B. IP-Adresse und Uhrzeit).
- Kein Aufruf von externen Dateien (z.B. Content Delivery Network / CDN, Bootstrap, jQuery). Alle benötigten Komponenten sind eingebettet und lokal verfügbar.
- Keine Cookies.

## Lizenz
- GPL 3
- Analog zum Fragenkatalog der SLUB und dem Mat-O-Wahl (ebenfalls GPL 3). 
- Quellcode, Lizenz und größere Änderungen müssen kenntlich gemacht werden.
- Änderungen, Weitergabe, sowie kommerzielle und private Nutzung erlaubt.
- Keine Garantie für Softwareschäden. 
