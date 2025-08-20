# Ports:
Ein Port ist ein virtueller Endpunkt im Betriebssystem, über den Netzwerkverbindungen an bestimmte Anwendungen oder Dienste weitergeleitet werden. Ports ermöglichen es, dass mehrere Dienste (z. B. Web, E-Mail) gleichzeitig über dieselbe IP-Adresse kommunizieren können.\
Portnummern reichen von 0-65535.

## Well-Known Ports:

Definition: Well-Known Ports sind von 0-1023. Es handelt sich hierbei um standardisierte Netzwerkdienste, welche von Betriebsystem als Systemdienste verwendet werden können.

Der Zweck dahinter ist eine einfache und einheitliche Kommunikation zwischen Servern und Clients möglich zu machen.

## Standardisierte Ports:
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

| Port    | Protokoll / Dienst | Name ausgeschrieben                 | Kurze Beschreibung                                                                                                         |
| ------- | ------------------ | ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| 20 / 21 | FTP                | File Transfer Protocol              | Überträgt Dateien zwischen Client und Server über separate Steuer- und Datenverbindungen ([Wikipedia][1])                  |
| 22      | SSH                | Secure Shell                        | Bietet gesicherten Remote-Zugriff und Dateiübertragung über verschlüsselte Verbindung ([Wikipedia][2], [Cloudflare][3])    |
| 23      | Telnet             | Teletype Network (Telnet)           | Ermöglicht unverschlüsselten Remote-Zugriff – gilt als unsicher                                                            |
| 25      | SMTP               | Simple Mail Transfer Protocol       | Standardprotokoll für den Versand von E-Mails über das Internet ([Wikipedia][4], [Amazon Web Services, Inc.][5])           |
| 53      | DNS                | Domain Name System                  | Übersetzt Domain-Namen in IP-Adressen, fungiert so als Internet-Adressbuch ([Wikipedia][6], [Fortinet][7])                 |
| 67 / 68 | DHCP               | Dynamic Host Configuration Protocol | Weist Geräten automatisch IP-Adressen und Netzwerk-Konfigurationsdaten zu ([Wikipedia][8], [Fortinet][9])                  |
| 80      | HTTP               | Hypertext Transfer Protocol         | Grundlage der Datenübertragung im Web via Browser und Server ([Wikipedia][10], [cloudns.net][11])                          |
| 110     | POP3               | Post Office Protocol version 3      | Protokoll zum Abrufen von E-Mails vom Server – oft herunterladen und löschen lokal ([TechTarget][12], [GeeksforGeeks][13]) |
| 119     | NNTP               | Network News Transfer Protocol      | Dient dem Lesen und Veröffentlichen in Usenet-Diskussionsgruppen                                                           |
| 123     | NTP                | Network Time Protocol               | Synchronisiert Netzwerkuhren für genaue Zeitangaben ([Wikipedia][14], [GeeksforGeeks][15])                                 |
| 143     | IMAP               | Internet Message Access Protocol    | Ermöglicht E-Mail-Verwaltung direkt auf dem Server (z. B. Synchronisation über mehrere Geräte)                             |
| 161     | SNMP               | Simple Network Management Protocol  | Netzwerkmanagement-Protokoll zur Abfrage von Geräten (Monitoring); Agenten liefern Daten                                   |
| 194     | IRC                | Internet Relay Chat                 | Protocol für Echtzeit-Textkommunikation über Channels oder private Nachrichten                                             |
| 443     | HTTPS              | Hypertext Transfer Protocol Secure  | Sicher verschlüsselte HTTP-Verbindungen via TLS/SSL zum Schutz der übertragenen Daten                                      |
