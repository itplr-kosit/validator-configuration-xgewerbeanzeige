# Prüftoolkonfiguration XGewerbeanzeige

Konfiguration für das von der KoSIT im Auftrag des IT-Planungsrates herausgegebene Prüftool, 
welches die Konformität von XML-Dokumenten gegen Schema und Schematron prüft.

Die Konfiguration beinhaltet Prüfszenarien für:

 * XGewerbeanzeige 1.3
 * XGewerbeanzeige 2.0 (Stand Handlungsanweisungen 08.01.2020)
 * XGewerbeanzeige 2.1 (Stand Handlungsanweisungen 15.01.2020)
 * XGewerbeanzeige 2.2 (Stand Handlungsanweisungen 26.08.2020)

Eine detaillierte Beschreibung des Prüftools findet sich [hier](https://github.com/itplr-kosit/validator). 

## Schnellstart

1. Die [Stand-alone Fassung des
Prüftools](https://github.com/itplr-kosit/validator/releases/download/v1.1.1/validationtool-1.1.1.zip)  herunterladen und
auspacken.
2. Die [Prüftool-Konfiguration XGewerbeanzeige](https://github.com/itplr-kosit/validator-configuration-xgewerbeanzeige/releases/download/release-2020-08-26/validator-configuration-xgewerbeanzeige_2020-08-26.zip) herunterladen und auspacken.
3. Mitgelieferte Beispielinstanzen validieren:
```
java -jar validationtool-1.1.1-standalone.jar -s scenarios.xml -o reports -h beispiele/*.xml
```
4. Die Prüfprotokolle liegen nun im XML- und HTML-Format im Verzeichnis reports/.
