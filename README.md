# Prüftoolkonfiguration XGewerbeanzeige

Konfiguration für das von der KoSIT im Auftrag des IT-Planungsrates herausgegebene Prüftool, 
welches die Konformität von XML-Dokumenten gegen Schema und Schematron prüft.

Die Konfiguration beinhaltet Prüfszenarien für:

 * XGewerbeanzeige 1.3
 * XGewerbeanzeige 2.0
 * XGewerbeanzeige 2.1
 * XGewerbeanzeige 2.2 (Entwurf)

Eine detaillierte Beschreibung des Prüftools findet sich [hier](https://github.com/itplr-kosit/validator). 

## Schnellstart

1. Die [Stand-alone Fassung des
Prüftools](https://github.com/itplr-kosit/validator/releases/download/v1.1.0/validationtool-1.1.0.zip)  herunterladen und
auspacken.
2. Die [Prüftool-Konfiguration XGewerbeanzeige](https://github.com/itplr-kosit/validator-configuration-xgewerbeanzeige/releases/download/release-2019-12-16/validator-configuration-xgewerbeanzeige_2019-12-16.zip) herunterladen und auspacken.
3. Mitgelieferte Beispielinstanzen validieren:
```
java -jar validationtool-1.1.0-standalone.jar -s scenarios.xml -o reports -h beispiele/*.xml
```
4. Die Prüfprotokolle liegen nun im XML- und HTML-Format im Verzeichnis reports/.
