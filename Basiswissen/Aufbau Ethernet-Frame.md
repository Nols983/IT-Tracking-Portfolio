# Aufbau kurz erklärt:

| Bereich             | Bestandteile                            | Beschreibung                                                                                                                                              |
| ------------------- | --------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Header**          | Ziel-MAC (6 B), Quell-MAC (6 B)         | Adressierung der beteiligten Geräte (§ Data Link Layer)                                                                                                   |
|                     | EtherType / Länge (2 B)                 | Kennzeichnet das nächste Protokoll (z. B. IPv4, ARP) oder Länge des Payloads                                                                              |
|                     | Optional: VLAN-Tag (4 B)                | Für VLAN-Identifikation (IEEE 802.1Q) – eingefügt nach den MAC-Adressen                                                                                   |
| **Payload (Daten)** | Variable Länge (min. 46 B, max. 1500 B) | Enthält die zu übertragenden Nutzdaten, wie z. B. ein IP-Paket. Ist der Payload zu klein, wird er mit Padding aufgefüllt.                                 |
| **Trailer**         | FCS (4 B)                               | Frame Check Sequence – CRC zur Erkennung von Übertragungsfehlern                                                                                          |


## Erklärung Padding:

Padding (Füllbytes) sorgt dafür, dass ein Ethernet-Frame mindestens die definierte Mindestlänge (64 Byte Gesamt, inkl. Header und Trailer) erreicht—wichtig für Kollisionserkennung und korrekte Übertragung durch die Hardware.

Besteht die Payload aus weniger als 46 Byte (ohne VLAN), füllt die Netzwerkkarte mit Nullen (0x00) auf.

Dadurch wird sichergestellt, dass Frame-Länge und Timing-Anforderungen eingehalten werden.
