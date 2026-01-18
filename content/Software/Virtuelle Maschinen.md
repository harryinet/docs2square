---
publish: true
created: 2026-01-10T15:58:28.253+01:00
modified: 2026-01-10T15:58:28.253+01:00
cssclasses: ""
---

Um virtuelle Maschinen zu erstellen hat man mehrere Möglichkeiten. Übliche kostenlose Programme sind:

* Hypervisor in Windows Pro
* Oracle Virtual Box
* VM Ware Workstation 

## Hypervisor in Windows Pro
Sofern die Installation in Windows Pro möglich ist, ist das mein Favorit. Die Installation ist dann am dichtesten an der Hardware.
Nach der Installation der wichtigen Programme wechsle ich auf die Bedienung über RPD Remotedesktop von Windows aus, dann erhalte ich eine höhere Auflösung, kann zwei Bildschirme nutzen und Töne werden auch übertragen. Das sind Defizite die es unter Hyper-V Screen Share gibt.

Im Hypervisor Manager kann man zu der VM definieren, dass diese z.B. mit der POC Hardware startet und auch sauber damit heruntergefahren wir. Nach dem Hochfahren des Rechners startet man einfach den vorher eingerichteten RDP Client und man kann darauf arbeiten.

### Installation
Die Aktivierung von Hyper-V in Windows erfordert zwei Hauptschritte: Zuerst müssen Sie die **Virtualisierung in Ihrem BIOS/UEFI** einschalten, dann aktivieren Sie die **Hyper-V-Funktion in Windows** selbst. Beachten Sie, dass Hyper-V in den **Home-Editionen von Windows nicht nativ verfügbar** ist. Sie benötigen eine Windows 10/11 Pro, Enterprise oder Education Version.

#### 1. Virtualisierung im BIOS/UEFI aktivieren

Hyper-V benötigt Hardware-Virtualisierungsunterstützung von Ihrem Prozessor (z. B. Intel VT-x oder AMD-V). Dies muss im BIOS oder UEFI Ihres Computers aktiviert sein.

1. Starten Sie Ihren Computer neu und drücken Sie die entsprechende Taste (oft **F2**, **Entf**, **Esc** oder **F10**), um ins BIOS/UEFI-Setup zu gelangen.
2. Suchen Sie in den Einstellungen nach einem Menüpunkt wie **"Virtualization Technology"** (für Intel) oder **"SVM Mode"** (für AMD).
3. Stellen Sie sicher, dass diese Option auf **"Enabled"** oder **"Aktiviert"** steht.
4. Speichern Sie die Änderungen und verlassen Sie das BIOS/UEFI. Der Computer startet neu.

#### 2. Hyper-V in Windows aktivieren

Sie können Hyper-V über die grafische Benutzeroberfläche oder über die Kommandozeile aktivieren.

##### Methode A: Über die Windows-Features (einfachste Methode)

1. Drücken Sie die **Windows-Taste + R**, geben Sie **`optionalfeatures`** ein und drücken Sie **Enter**.
2. Im Fenster **"Windows-Features aktivieren oder deaktivieren"** suchen Sie nach **"Hyper-V"**.
3. Setzen Sie einen Haken vor **"Hyper-V"**. Dadurch werden automatisch auch die Unterpunkte **"Hyper-V-Plattform"** und **"Hyper-V-Verwaltungstools"** ausgewählt.
4. Klicken Sie auf **"OK"**. Windows installiert nun die notwendigen Komponenten.
5. Starten Sie Ihren Computer neu, wenn Sie dazu aufgefordert werden.

##### Methode B: Über PowerShell (für fortgeschrittene Nutzer)

1. Öffnen Sie **PowerShell als Administrator**. Klicken Sie dazu mit der rechten Maustaste auf das Startmenü und wählen Sie **"Windows PowerShell (Admin)"** oder **"Terminal (Admin)"**.
2. Geben Sie den folgenden Befehl ein und drücken Sie **Enter**:
    PowerShell
    ```
    Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All
    ```
3. Wenn die Installation abgeschlossen ist, werden Sie gefragt, ob Sie den Computer neu starten möchten. Geben Sie **`Y`** für Ja ein und drücken Sie **Enter**.

Nach dem Neustart finden Sie den **"Hyper-V-Manager"** im Startmenü und können mit der Erstellung von virtuellen Maschinen beginnen. Dieses Video demonstriert die Installation und Konfiguration von Hyper-V in Windows 11.
https://www.youtube.com/watch?v=t972GINTjF4

#### RDP unter z.B. Ubuntu
Desktop Sharing and Remote Logging on Ubuntu Server
https://www.youtube.com/watch?v=dRzI3kAjW5E

## Oracle Virtual Box 
Das nutze ich, wenn mir unter Windows, je nach Rechnereinstellung die Installation von Hypervisor nicht möglich ist.

## VM Ware Workstation 
Nutze ich eigentlich nicht mehr, da die anderen Lösungen gut funktionieren.
