# 🧑‍💻 Anfänger Guide – Dein erstes Homelab

## 👋 Was ist ein Homelab?

Ein Homelab ist deine eigene kleine IT-Umgebung zuhause.

👉 Du betreibst selbst:

* Server
* Anwendungen (z. B. Plex, Minecraft, DNS)
* Netzwerke

Ziel ist es:

* zu lernen
* Dinge auszuprobieren
* reale IT-Szenarien zu simulieren

---

## 🤔 Warum überhaupt ein Homelab?

Ein Homelab hilft dir dabei:

* praktische Erfahrung zu sammeln
* Systeme wirklich zu verstehen (nicht nur Theorie)
* Fehler zu machen und daraus zu lernen
* dich auf Jobs im IT-Bereich vorzubereiten

👉 Gerade als Fachinformatiker ist das ein riesiger Vorteil.

---

## 🧱 Was brauchst du für den Einstieg?

### 💻 Hardware (einfach starten!)

Du brauchst kein Rechenzentrum 😄

Möglichkeiten:

* alter PC / Laptop
* Mini-PC (z. B. Fujitsu, Shuttle)
* Raspberry Pi

👉 Wichtig:

* mindestens 8 GB RAM empfohlen
* stabile Internetverbindung

---

### 🐧 Betriebssystem

Ich empfehle: **Ubuntu Server**

Warum?

* leichtgewichtig (kein Desktop)
* stabil
* sehr viele Tutorials online

---

## ⚙️ Schritt 1 – Ubuntu Server installieren

1. ISO herunterladen
2. Bootfähigen USB-Stick erstellen
3. Installation starten
4. SSH aktivieren (wichtig!)

👉 Danach kannst du deinen Server remote verwalten:

```bash
ssh user@server-ip
```

---

## 🐳 Schritt 2 – Docker installieren

Docker ist die Grundlage deines Homelabs.

```bash
sudo apt update
sudo apt install docker.io -y
```

Docker starten und aktivieren:

```bash
sudo systemctl enable docker
sudo systemctl start docker
```

(Optional – ohne sudo arbeiten):

```bash
sudo usermod -aG docker $USER
```

---

## 📦 Schritt 3 – Dein erster Container

Teste Docker mit einem einfachen Beispiel:

```bash
docker run hello-world
```

👉 Wenn das funktioniert: alles richtig eingerichtet ✅

---

## 🧠 Schritt 4 – Docker Compose nutzen

Für mehrere Services brauchst du Docker Compose:

```bash
sudo apt install docker-compose -y
```

Beispiel `docker-compose.yml`:

```yaml
version: "3"

services:
  nginx:
    image: nginx
    ports:
      - "8080:80"
```

Starten:

```bash
docker compose up -d
```

👉 Jetzt läuft dein erster Webserver!

---

## 🌐 Schritt 5 – Erste sinnvolle Services

Hier solltest du anfangen:

### 🔧 Pflicht (Grundlage)

* Portainer → Docker Verwaltung
* Pi-hole → DNS + Adblock

---

### 📊 Monitoring

* Uptime Kuma → Server überwachen

---

### 🧑‍💻 Zugriff

* SSH (Standard)
* optional: Web-Terminal

---

## 🧭 Wie du weitergehst

Wenn das läuft, kannst du dein Homelab erweitern:

* Reverse Proxy (Traefik)
* eigene Domains (DDNS)
* Medienserver (Plex)
* Gameserver (Minecraft)

---

## ⚠️ Typische Anfängerfehler

* ❌ alles auf einmal machen
* ❌ keine Backups
* ❌ keine Dokumentation
* ❌ blind Copy-Paste ohne Verständnis

👉 Nimm dir Zeit und verstehe jeden Schritt.

---

## 🧠 Mein Tipp

Baue dein Homelab Schritt für Schritt:

1. Docker verstehen
2. 1–2 Container betreiben
3. Netzwerk verstehen
4. Monitoring hinzufügen
5. erweitern

👉 Genau so ist auch dieses Projekt entstanden.

---

## 🚀 Nächster Schritt

👉 Schau dir jetzt die anderen Dokumentationen im Homelab-Ordner an:

* Architektur
* Services
* Netzwerk

So kannst du tiefer einsteigen und dein eigenes Setup aufbauen.
