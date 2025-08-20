# Aufbau kurz erklärt:

| Bereich             | Bestandteile                            | Beschreibung                                                                                                                                              |
| ------------------- | --------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Header**          | Ziel-MAC (6 B), Quell-MAC (6 B)         | Adressierung der beteiligten Geräte (§ Data Link Layer)                                                                                                   |
|                     | EtherType / Länge (2 B)                 | Kennzeichnet das nächste Protokoll (z. B. IPv4, ARP) oder Länge des Payloads                                                                              |
|                     | Optional: VLAN-Tag (4 B)                | Für VLAN-Identifikation (IEEE 802.1Q) – eingefügt nach den MAC-Adressen                                                                                   |
| **Payload (Daten)** | Variable Länge (min. 46 B, max. 1500 B) | Enthält die zu übertragenden Nutzdaten, wie z. B. ein IP-Paket. Ist der Payload zu klein, wird er mit Padding aufgefüllt.                                 |
| **Trailer**         | FCS (4 B)                               | Frame Check Sequence – CRC zur Erkennung von Übertragungsfehlern                                                                                          |


