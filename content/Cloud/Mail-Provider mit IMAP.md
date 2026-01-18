---
publish: true
created: 2026-01-10T15:58:28.244+01:00
modified: 2026-01-10T15:58:28.244+01:00
cssclasses: ""
---

## Thema Mail ist etwas hakelig
Der Betrieb eines eigenen Mailservers ist komplex und birgt viele Herausforderungen.

Die größte Schwierigkeit ist die **Zustellbarkeit (Deliverability)**. Große Provider (Gmail, Outlook) stufen neue, unbekannte Server oft als Spam ein. Du musst dich um die korrekte Konfiguration von **SPF**, **DKIM** und **DMARC** kümmern, um die Authentizität deiner E-Mails zu beweisen.

Zusätzlich erfordert die **Sicherheit** ständige Aufmerksamkeit: Du musst den Server gegen Spam-Relaying, Viren und Angriffe härten. Die **Wartung** (Updates, Backups, Blacklist-Überwachung) ist zeitintensiv und erfordert tiefes technisches Know-how. Ein kleiner Fehler kann dazu führen, dass dein gesamter Mailverkehr zum Erliegen kommt.

## Gängige Mail Provider
Aus obigen Gründen bietet es sich an einen zuverlässigen Mailprovider zu nutzen, der dies alles und mehr für einen erledigt. Wenn wir das auf vertrauenswürdige begrenzen, dann sind hier Beispiele, jeder Anbieter wirbt mit unterschiedlichen Vorteilen:

* STRATO
* Mailbox.org
* Posteo
* Tuta
* Proton
* IONOS

Ein Postfach mit 2GB ist heute eher an der Grenze, denn das Mail-Postfach wir heutzutage als auch einfaches Datenlager verwendet.

> [!important] 
>  Immer vor Festlegung die Preise vergleichen, oft ist eine zusätzliche Domaine notwendig. Es erscheinen niedrige Einstiegspreise und dann im Folgejahr wird es schnell das 3-5 fache pro Monat. Ein Postfach mit 25 weiteren Mail-Adressen sind KEINE 25 Postfächer.

* STRATO erwies sich schon jahrelang als zuverlässig und nicht zu teuer, eher günstig, es werden **25 Postfächer** mit je 5GB speicher zu 5€ mtl. geboten. https://www.strato.de/mail/
* TUTA zum Beispiel bietet **ein** Postfach mit 20GB zu 3€ mtl. https://tuta.com/de/pricing

> [!tip] 
>  Eine gute Postfach-Göße die auch etwas auf Zukunft, bzw. hier für die Vergangenheit geeignet ist, ist mindestens 5GB.
## Mail Client Software
#### Outlook
Sofern man Microsoft Outlook für unabdingbar kann man dieses verwenden. Man kann dort auch IMAP und SMTP Mailkonten eintragen. Das funktioniert sogar sehr gut.

#### Thunderbird von Mozilla
Der ewige Mail-Client hat in den Jahren viele Verbesserungen erfahren, läuft auch äußerst stabil. Es gibt sehr viele Erweiterungen für bestimmte Zwecke, die einem das Leben einfacher machen. Allen voran als Beispiel "Quicktext".

In der Grundeinstellung funktioniert schon alles sehr gut. Es ist sinnvoll die einzelnen Einstellungen durchzugehen, zu verstehen und für seine Zwecke anzupassen. Danach kann man sich mit Erweiterungen beschäftigen.

## Übertragen der Mails
Mit Hilfe von Tunderbird und den richtigen Einstellungen im Outlook Web Einstellungen ist es kein Problem sehr schnell alle Mails von Outlook.com zu seinem anderen Mail Provider zu übertragen.

Nach den Einstellungen hier folgend klann man problemlos ganze Ordner von MS Outlook Konto zu anderen IMAP Provider verschieben.
##### MS Outlook
Man muss in der Web-Oberfläche das IMAP erlauben
https://support.microsoft.com/de-de/office/pop-imap-und-smtp-einstellungen-f%C3%BCr-outlook-com-d088b986-291d-42b8-9564-9c414e2aa040

**Aktivieren des POP- oder IMAP-Zugriffs in Outlook.com**
Wenn Sie POP oder IMAP für den Zugriff auf Ihre E-Mails in Outlook.com verwenden möchten, müssen Sie zuerst den Zugriff aktivieren.
1. Wählen Sie **Einstellungen**  > **Mail** > **Weiterleitung und IMAP**
2. Schalten Sie unter **POP und IMAP** den Schieberegler für **Geräte und Apps die Verwendung von POP** erlauben oder **Geräte und Apps die Verwendung von IMAP** erlauben je nach aktiviertem Konto auf **EIN** um.   
3. Wählen Sie **Speichern** aus.

> [!attention] 
>  Hier wirklich NUR das IMAP einschalten, wenn man zusätzlich POP3 einschaltet kann es Probleme geben.

##### Thunderbird anpassen
Man muss im Thunderbird eine kleine Einstellung vornehmen.

1. Links unten Zahnrad zu Einstellungen
2. Ganz mach unten scrollen bis als letztes der Button "Konfiguration Bearbeiten" erscheint
3. Klicken
4. In der Suchleiste "ipv6" eingeben
5. das Flag "network.dns.disableIPv6" auf "true" klicken

Einstellungen schließen, dann sollte das MS Outlook Konto sauber im Thunderbird erscheinen

## Mails aus der Cloud raus
Nun kommt man ja nicht um einen Dienstleister herum, zumindest nicht ohne sehr hohen administrativen Aufwand. Man kann sich allerdings das Ziel setzen, möglichst wenig Mails bei dem Provider in einer Art Datengrab schlummern zu lassen. Sollte es doch einmal eine fremden Zugriff geben dann wäre nicht viel zu sehen.

Siehe hier zu [[Cloud/Synology MailPlus Server und Client mit Apps]]

#### Wieder bietet sich hier das Synolgy NAS an
Damit ist man in der Lage per POP3 sämtliche Mails in seinen eigenen Speicher zu ziehen, sofort.
Weiter kann man über das Synolgy NAS Mails unter Verwendung des Providers versenden.
Die normale Bedienung geschieht über Web-Browser von überall her, auch gesichert mit 2FA.
Das ganze geht auch mobil.

**Lediglich zwei Einschränkungen**
* Die Mails werden in einem Zeitrythmus per POP3 abgeholt, also alle 3-7 Minuten oder länger, so wie man es einstellt.
* Der mobile spezielle Mail-Client ist optisch nicht so berauschend, aber man kann alles machen.

