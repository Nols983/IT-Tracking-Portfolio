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

# Basis Netzwerkkomponenten

| **Gerät**   | **Funktion / Beschreibung** |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Hub**     | Ein einfaches Gerät auf OSI-Schicht 1, das Signale an alle angeschlossenen Ports weiterleitet – ohne Auswertung oder Adressierung, also sehr ineffizient im modernen Ethernet‑LAN.                    |
| **Switch**  | Arbeitet auf OSI-Schicht 2 (Data Link). Lernt MAC-Adressen und leitet Frames gezielt nur an den entsprechenden Port weiter – effizienter als Hubs. Layer-3-Switches können auch IP-basiert routen.    |
| **Router**  | Gerät der OSI-Schicht 3 (Network). Verbindet mehrere Netzwerke, trifft Routing-Entscheidungen anhand von IP-Adressen und besitzt oft Funktionen wie NAT, Firewall und sogar VPN.)                     |
| **Gateway** | Hybrid-Gerät, das Protokolle oder Netzwerke unterschiedlicher Art verbindet – z. B. zwischen Ethernet und DSL, oder Netzwerk und Internet. Gateways können auf jeder OSI-Schicht operieren.)          |
