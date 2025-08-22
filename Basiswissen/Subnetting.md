# Subnetting

Definition: Subnetting ist das Aufteilen eines großen IP-Netzwerks in kleinere Teilnetze (Subnets). Dadurch kommunizieren Geräte innerhalb eines Subnets direkt, während die Verbindung zwischen Subnets durch einen Router erfolgt

Gründe für Subnetting:
- Bessere Netzwerkverwaltung & Leistung: Weniger Broadcast-Domänen, weniger Traffic.
- Sicherheitsvorteile: Isolierung von Netzen erlaubt gezielte Zugriffskontrolle.
- Effizientere IP-Nutzung: Subnetting verhindert Verschwendung in großen Adressbereichen.

## 1.) Beispiel (2 Subnetze):

**Aktuelles Netzwerk:**

192.168.1.0 /24

- Das /24 bedeutet: Subnetzmaske 255.255.255.0
- Damit gibt es 256 Adressen (0–255), davon nutzbar 254 Hosts (1–254).



**Schritt 1: Subnetzmaske anpassen**

- Bisher: /24 → 255.255.255.0

- Teilt man in 2 Netze, nimmt man /25 → 255.255.255.128

**Schritt 2: Neue Netze berechnen**

| Subnetz | Netzadresse   | Hostbereich                   | Broadcast     | Anzahl Hosts |
| ------- | ------------- | ----------------------------- | ------------- | ------------ |
| Netz 1  | 192.168.1.0   | 192.168.1.1 – 192.168.1.126   | 192.168.1.127 | 126          |
| Netz 2  | 192.168.1.128 | 192.168.1.129 – 192.168.1.254 | 192.168.1.255 | 126          |

## 2.) Beispiel (4 Subnetze):

**Ausgangsnetz:**

192.168.1.0 /24

**Schritt 1: Subnetzmaske anpassen**

- Aufteilung in 4 Subnetze → neuer Präfix /26 → neue Subnetzmaske 255.255.255.192
- Jedes Subnetz hat 64 Adressen, davon 62 nutzbare Hosts. (2 entfallen wegen Netzwerk- und Broadcastadresse)

**Schritt 2: Neue Netze berechnen**

  | Subnetz | Netzadresse   | Hostbereich                   | Broadcast     | Anzahl Hosts |
| ------- | ------------- | ----------------------------- | ------------- | ------------ |
| Netz 1  | 192.168.1.0   | 192.168.1.1 – 192.168.1.62    | 192.168.1.63  | 62           |
| Netz 2  | 192.168.1.64  | 192.168.1.65 – 192.168.1.126  | 192.168.1.127 | 62           |
| Netz 3  | 192.168.1.128 | 192.168.1.129 – 192.168.1.190 | 192.168.1.191 | 62           |
| Netz 4  | 192.168.1.192 | 192.168.1.193 – 192.168.1.254 | 192.168.1.255 | 62           |

## 3.) Beispiel (4 Subnetze und andere Präfix beim Ausgangsnetzwerk):

**Ausgangsnetz:**

192.168.0.0 /22

**Schritt 1: Subnetzmaske anpassen**

- Aufteilung in 4 Subnetze → neuer Präfix /24 → neue Subnetzmaske 255.255.255.0
- Jedes Subnetz hat 255 Adressen, davon 253 nutzbare Hosts. (2 entfallen wegen Netzwerk- und Broadcastadresse)

**Schritt 2: Neue Netze berechnen**

| Subnetz | Präfix | Netzadresse | Hostbereich                 | Broadcast     | Nutzbare Hosts |
| ------- | ------ | ----------- | --------------------------- | ------------- | -------------- |
| Netz 1  | /24    | 192.168.0.0 | 192.168.0.1 – 192.168.0.254 | 192.168.0.255 | 253            |
| Netz 2  | /24    | 192.168.1.0 | 192.168.1.1 – 192.168.1.254 | 192.168.1.255 | 253            |
| Netz 3  | /24    | 192.168.2.0 | 192.168.2.1 – 192.168.2.254 | 192.168.2.255 | 253            |
| Netz 4  | /24    | 192.168.3.0 | 192.168.3.1 – 192.168.3.254 | 192.168.3.255 | 253            |
