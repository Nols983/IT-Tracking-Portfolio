# Basis Protokolle

| **Protokolle**                                    | **Funktion / Beschreibung**                                                                              |
| ------------------------------------------------ | -------------------------------------------------------------------------------------------------------- |
| **ARP** (Address Resolution Protocol)            | Löst IP-Adressen in MAC-Adressen auf – essenziell für Kommunikation im LAN.                              |
| **RARP** (Reverse ARP)                           | Gerät kennt MAC-Adresse, fragt damit seine IP-Adresse an – heute weitgehend durch DHCP ersetzt.          |
| **ICMP** (Internet Control Message Protocol)     | Unterstützt Fehlermeldungen und Netzwerkdiagnose (z. B. Ping, Traceroute).                               |
| **NTP** (Network Time Protocol)                  | Synchronisiert Systemzeitnetzweit – wichtig für Protokolle, Sicherheit, Logs.                            |
| **IGMP** (Internet Group Management Protocol)    | Verwaltert Multicast-Gruppen, z. B. für IPTV oder Streaming im LAN.                                      |
| **LDAP** (Lightweight Directory Access Protocol) | Zugriff auf Verzeichnisse über das Netzwerk – beispielsweise für Benutzerverwaltung.                     |
| **SCP** (Secure Copy Protocol)                   | Sichere Dateiübertragung über SSH.                                                                       |
| **NAT** (Network Address Translation)            | Erlaubt mehreren Geräten die Nutzung einer einzigen öffentlichen IP-Adresse.                             |
| **IPsec** (Internet Protocol Security)           | Sicherung von IP-Kommunikation durch Verschlüsselung und Authentifizierung, z. B. in VPNs.               |
| **TCP** (Transmission Control Protocol)          | Zuverlässiges, zustandsorientiertes Transportprotokoll mit Port-Nutzung, Fluss- und Fehlerkontrolle.     |
| **UDP** (User Datagram Protocol)                 | Leichtgewichtiges, verbindungsloses Transportprotokoll mit Port-Nutzung – für niedrige Latenz optimiert. |

# CIA

| Begriff             | Bedeutung / Definition                                                                                                                                                                              | Kontext / Zweck                                                                                                                                             |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **CIA**             | Akronym für **Confidentiality (Vertraulichkeit)**, **Integrity (Integrität)** und **Availability (Verfügbarkeit)**.                                                                                 | Grundlage der Informationssicherheit – dient als Modell zur Gestaltung von Schutzmechanismen.                                             |
| **Vertraulichkeit** | Sicherstellung, dass **nur autorisierte Personen Zugang** zu bestimmten Informationen haben.                                                                                                        | Verhindert unberechtigten Zugriff auf sensible Daten.                                                                     |
| **Integrität**      | Gewährleistung der **Richtigkeit, Vollständigkeit und Unverfälschtheit** von Daten im gesamten Lebenszyklus.                                                                                        | Schutz vor ungewollter oder böswilliger Veränderung, Manipulation, Korruption.                 |
| **Verfügbarkeit**   | Daten und Systeme sind **autorisierter Nutzung zugänglich**, wenn diese benötigt werden.                                                                                                            | Schutz gegen Ausfälle, zur Sicherstellung der Betriebsbereitschaft und Systemverfügbarkeit.                               |


