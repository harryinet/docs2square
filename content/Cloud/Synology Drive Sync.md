---
publish: true
created: 2026-01-10T15:58:28.245+01:00
modified: 2026-01-10T15:58:28.245+01:00
cssclasses: ""
---

> [!missing] 
>  Synology Drive Sync hat einen Nachteil in Linux. Man kann im Synchronisations-Modus <u>nicht</u> die Einstellung wählen **Synchronisation bei Bedarf (On-Demand) aktivieren**. Das steht nur unter Windows zur Verfügung. 
>  Das Gleiche gilt auch für das Pendant **Nextcloud Files** im Nextcloud System.

[Was ist On-Demand-Synchronisierung? - Synology Knowledge Center](https://kb.synology.com/de-de/DSM/tutorial/What_is_On-demand_Sync)

Somit ergibt sich in Linux, dass die ganzen Ordner synchronisiert werden, was sich auf den Speicherplatz der PCs und Notebooks auswirkt. **Auch muss man überlegen ob man das möchte**. Alternativ kann man einen speziellen Ordner für z.B. "Mobile Nutzung" synchronisieren und die restlichen Daten lokal über Shares erreichen, direkt auf dem NAS oder Cloud Storage. 

## Allgemein
Synology Drive ist eine umfassende Cloud-Lösung, die den entscheidenden Vorteil bietet, eine **private Cloud** zu sein. Im Gegensatz zu Diensten wie Dropbox oder Google Drive werden alle deine Dateien auf deinem eigenen Synology NAS gespeichert. Du behältst die volle Kontrolle und Datensouveränität, ohne deine Informationen einem Drittanbieter anvertrauen zu müssen. Das ist der größte Pluspunkt für Datenschutz und Sicherheit.

Synology Drive fungiert als zentrale Schaltzentrale für deine Daten. Über eine Desktop-Anwendung und mobile Apps kannst du Dateien automatisch zwischen deinem NAS und deinen Geräten (PC, Mac, Smartphone) synchronisieren. Dies ermöglicht einen nahtlosen Zugriff auf deine Dokumente, Fotos und Videos von überall aus.

Ein weiterer wesentlicher Vorteil ist die **leistungsstarke Versionierung**. Synology Drive speichert mehrere Versionen deiner Dateien, sodass du jederzeit zu einem früheren Zustand zurückkehren kannst. Dies schützt effektiv vor versehentlichem Löschen, Änderungen oder sogar vor Ransomware-Angriffen.

Darüber hinaus bietet es einfache Kollaborationsfunktionen. Du kannst Dateien und Ordner sicher mit anderen Benutzern teilen, Passwörter für Links festlegen und Berechtigungen individuell verwalten. Synology Drive vereint somit die Benutzerfreundlichkeit einer öffentlichen Cloud mit der Sicherheit und Kontrolle deines eigenen Servers.

> [!important] 
>  Man muss in dem Benutzer in der Synology Systemsteuerung dem Benutzer die Anwendung "Synology Drive" freigeben.
## Videos

##### Kurzanleitung
[Besser als OneDrive & Google Drive? - Eigene Cloud mit Synology Drive einrichten. 2023](https://www.youtube.com/watch?v=kYVEusgK-kk)
##### Ausführliche Anleitung
[Synology Drive: Die ultimative Anleitung (2024)](https://www.youtube.com/watch?v=9ax888Z23dc)

## Alternative
* Das wäre [[Cloud/Nextcloud File Sync]], entweder selbst gehostet, was sehr aufwändig ist, oder bei einem Provider für wenig Geld.