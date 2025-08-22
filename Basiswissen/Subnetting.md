# Subnetting

Definition: Subnetting ist das Aufteilen eines großen IP-Netzwerks in kleinere Teilnetze (Subnets). Dadurch kommunizieren Geräte innerhalb eines Subnets direkt, während die Verbindung zwischen Subnets durch einen Router erfolgt

Gründe für Subnetting:
- Bessere Netzwerkverwaltung & Leistung: Weniger Broadcast-Domänen, weniger Traffic.
- Sicherheitsvorteile: Isolierung von Netzen erlaubt gezielte Zugriffskontrolle.
- Effizientere IP-Nutzung: Subnetting verhindert Verschwendung in großen Adressbereichen.

## Beispiel für ein IPv4 Subnetz:

Aktuelles Netzwerk:
192.168.1.0 /24

- Das /24 bedeutet: Subnetzmaske 255.255.255.0
- Damit gibt es 256 Adressen (0–255), davon nutzbar 254 Hosts (1–254).



Schritt 1: Subnetzmaske anpassen

Bisher: /24 → 255.255.255.0

Teilt man in 2 Netze, nimmt man /25 → 255.255.255.128

Schritt 2: Neue Netze berechnen

Netz 1: 192.168.1.0 – 192.168.1.127

Netzadresse: 192.168.1.0

Broadcast: 192.168.1.127

Host-Bereich: 192.168.1.1 – 192.168.1.126 (126 Hosts)

Netz 2: 192.168.1.128 – 192.168.1.255

Netzadresse: 192.168.1.128

Broadcast: 192.168.1.255

Host-Bereich: 192.168.1.129 – 192.168.1.254 (126 Hosts)
