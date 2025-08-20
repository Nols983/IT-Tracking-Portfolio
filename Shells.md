# Shell/Reverse Shell Übersicht:

Netcat:\
Beispiel Befehl:"Nc -lvnp 443" \

l = netcat hört bzw wartet auf verbindung\
v = verbose mode wird benutzt um in Kommandozeile live mitzuverfolgen was passiert\
n = verhindert das DNS anstelle einer IP Adresse verwendet wird\
p= zu verwendender Port\

Normale Ports die für Angriffe genutzt werden können.\
53 - DNS\
80 - HTTP\
8080 - Alternativer HTTP Port (Proxy oder falls 80 andersweitig verwendet wird)\
443 - HTTPS (abgesichertes HTTP)\
139 - NetBIOS über TCP/IP, Windows Dateifreigaben in älteren Netzwerken\
445 - Microsoft-DS (SMB direkt über TCP), Datei - und Druckerfreigaben, Active Directory, etc\
