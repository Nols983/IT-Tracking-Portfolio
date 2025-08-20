# IPv4

Definition: IPv4 steht für Internet Protocol Version 4. Es ist eine der zentralen Technologien des Internets und bildet die logische Adressierungsebene (Layer 3), die Datenpakete von einem Gerät auf ein anderes über verschiedene Netzwerke hinweg transportiert.

Es ist eine 32-Bit Adresse, welche in 4 Oktetten in Dezimalform dargestellt wird.\
Beispiel: 192.168.128.1 (Dezimalschreibweise) == 11000000.10101000.10000000.00000001 (Binärschreibweise)

## Weiterführende Begriffe:

| Begriff               | Funktion                                                                                            |
| --------------------- | --------------------------------------------------------------------------------------------------- |
| **Subnetzmaske**      | 32-Bit-Maske (z. B. 255.255.255.0) teilt IP in Netzwerk‑ und Hostteil.                              |
| **Netzadresse**       | Erster Wert im Subnetz – identifiziert das Teilnetz.                                                |
| **Broadcast-Adresse** | Letzte Adresse im Subnetz – erreicht alle Geräte im Subnetz.                                        |

Beispiel:\
192.168.178.0 /24 -> Netzwerkadresse\
255.255.255.0 -> Subnetzmaske\
192.168.178.254 -> Broadcast Adresse

## Binärsystem

Die Zahlen werden von links nach rechts kleiner:

10000000 = 128\
01000000 = 64\
00100000 = 32\
00010000 = 16\
00001000 = 8\
00000100 = 4\
00000010 = 2\
00000001 = 1

## Subnetting

Definition: Subnetting ist das Aufteilen eines großen IP-Netzwerks in kleinere Teilnetze (Subnets). Dadurch kommunizieren Geräte innerhalb eines Subnets direkt, während die Verbindung zwischen Subnets durch einen Router erfolgt

Gründe für Subnetting:
- Bessere Netzwerkverwaltung & Leistung: Weniger Broadcast-Domänen, weniger Traffic.
- Sicherheitsvorteile: Isolierung von Netzen erlaubt gezielte Zugriffskontrolle.
- Effizientere IP-Nutzung: Subnetting verhindert Verschwendung in großen Adressbereichen.
