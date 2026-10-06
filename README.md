# Beyondkal Server Manager by PaRaDoX

**[🇩🇪 Deutsch](#deutsch) · [🇬🇧 English](#english)**

**⬇️ [Download – neueste Version / latest version](https://github.com/paradox1337s/beyondkal-server-manager/releases/latest)**

---

<a id="deutsch"></a>
# 🇩🇪 Deutsch

**Das Verwaltungs-Tool für Kal-Online-Server (MainSvr, DataSvr, AuthSvr).**
Starten, überwachen und konfigurieren – als Windows-Programm am Server, im Browser oder vom Handy.

## ⬇️ Download

**[Neueste Version herunterladen](https://github.com/paradox1337s/beyondkal-server-manager/releases/latest)** → `BeyondkalManager.exe`

1. `BeyondkalManager.exe` in einen Unterordner deines Serverordners legen, z. B. `Server\BeyondkalServerManager\`
2. Starten – beim ersten Start legst du den Admin-Zugang an, danach erkennt der Manager deine Server selbst

`bkm-cli.exe` ist optional (Kommandozeile für Notfälle, z. B. Passwort zurücksetzen).

> **Windows-SmartScreen:** Da die EXE nicht signiert ist, kann beim ersten Start „Der Computer wurde durch Windows geschützt“ erscheinen → **Weitere Informationen** → **Trotzdem ausführen**.

## Server steuern & überwachen
- **Dashboard** mit allen Servern auf einen Blick: Status, Laufzeit, CPU, RAM, Ports
- **Starten, Stoppen, Neustarten** – einzeln oder alle, in der richtigen Reihenfolge (Abhängigkeiten)
- **Automatischer Neustart** nach Absturz oder Hänger, mit Begrenzung gegen Neustart-Schleifen
- **Ankündigung im Spiel** vor geplanten Neustarts
- **Wartungsmodus** und **Adminbefehle** direkt aus dem Tool
- **Geplanter Neustart** an festen Tagen und Uhrzeiten
- **Absturz- und Hängeberichte**, **Stabilität der letzten 7 Tage**
- Beim Beenden oder Aktualisieren des Managers **laufen die Spielserver weiter**

## Config-Editor
- Alle Config-Dateien (`Config`, `Configs`, Hauptordner) bearbeiten
- **Koreanische (CP949), UTF-8 und gemischte Dateien** werden sicher erkannt und unverändert zurückgeschrieben
- **Prüfung beim Speichern**: doppelte Schlüssel, fehlende Werte, Text außerhalb von Sätzen
- **Vorschau mit Unterschieden** vor jedem Speichern
- **Automatische Sicherung** jeder Änderung, Wiederherstellung mit einem Klick
- **Tägliche Config-Sicherung** und **Komplettsicherung** als ZIP
- **Suche** über alle Configs
- **Schutz bei gleichzeitiger Bearbeitung**: Wurde die Datei inzwischen geändert, kannst du deine Fassung auf die neue anwenden
- Passwörter in Configs (z. B. DB-Zugang) sind **standardmäßig verdeckt**

## Konsole & Logs
- **Live-Konsole** aller Server mit Filter (Server, Stufe, Suchbegriff) und Export
- **Manager-Logs** und Protokoll aller Admin-Aktionen und Anmeldungen

## Benachrichtigungen
- **Discord-Meldungen** bei Absturz, Hänger, Neustart, Start/Stopp und Wartung – einzeln wählbar

## Zugriff von überall – über einen Port
- **Am PC** als Windows-Programm mit eigenem Fenster und Symbol im Infobereich
- **Im Browser** am Server
- **Vom Handy oder über VPS** per HTTPS, am Handy **als App installierbar**
- Eingebaute Schritt-für-Schritt-Anleitung für VPN (z. B. Tailscale), Firewall und Zertifikat
- **API-Tokens** für eigene Apps

## Benutzer & Sicherheit
- Mehrere Benutzer mit Rollen: **Admin** (alles), **Operator** (Server steuern, Adminbefehle, Wartung), **Viewer** (nur lesen)
- Schutz vor Passwort-Raten, Sitzungen mit Ablaufzeit, „Angemeldet bleiben“
- Fernzugriff ist **ab Werk aus**, der Manager öffnet **keine Ports** von selbst
- Kritische Aktionen nur mit **Bestätigung**

## Komfort
- **Automatische Updates**: Der Manager prüft täglich, ob es eine neue Version gibt, und fragt vor dem Download – *Herunterladen & installieren*, *Später* oder *Version überspringen*. Downloads werden per SHA-256 geprüft.
- **Systemcheck** mit Fehlersuche und Hinweisen
- **Serverordner automatisch durchsuchen** – Ports und EXEs werden selbst erkannt
- **Deutsch / Englisch**, helles und dunkles Design
- **Autostart mit Windows**
- Einstellungen exportieren und importieren

## Voraussetzungen
- Windows 10/11 oder Windows Server 2016+ (64 Bit)
- Kein .NET nötig (eigenständige EXE)
- **Microsoft Edge WebView2** für das Programmfenster: unter Windows 10/11 bereits vorhanden. Fehlt es (oft bei Windows Server), fragt der Manager, ob er den offiziellen Microsoft-Installer laden soll. Bei „Nein“ öffnet sich die Oberfläche im Browser – alle Funktionen bleiben gleich.

---

<a id="english"></a>
# 🇬🇧 English

**The management tool for Kal Online servers (MainSvr, DataSvr, AuthSvr).**
Start, monitor and configure your servers – as a Windows program on the server, in the browser or from your phone.

## ⬇️ Download

**[Download the latest version](https://github.com/paradox1337s/beyondkal-server-manager/releases/latest)** → `BeyondkalManager.exe`

1. Put `BeyondkalManager.exe` into a subfolder of your server folder, e.g. `Server\BeyondkalServerManager\`
2. Start it – on first start you create the admin account, then the manager detects your servers on its own

`bkm-cli.exe` is optional (command line for emergencies, e.g. resetting a password).

> **Windows SmartScreen:** The EXE is not signed, so on first start Windows may show “Windows protected your PC” → **More info** → **Run anyway**.

## Control & monitor servers
- **Dashboard** with all servers at a glance: status, uptime, CPU, RAM, ports
- **Start, stop, restart** – individually or all at once, in the right order (dependencies)
- **Automatic restart** after a crash or hang, with a limit against restart loops
- **In-game announcement** before scheduled restarts
- **Maintenance mode** and **admin commands** directly from the tool
- **Scheduled restart** on fixed days and times
- **Crash and hang reports**, **stability of the last 7 days**
- When the manager is closed or updated, **the game servers keep running**

## Config editor
- Edit all config files (`Config`, `Configs`, main folder)
- **Korean (CP949), UTF-8 and mixed files** are detected reliably and written back unchanged
- **Validation on save**: duplicate keys, missing values, text outside of entries
- **Preview of the changes** before every save
- **Automatic backup** of every change, restore with one click
- **Daily config backup** and **full backup** as ZIP
- **Search** across all configs
- **Protection against simultaneous editing**: if the file was changed meanwhile, you can apply your version to the new one
- Passwords in configs (e.g. DB login) are **hidden by default**

## Console & logs
- **Live console** of all servers with filters (server, level, search term) and export
- **Manager logs** and a record of all admin actions and logins

## Notifications
- **Discord messages** on crash, hang, restart, start/stop and maintenance – each one selectable

## Access from anywhere – over one port
- **On the PC** as a Windows program with its own window and a tray icon
- **In the browser** on the server
- **From your phone or via VPS** over HTTPS, **installable as an app** on the phone
- Built-in step-by-step guide for VPN (e.g. Tailscale), firewall and certificate
- **API tokens** for your own apps

## Users & security
- Multiple users with roles: **Admin** (everything), **Operator** (control servers, admin commands, maintenance), **Viewer** (read only)
- Protection against password guessing, sessions with expiry, “stay signed in”
- Remote access is **off by default**, the manager **never opens ports** on its own
- Critical actions only with **confirmation**

## Convenience
- **Automatic updates**: the manager checks daily for a new version and asks before downloading – *Download & install*, *Later* or *Skip this version*. Downloads are verified with SHA-256.
- **System check** with troubleshooting hints
- **Scan the server folder automatically** – ports and EXEs are detected on their own
- **German / English**, light and dark theme
- **Start with Windows**
- Export and import settings

## Requirements
- Windows 10/11 or Windows Server 2016+ (64-bit)
- No .NET needed (self-contained EXE)
- **Microsoft Edge WebView2** for the program window: already included in Windows 10/11. If it is missing (often on Windows Server), the manager offers to download the official Microsoft installer. If you choose “No”, the interface opens in the browser instead – all features stay the same.
