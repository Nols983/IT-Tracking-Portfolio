# RAID Definition

Der Begriff RAID steht für Redundant Array of Independent Disks. Dabei handelt es sich um eine Technik zur virtuellen Zusammenfassung mehrerer physischer Speichermedien (wie HDDs oder SSDs) zu einer logischen Einheit, die eine höhere Ausfallsicherheit und/oder eine bessere Leistung gegenüber einzelnen Laufwerken ermöglicht 


## Wofür wird RAID verwendet?

- Ausfallsicherheit (Redundanz): Einige RAID-Formen speichern Daten mehrfach (z. B. Spiegelung), sodass ein Ausfall einzelner Laufwerke keinen Datenverlust bedeutet 
Wikipedia
.

- Performance-Steigerung: Durch Verteilung der Daten auf mehrere Laufwerke können Zugriffe parallelisiert werden – nützlich etwa bei sequenziellen Transfers 


- Größere logische Volumina: Mehrere Platten ergeben zusammen ein großes Speicherfach, als wären sie eine einzige Einheit 

## RAID Level

| RAID-Level        | Technik                              | Mindestanzahl der Laufwerke | Kapazitätseffizienz | Vorteile                                              | Nachteile                                                  |
| ----------------- | ------------------------------------ | --------------------------- | ------------------- | ----------------------------------------------------- | ---------------------------------------------------------- |
| **RAID 0**        | Striping (Daten verteilen)           | 2                           | 100 %               | Sehr hohe Performance beim Lesen/Schreiben            | Keine Redundanz – schon ein Ausfall führt zum Datenverlust |
| **RAID 1**        | Mirroring (Daten spiegeln)           | 2                           | 50 %                | Sehr hohe Ausfallsicherheit – sofort redundante Kopie | Nur halbe Speicherkapazität                                |
| **RAID 5**        | Striping + verteilte Parität         | 3                           | ca. (n–1)/n         | Gute Mischung aus Performance und Redundanz           | Schreib-Performance niedriger, aufwendige Rebuilds         |
| **RAID 6**        | Striping + doppelte Parität          | 4                           | ca. (n–2)/n         | Kann zwei Plattenverlust gleichzeitig verkraften      | Noch langsamere Schreiboperationen, hoher Rechenaufwand    |
| **RAID 10** (1+0) | Kombination aus Mirroring & Striping | mind. 4 (2x2)               | 50 %                | Sehr hohe Performance + sehr gute Redundanz           | Kostenintensiv (viele Platten nötig)                       |

