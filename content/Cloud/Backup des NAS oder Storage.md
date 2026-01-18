---
publish: true
created: 2026-01-10T15:58:28.246+01:00
modified: 2026-01-10T15:58:28.246+01:00
cssclasses: ""
---

## Eigene interne Maßnahmen
In der Regel gilt der gedankliche Ansatz, das NAS ist ja das Backup meines Computers. Man hat ja Maßnahmen ergriffen.

* Redundanz von Hardware, mehrere Festplatten im NAS
* Kopieren auf eine externe Festplatte

Dies sind aber alle räumlich eben in den eigenen Räumen, was eben das Risiko bei einer Katastrophe wie Feuer, Wasser oder sonstige Zerstörung und Verlust birgt.

## Backup in Cloud
Die größten Vorteile sind der Schutz vor Hardware-Ausfällen und die einfache, automatische Wiederherstellung von Daten.
Es gibt viele Anbieter die Speicherplatz in der Cloud anbieten, jedoch falle alle weg, die nicht in Deutschland oder Europa agieren.

> [!caution] 
>  Ein absolutes No-Go sind alle Dienste in US, wie Google, Amazon, Microsoft, ...

## Nochmal Hetzner
Über die Bedienoberfläche der Hetzner Console habe ich die StorageBox mit 1TB gebucht BX11, in diesem Falle Standort **Helsinki**.
[Storage Box: Günstiger Online Speicher und Datenarchivierung](https://www.hetzner.com/de/storage/storage-box/)

Nach dorthin transferiere ich einmal in der Nacht die Daten mit dem **Synolgy Hyperbackup**, wahlweise voll verschlüsselt oder als 1:1 Kopie. [Synology Inc.](https://www.synology.com/de-de/dsm/feature/hyper_backup)

Sollte einmal die Datenmenge kräftig anwachsen, dann bucht man einfach mehr Speicherplatz.

> [!summary] 
>  Hier gilt, rechne wie lange man den monatlichen Betrag zahlen muss um stattdessen ein Hardware NAS zu bezahlen. Dies mit allen Werten wie Strom, Support, Verfügbarkeit.

