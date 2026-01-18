---
publish: true
created: 2026-01-10T16:11:25.265+01:00
modified: 2026-01-18T12:26:52.901+01:00
cssclasses: ""
---

##### Einleitung
Die Synology Diskstation bieten eine robustes System um Kalender zu speichern.
Dieses lässt sich durch den Admin dort installieren und muss für den jeweiligen Benutzer in den Berechtigungen freigeschaltet werden. Dazu gibt es einschlägige Videos und Anleitungen. Es ist recht trivial.

Das Kalendersystem stellt das sog. Caldav Protokoll zur Verfügung, welche schon viele Jahrzehnte in der IT verwendet wird.

Die Kalender Client Software im App Store, sei es Apple oder Google, hat nun nicht immer diese Funktionalität "eingebaut".

Seiten Synology und vieler Influenzer die sich zu Synology Software äußern ist es am sinnvollsten und am sichersten das Zwischenprodukt CalDAV5x zu verwenden.

Leider ist das im Google App Store mit einem Preis von ca. 6 EUR behaftet.

Ein Gemini Abfrage nach Alternativen ergibt das nahezu identisch Produkt in F-Droid zum Download.
##### Vorab Hinweis
Man sollte unter dem Link https://f-droid.org/de/packages/at.bitfire.davdroid/ auch die APK für F-Droid herunterladen, weiter oben, dann hätte man den Store gleich mit installiert und Updates sind einfacher.
##### Die kostenlose Version von DAVx5 (Legal!)
Viele Nutzer stören sich am Preis im Google Play Store. Da DAVx5 **Open Source** ist, bieten die Entwickler die App über **F-Droid** (einen alternativen App-Store für Open-Source-Software) völlig **kostenlos** an.

- **Vorteil:** Es ist exakt die gleiche App, nur ohne die automatischen Updates über Google.
- **Link:** [DAVx5 auf F-Droid](https://f-droid.org/de/packages/at.bitfire.davdroid/)

Ganz unten in dem link oder über den installierten Store lädt man die APK der **Version 4.5.7-ose** herunter, zur Installation muss man in der Systemsteuerung eine Option freischalten wegen Fremdsoftware. Diese aber dann wieder sperren. Da sich das Protokoll Caldav lange nicht geändert hat und auch nicht ändern wird, sollte das viele Monate, Jahre funktionieren.
##### Konto in CalDAV5x eintragen
Das ist dann auch wieder einfach, man öffnet die Synchronisations-App, trägt die URL, das Synology Konto und das Passwort ein, das war es.

Nach erfolgreicher Verbindung kann man jederzeit im CalDAV5x synchronisieren, muss man aber nicht, es geschieht meist automatisch. Wenn man zusätzlich Kalender erhält, dann ist das "Jetzt synchronisieren" hilfreich. Diese müssen "eingeschaltet" werden.
##### Benutzer freigeben
Man legt an besten eine neuen Kalender an, in dem gemeinsame Daten gespeichert werden, es genügt, wenn das ein Benutzer erledigt.
Dieser wird dann freigeben für einen anderen Synolgy Benutzer mit Lese/Schreib-Rechten, der muss dann eben "jetzt synchronisieren" und den Kalender einschalten in seiner App.

> [!Success] 
> In der Anfangszeit ist gegenseitige Kontrolle angebracht.

##### Kalender Client Software
Mein persönlicher Favorit ist die kostenlose Version von aCalendar aus dem Playstore.
https://play.google.com/store/apps/details?id=org.withouthat.acalendar&pcampaignid=web_share

Die Kalander Software wird direkt aus dem Playstore installiert und sucht sich dann auf dem Smartphone die entsprechenden Konten zusammen, wie z.B. Google.

> [!Tip] 
> Sobald CalDAVx5 installiert und mit dem Synology Konto verbunden ist erscheint das Kalenderkonto in der Kalenderliste der App und ist dort auswählbar. Alle anderen Kalender, die auf dem Smartphone zur Verfügung stehen sind optimaler Weise auszublenden, zu deaktivieren in der Kalender App. Sonst gibt man Termin auf Kalender ein, die nicht synchronisiert werden. Auch ist es hilfreich für genau dieses Konto eine auffällige Farbe zu wählen.