# 🏠 Homelab

## 📖 Übersicht

Dieses Homelab bildet eine kleine, produktionsähnliche IT-Infrastruktur ab.

Ziel ist es, reale Szenarien aus der Systemadministration und Netzwerktechnik umzusetzen und zu verstehen.

---

## 🧱 Aufbau

Das Homelab besteht aus mehreren Systemen:

* Raspberry Pi → Core Services (DNS, Monitoring)
* Shuttle Server → Gateway + Hauptservices
* Fujitsu Server → Gameserver

---

## ⚙️ Technologien

* Docker & Docker Compose
* Traefik (Reverse Proxy + TCP Routing)
* Pi-hole (DNS)
* Uptime Kuma (Monitoring)
* Tailscale (Remote Access)

---

## 🧭 Navigation

### 🔰 Einstieg

* `01-Getting-Started/` → Grundlagen & Einführung

### 🧱 Architektur

* `02-Architecture/` → Aufbau & Netzwerkstruktur

### ⚙️ Services

* `03-Services/` → Alle laufenden Dienste

### 🐳 Docker

* `04-Docker/` → Compose Dateien & Setup

### 🌐 Netzwerk

* `05-Network/` → DNS, Traefik, DDNS

### 🔐 Security

* `06-Security/` → Absicherung des Systems

### 🔄 Betrieb

* `07-Operations/` → Monitoring, Backups, Wartung

---

## 🎯 Ziel

Dieses Homelab dient als:

* Lernumgebung
* Testsystem
* Dokumentation meiner IT-Kenntnisse

und wird kontinuierlich erweitert.

Hinweis: Sensible Daten wie IP-Adressen, Domains und API-Keys wurden bewusst anonymisiert.
