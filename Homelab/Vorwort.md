# Homelab Übersicht

## Vorwort

Herzlich Willkommen zu meinem Homelab.

Dieses Projekt dient dazu, eine eigene IT-Infrastruktur im kleinen Maßstab aufzubauen, zu verstehen und kontinuierlich zu verbessern. Ziel ist es, reale Szenarien aus der Praxis (z. B. Serverbetrieb, Monitoring, Netzwerkstruktur) nachzubilden.

Gleichzeitig soll diese Dokumentation auch Einsteigern helfen, die ersten Schritte in Richtung Homelab und Self-Hosting zu gehen.

---

## Ziel dieses Homelabs

* Aufbau einer stabilen, containerbasierten Infrastruktur
* Verständnis von Netzwerken, DNS und Reverse Proxys
* Monitoring und Absicherung von Diensten
* Bereitstellung eigener Services (z. B. Gameserver, Medienserver)

---

## Warum Ubuntu Server + Docker?

### Ubuntu Server

Ich nutze Ubuntu Server 24.04, da:

* weit verbreitet in der Praxis
* stabil und zuverlässig
* große Community + viele Anleitungen
* geringer Ressourcenverbrauch (kein GUI)

--> Perfekt für Server und Homelab-Umgebungen

---

### Docker

Docker ermöglicht es, Anwendungen in Containern laufen zu lassen.

Vorteile:

* einfache Installation von Services
* saubere Trennung der Anwendungen
* schnelle Updates und Deployments
* ideal für Multi-Service-Umgebungen

--> Dadurch kann ich viele Dienste parallel betreiben, ohne das System zu „zumüllen“.

---

## Meine aktuellen Services

Hier eine Übersicht der aktuell eingesetzten Container:

### Infrastruktur

* **Portainer** → Verwaltung aller Docker-Container
* **Traefik** → Reverse Proxy für Routing und Zugriff
* **Pi-hole** → DNS-Server mit Werbeblocker

---

### Monitoring

* **Uptime Kuma** → Überwachung der Erreichbarkeit
* **ntfy** → Benachrichtigungen bei Ausfällen
* **Netdata** → Performance Monitoring der Systeme

---

### Zugriff & Verwaltung

* **Termix** → SSH/SFTP Zugriff im Browser
* **UpSnap** → Wake-on-LAN & Gerätesteuerung

---

### Services

* **Plex** → Medienserver für Filme & Serien
* **Dashy** → Dashboard für schnellen Zugriff

---

### Gaming

* **Minecraft Server**
* **Factorio Server**
* **Terraria Server**

---

### Kommunikation

* **TeamSpeak 3 Server**

  * AFK Bot
  * Memewall Bot

---

### Automatisierung

* **Watchtower** → automatische Container Updates

---

## Zukunftspläne

* Aufbau einer Backup-Strategie
* Verbesserung der Netzwerkstruktur
* Erweiterung der Monitoring-Lösungen
* Remote-Gaming über Server

---

## Für Einsteiger

Falls du neu in diesem Bereich bist, empfehle ich:

1. Grundlagen zu Linux verstehen
2. Docker Basics lernen
3. Erste eigene Container starten

--> Danach kannst du Schritt für Schritt dein eigenes Homelab aufbauen.
