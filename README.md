# Beyondkal Server Manager by PaRaDoX

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
