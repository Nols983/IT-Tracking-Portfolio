# RAID

| RAID-Level        | Technik                              | Mindestanzahl der Laufwerke | Kapazitätseffizienz | Vorteile                                              | Nachteile                                                  |
| ----------------- | ------------------------------------ | --------------------------- | ------------------- | ----------------------------------------------------- | ---------------------------------------------------------- |
| **RAID 0**        | Striping (Daten verteilen)           | 2                           | 100 %               | Sehr hohe Performance beim Lesen/Schreiben            | Keine Redundanz – schon ein Ausfall führt zum Datenverlust |
| **RAID 1**        | Mirroring (Daten spiegeln)           | 2                           | 50 %                | Sehr hohe Ausfallsicherheit – sofort redundante Kopie | Nur halbe Speicherkapazität                                |
| **RAID 5**        | Striping + verteilte Parität         | 3                           | ca. (n–1)/n         | Gute Mischung aus Performance und Redundanz           | Schreib-Performance niedriger, aufwendige Rebuilds         |
| **RAID 6**        | Striping + doppelte Parität          | 4                           | ca. (n–2)/n         | Kann zwei Plattenverlust gleichzeitig verkraften      | Noch langsamere Schreiboperationen, hoher Rechenaufwand    |
| **RAID 10** (1+0) | Kombination aus Mirroring & Striping | mind. 4 (2x2)               | 50 %                | Sehr hohe Performance + sehr gute Redundanz           | Kostenintensiv (viele Platten nötig)                       |

