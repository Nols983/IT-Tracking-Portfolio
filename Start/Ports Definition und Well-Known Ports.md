# Ports:
Ein Port ist ein virtueller Endpunkt im Betriebssystem, über den Netzwerkverbindungen an bestimmte Anwendungen oder Dienste weitergeleitet werden. Ports ermöglichen es, dass mehrere Dienste (z. B. Web, E-Mail) gleichzeitig über dieselbe IP-Adresse kommunizieren können.\
Portnummern reichen von 0-65535.

## Well-Known Ports:

Definition: Well-Known Ports sind von 0-1023. Es handelt sich hierbei um standardisierte Netzwerkdienste, welche von Betriebsystem als Systemdienste verwendet werden können.

Der Zweck dahinter ist eine einfache und einheitliche Kommunikation zwischen Servern und Clients möglich zu machen.

### Standardisierte Ports:
| Port      | Protokoll / Dienst | Kurzbeschreibung                                                                                                    |
| --------- | ------------------ | ------------------------------------------------------------------------------------------------------------------- |
| 20 / 21   | FTP                | Datenübertragung (20) & Steuerung (21) für Dateitransfer                                                            |
| 22        | SSH                | Sicherer Remote-Zugriff & Dateiübertragung                                                                          |
| 23        | Telnet             | Unverschlüsselter Remote-Zugriff (unsicher)                                                                         |
| 25        | SMTP               | Versand von E-Mails                                                                                                 |
| 53        | DNS                | Namensauflösung (Domain → IP)                                                                                       |
| 67 / 68   | DHCP               | IP-Adressen-Zuweisung (Server / Client)                                                                             |
| 80        | HTTP               | Unverschlüsselte Webseitenübertragung                                                                               |
| 110       | POP3               | Abruf von E-Mails vom Server                                                                                        |
| 119       | NNTP               | Usenet Newsserver-Kommunikation                                                                                     |
| 123       | NTP                | Zeitsynchronisation im Netzwerk                                                                                     |
| 143       | IMAP               | E-Mail-Verwaltung direkt auf dem Server                                                                             |
| 161       | SNMP               | Netzwerkverwaltung (Agenten)                                                                                        |
| 194       | IRC                | Internet Relay Chat                                                                                                 |
| 443       | HTTPS              | Verschlüsselte Webseitenübertragung (HTTP over TLS/SSL)                                                             |
