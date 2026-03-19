# 🖥️ Hardware

## 📖 Übersicht

Dieses Homelab besteht aus mehreren Geräten, die jeweils eine klare Aufgabe übernehmen.

Ziel ist es, die Last zu verteilen und verschiedene Dienste voneinander zu trennen.

---

## 🍓 Raspberry Pi 5

**Rolle:** Infrastruktur & Core Services

**Technische Daten:**

* CPU: ARM Cortex-A76
* RAM: 8 GB
* Storage: externe SSD

**Einsatzbereiche:**

* DNS-Server (Pi-hole)
* Monitoring (Uptime Kuma)
* zentrale Infrastruktur-Dienste

**Warum dieses Gerät?**

* geringer Stromverbrauch
* ausreichend Leistung für leichte Services
* ideal für dauerhafte Grunddienste

---

## 🖥️ Shuttle PC

**Rolle:** Hauptserver / Gateway

**Technische Daten:**

* CPU: Intel (je nach Modell)
* RAM: 8 GB
* Storage: SSD

**Einsatzbereiche:**

* Docker Host für die meisten Services
* Reverse Proxy (Traefik)
* zentrale Steuerung des Homelabs

**Warum dieses Gerät?**

* mehr Leistung als der Raspberry Pi
* geeignet für mehrere parallel laufende Container
* stabile Grundlage für produktionsähnliche Dienste

---

## 🎮 Fujitsu Mini PC

**Rolle:** Gameserver

**Technische Daten:**

* CPU: Intel i5-10400T
* RAM: 16 GB
* Storage: SSD

**Einsatzbereiche:**

* Minecraft Server
* Factorio Server
* Terraria Server

**Warum dieses Gerät?**

* dedizierte Ressourcen für Gameserver
* verhindert Performance-Probleme auf dem Hauptsystem
* flexibel je nach Spiel nutzbar

---

## 💾 NAS

**Rolle:** Storage

**Technische Daten:**

* Storage: mehrere TB (RAID 1)
* Netzwerk: LAN-Anbindung

**Einsatzbereiche:**

* Medien (Plex)
* Backups
* zentrale Datenablage

**Warum dieses Gerät?**

* große Speicherkapazität
* zentraler Zugriff für mehrere Systeme
* Datensicherheit durch RAID

---

## 🌐 Router (Fritzbox)

**Rolle:** Netzwerkzentrale

**Technische Daten:**

* Standard Heimrouter (IPv4/IPv6)

**Einsatzbereiche:**

* Verbindung zum Internet
* Verwaltung des Heimnetzwerks
* Basis für die Kommunikation aller Geräte

---

## ⚠️ Hinweis

Konkrete IP-Adressen, Domains und sensible Daten wurden aus Sicherheitsgründen nicht dokumentiert.

