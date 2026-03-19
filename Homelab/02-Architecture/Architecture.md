# 🧱 Architektur

## 🌐 Netzwerkübersicht

![Homelab Netzwerk](../images/network-overview.png)

---

## 🖥️ Systeme im Überblick

Das Homelab besteht aus mehreren Geräten mit klaren Aufgaben:

### 🍓 Raspberry Pi 5

* DNS (Pi-hole)
* Monitoring (Uptime Kuma)
* zentrale Infrastruktur-Services

---

### 🖥️ Shuttle PC

* zentrale Docker-Instanz
* Reverse Proxy (Traefik)
* Hosting der meisten Services

---

### 🎮 Fujitsu Mini PC

* Gameserver (Minecraft, Factorio, Terraria)
* getrennt vom restlichen System für bessere Performance

---

### 💾 NAS

* Speicherung von Medien (Plex)
* Backups und Datenablage

---

### 🌐 Router (Fritzbox)

* zentrale Netzwerkverbindung
* Verbindung zum Internet
* Weiterleitung von Traffic ins Homelab

---

## 🔁 Zusammenspiel der Systeme

* Alle Geräte befinden sich im gleichen lokalen Netzwerk
* DNS-Anfragen laufen über den Raspberry Pi (Pi-hole)
* Externer Traffic wird über den Router an den Shuttle weitergeleitet
* Traefik übernimmt das Routing zu den jeweiligen Services
* Der Fujitsu Server wird für Gameserver genutzt und separat angebunden

---

## 🎯 Ziel der Architektur

* klare Trennung der Aufgaben
* einfache Erweiterbarkeit
* zentrale Verwaltung über Docker
* möglichst realitätsnahe Infrastruktur

