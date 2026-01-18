---
publish: true
created: 2026-01-10T15:58:28.243+01:00
modified: 2026-01-10T15:58:28.243+01:00
cssclasses: ""
---


> [!caution] 
> Der Betrieb eines eigenen Mailservers ist technisch anspruchsvoll und bringt zahlreiche Schwierigkeiten mit sich. 

Die größte Herausforderung ist die **Zustellbarkeit** deiner E-Mails. Viele große E-Mail-Provider wie Google oder Microsoft betrachten E-Mails von unbekannten Servern oft als Spam. Du musst deine Server-IP-Adresse sauber halten und komplexe DNS-Einträge (wie SPF, DKIM, DMARC) perfekt konfigurieren, um Vertrauen bei den Empfängern aufzubauen. Ein weiterer Punkt ist die **Sicherheit**. Dein Server ist ein attraktives Ziel für Hacker und Angriffe. Er muss kontinuierlich mit den neuesten Sicherheitspatches und einer robusten Firewall geschützt werden, um Datenlecks und Missbrauch zu verhindern. Hinzu kommen hohe Anforderungen an die **Verfügbarkeit** und das **Wartungsmanagement**. Der Server muss rund um die Uhr laufen und erfordert regelmäßige Überwachung und Fehlerbehebung. Dies macht den Betrieb für Laien sehr schwierig und zeitaufwendig.

Auch kosten Mail-Postfächer mit viel Speicher bei den Provider monatlich ab 3 EUR aufwärts.
### Standard Postfach
Bei vielen Providern gibt es preisgünstige Postfächer mit allerdings wenig Speicher.
### Warum eigenen Mail Speicher verwenden
Früher war es so, dass Mails in der Mail App direkt auf dem eigenen Computer gespeichert wurden, man hatte ja nur einen PC, keine Mobil Geräte. Im laufe der Zeit setzte sich das IMAP Protokoll durch. Damit kann man Mails von jedem Gerät abrufen und lässt diese zentral auf dem Speicher des Mail-Providers.
### Alternative Konzepte
Um den ganz oben technischen Herausforderungen aus dem Weg zu gehen bietet es sich an diese Mails auf einem eigenen Server zu speichern aber dennoch den SPAM Filter und das SMTP-Relay des Providers zu nutzen, die bei relativ niedrigen Preisen.

Sämtliche Mails werden in den verhältnismäßig großen Speicher des eigen Mailservers eingelesen.
## Konzept
Verwenden des Synology MailServer Plus und zugehörige WebBrowser-Mail und mobile Mail Clients.
##### Vorteile
- Keine zusätzliche Portfreigaben durch den Router
- Gekapselte mobile App
- Überall zu bearbeiten per WebBrowser
##### Nachteile
Leicht zeitversetzter Empfang der Mails, je nach eingestellter Abrufrate.
Die Android Mail-Client App ist recht einfach gehalten.
### Umsetzung
Es sind relativ einfache Schritte in der Synology schnell erledigt.
1. MailPlus Server Installieren.
2. MailPlus installieren, Client Zugriff Software.
3. In der Synology Systemsteuerung bei den Benutzern den Zugriff auf Anwendung "Synology MailPlus", der Clientsoftware, aktivieren.
4. Dort ebenfalls unter Dienst im Reiter "MailPlus Client" den Haken setzen bei "Erlauben Mails von externen POP3-Servern zu empfangen".
5. Im Programm "Synology MailPlus Server" die Konten aktivieren, die diesen nutzen sollen.
6. In der Systemsteuerung im Anmeldeportal das "Synology MailPlus" konfigurieren, die Einträge können wie vorgeschlagen vorgenommen werden.
7. Als Benutzer anmelden mit der bekannten URL und den Mail Client starten
8. Rechts oben unter Name->Einstellungen das SMTP und POP3 Postfach konfigurieren, einstellen, dass Original-Kopien im POP3 Postfach gelöscht werden..

Nun kann man über den WebBrowser oder die originale mobile Synology MailPlus App aus dem Store Mails empfangen und versenden. Für den Versand wird der Server des Providers als SMTP-Relay genutzt, spezifisch für das Postfach.

##### Video
Dies Video zeigt etwas holperig die Einrichtung, das Ergebnis zählt.
Die benannte Ports ab 09:58 werden nicht benötigt, einfach bei 12:20 starten.

![MailPlus Server](https://www.youtube.com/watch?v=PJ4gWZAgndM&t=2339s)