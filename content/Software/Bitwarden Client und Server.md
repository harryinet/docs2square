---
publish: true
created: 2026-01-10T15:58:28.251+01:00
modified: 2026-01-10T15:58:28.252+01:00
cssclasses: ""
---

## Schnelleinstieg
* Konto im Vaultwarden Server anlegen wie hier weiter unten beschrieben [[Software/Bitwarden Client und Server#Konto im Vaultwarden anlegen]]
* Bitwarden Client einrichten [[Software/Bitwarden Client und Server#Einrichtung im Browser und Smartphone]]

> [!danger] 
> Die Daten liegen verschlüsselt durch euer Masterpasswort auf dem Server und sind für niemanden einzusehen bzw. wieder herzustellen.

Ein Backup ist nicht nötig, da alle Passworte synchronisiert auf allen Geräten zur Verfügung stehen, ggf. Mobile App und Desktop App. Auch können Passwort bei den jeweiligen Diensten oder Webpages neu generiert werden.
##### Links
* [Installieren und synchronisieren Sie alle Ihre Geräte | Bitwarden](https://bitwarden.com/de-de/download/)
##### Video
* Sehr umfangreich, ich bin damals ohne dem gestartet, einfach learning-by-doing, auch ist es schon 2 Jahre alt, die Apps sind aktueller und ansprechender gestaltet.
* [Bitwarden Tutorial | The Full Beginners Guide](https://www.youtube.com/watch?v=OkYKb0Sx-XA)
## Bitwarden Client
Der Bitwarden-Client bietet eine Vielzahl von Vorteilen, die ihn zu einer herausragenden Wahl für die **Verwaltung von Passwörtern** machen. Hier sind die wichtigsten Vorzüge, die den Client so nützlich und sicher gestalten:

#### Einrichtung im Browser und Smartphone
Die Einrichtung nach der Installation in Mobile App, Desktop App und in Browser Erweiterung ist nahezu identisch. Vorher das Konto im Vaultwarden Server anlegen wie hier weiter unten beschrieben [[Software/Bitwarden Client und Server#Konto im Vaultwarden anlegen]]

* Eigenen Server eintragen statt Bitwarden.com
* Mailadresse 
* Sehr sicheres Masterpasswort verwenden
* in den Einstellungen 
	* Mobile App: Biometrie aktivieren
	* Browser Erweiterung: 6-8 stellige PIN eintragen 
	  und **nicht** bei jedem Anmelden das Masterpasswort verlangen, Haken raus

> [!question] 
> Bei Fragen meldet euch einfach. 

#### Funktionalität und Benutzerfreundlichkeit ✨
Neben Sicherheit bietet der Client leistungsstarke Funktionen, die deinen digitalen Alltag erleichtern. Die automatische Vervollständigung von Anmeldedaten in Browsern und Apps spart Zeit und verhindert Tippfehler. Mit dem integrierten Passwort-Generator kannst du schnell starke, einzigartige Passwörter für jeden Dienst erstellen. Die Organisationsfunktionen ermöglichen es dir, Anmeldedaten in Ordnern zu kategorisieren und Favoriten festzulegen. Ein weiterer Pluspunkt ist die Möglichkeit, verschiedene Arten von sensiblen Informationen wie Kreditkartendaten oder sichere Notizen zu speichern. Der Client ist zudem schlank und ressourcenschonend, was eine schnelle und reibungslose Nutzung gewährleistet. Auch die Freigabe von Anmeldedaten mit Familienmitgliedern oder Teamkollegen ist über Organisationen möglich.

#### Sicherheit und Vertraulichkeit 🔒
Der größte Vorteil von Bitwarden ist das hohe Maß an Sicherheit. Alle deine Passwörter werden auf deinen Geräten mit einer starken, Ende-zu-Ende-Verschlüsselung gesichert, bevor sie zu den Servern übertragen werden. Nur du kannst deine Daten entschlüsseln. Die Open-Source-Natur von Bitwarden bedeutet, dass der Code öffentlich einsehbar ist. Das ermöglicht unabhängigen Experten, den Code kontinuierlich auf Schwachstellen zu überprüfen, was das Vertrauen in die Plattform stärkt. Regelmäßige Sicherheitsaudits durch Dritte bestätigen diese Transparenz und Robustheit.

#### Plattformübergreifende Verfügbarkeit 💻📱
Bitwarden glänzt durch seine breite Kompatibilität. Egal, ob du einen Windows-PC, einen Mac, ein Linux-System, ein Android-Smartphone oder ein iPhone nutzt – der Bitwarden-Client ist als Desktop-Anwendung, Browser-Erweiterung und mobile App verfügbar. Diese nahtlose Integration ermöglicht es dir, jederzeit und überall auf deine Passwörter zuzugreifen. Die Synchronisierung deiner Daten zwischen allen Geräten erfolgt automatisch und sicher, sodass deine Informationen stets auf dem neuesten Stand sind.

#### Kostenlose und flexible Nutzung 💰
Ein erheblicher Vorteil von Bitwarden ist das attraktive Preismodell. Die grundlegende Version mit allen wesentlichen Funktionen ist **kostenlos** nutzbar. Für fortgeschrittene Features wie erweiterte Authentifizierungsmethoden oder Dateianhänge gibt es ein preiswertes Premium-Abonnement. Die Möglichkeit, einen eigenen Server (Self-Hosting) zu betreiben, gibt Nutzern, die maximale Kontrolle über ihre Daten wünschen, die vollständige Souveränität.

## Vaultwarden Server - hier als Bitwarden Server
Vaultwarden ist eine inoffizielle, quelloffene und schlanke Alternative zum offiziellen Bitwarden-Server. Während Bitwarden als Client (Browser-Erweiterung, App) genutzt wird, stellt Vaultwarden die Server-Komponente bereit, auf der deine verschlüsselten Daten gespeichert werden. Der größte Vorteil von Vaultwarden liegt in der Möglichkeit des **Self-Hostings**.

#### Konto im Vaultwarden anlegen
Mit der bekannten URL und deiner Mailadresse ein Konto eröffnen.
* Die URL kann bei mir erfragt werden.
* Den Anweisungen in der Mail folgen.
* Im Web-Interface auch die 2FA aktivieren
* Eine gute 2FA App ist Proton Authenticator, es ist nicht verkehrt die auf dem Smartphone zu haben. Man muss dazu kein Konto anlegen, einfach auf Smartphone installieren. [Proton Authenticator: Private, secure 2FA authenticator | Proton](https://proton.me/authenticator)

> [!attention] 
>  Allerdings werden in Zukunft die 2FA TOTP-Strings direkt in der Bitwarden App bei dem jeweiligen Konto hinterlegt bzw. eingescannt. So kann man die 6-stellige  Zahl nach dem Anmelden direkt per PASTE (CTRL+V) in das Feld bei der Anmeldung einfügen, wenn gefordert.

#### Video zur Einrichtung
Es gibt mehrere Videos, dieses hat es ganz gut beschrieben
[Vaultwarden Server (Bitwarden): Kostenloser Passwortmanager auf Synology installieren | Full Guide](https://www.youtube.com/watch?v=vLt5EOOIX7s)
#### Vorteile des Self-Hostings 🌍
Der Hauptnutzen von Vaultwarden ist die absolute Kontrolle über deine Daten. Anstatt deine sensiblen Passwort-Tresore in der Cloud eines Unternehmens zu speichern, hostest du sie auf deinem eigenen Server, zum Beispiel auf einem **Raspberry Pi** oder einem **Synology NAS**. Dies eliminiert die Abhängigkeit von einem Drittanbieter und gibt dir die vollständige Datensouveränität. Deine Passwörter bleiben in deiner privaten Infrastruktur, was den **Datenschutz** auf ein Maximum hebt.

#### Ressourcenschonung und Leistung ✨
Vaultwarden ist extrem **ressourcenschonend**. Die Software ist in der Programmiersprache Rust geschrieben, was sie besonders effizient und schnell macht. Sie benötigt nur minimale Rechenleistung und wenig Arbeitsspeicher. Diese Eigenschaft macht Vaultwarden zur idealen Lösung für schwächere Geräte wie Einplatinencomputer (z. B. Raspberry Pi), die 24/7 laufen sollen, ohne dabei viel Strom zu verbrauchen.

#### Kosten und Kompatibilität 💰
Ein weiterer großer Vorteil ist der **kostenfreie Zugang zu Premium-Funktionen**. Vaultwarden erlaubt es, die meisten Premium-Features der offiziellen Bitwarden-Clients (wie Zwei-Faktor-Authentifizierung oder erweiterte Organisationsmöglichkeiten) zu nutzen, ohne für ein Bitwarden Premium-Abo bezahlen zu müssen. Vaultwarden ist zudem vollständig mit allen offiziellen Bitwarden-Clients kompatibel. Das bedeutet, du kannst die bekannten und vertrauten Desktop-, Browser- und Mobil-Clients weiterhin verwenden und dich einfach mit deiner selbstgehosteten Vaultwarden-Instanz verbinden.

Zusammengefasst bietet Vaultwarden die perfekte Balance aus Sicherheit, Kontrolle, Kostenersparnis und Benutzerfreundlichkeit für alle, die Wert auf die Hoheit über ihre eigenen Daten legen.