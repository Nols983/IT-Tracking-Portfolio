# IPv4

Definition: IPv4 steht für Internet Protocol Version 4. Es ist eine der zentralen Technologien des Internets und bildet die logische Adressierungsebene (Layer 3), die Datenpakete von einem Gerät auf ein anderes über verschiedene Netzwerke hinweg transportiert.

Es ist eine 32-Bit Adresse, welche in 4 Oktetten in Dezimalform dargestellt wird.

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
192.168.178.254 -> Broadcast Adresse\
192.168.178.1 - 192.168.178.253 -> gültige Hosts im Netzwerk

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

# IPv6

## Grundlagen

- IPv6 = Internet Protocol Version 6 (Nachfolger von IPv4)

- Adresslänge: 128 Bit → ca. 3,4 × 10³⁸ Adressen (praktisch unerschöpflich)

- Schreibweise: Hexadezimal, in 8 Blöcken à 16 Bit, getrennt durch :
- Beispiel: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

## Adresstypen

- Unicast → eine eindeutige Adresse (ein Gerät)

- Multicast → eine Gruppe von Geräten

- Anycast → mehrere Geräte, aber Antwort vom nächstgelegenen

## Wichtige Bereiche

- Global Unicast: 2000::/3 → weltweit eindeutige Adressen

- Link-Local: fe80::/10 → automatisch vergeben, nur im lokalen Netz

- Unique Local (ULA): fc00::/7 → ähnlich wie private IPv4-Adressen (RFC1918)

## Weitere Merkmale

- Keine NAT mehr notwendig (jeder Host kann eine eindeutige Adresse haben)

- Integrierte IPsec-Unterstützung für Sicherheit

- Autokonfiguration (SLAAC) + DHCPv6 möglich

- Präfix-Länge statt Subnetzmaske → z. B. /64
