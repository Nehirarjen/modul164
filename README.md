# modul164

## Tag 1 

### Auftrag 1:
Fassen Sie in Stichworten zusammen

Datenmodellierung - drei Datenmodelle:
1. Konzeptionelles Datenmodell (ERM) - besteht aus Entitäten & Relationen
2. Logisches Datenmodell (ERD) - Abbildung der ERM mit Privat- & Fremdschlüsseln
3. Physisches Datenmodell - erweiterung um produktspezifische Erzeugungsanweisungen

---

# Tag 2 

### Auftrag 2:
Erstellen Sie eine Zusammenfassung der Theorie

Das Problem: Wenn verschiedene Tabellen dieselben Felder nutzen, hast du dieselben Daten mehrfach im System. Das sorgt für Datenmüll (Redundanz) und führt schnell zu Fehlern (Inkonsistenz), weil man Werte an mehreren Stellen aktuell halten müsste.

Die Lösung: Du packst alle identischen Felder in eine einzige, übergeordnete Tabelle (Supertyp / Generalisierung). Die speziellen Felder, die nicht überall reinpassen, kommen in untergeordnete Tabellen (Subtypen / Spezialisierung).

Die Verbindung: Die Untertabellen werden über einen Fremdschlüssel mit der Haupttabelle verknüpft. Das Ganze nennt man "is_a"-Beziehung (Untertyp ist ein Obertyp). In der Programmierung heißt dieses Prinzip Vererbung.

Die Regeln: Beim Koppeln musst du festlegen, ob ein Datensatz zu mehreren Untertabellen gleichzeitig gehören darf (überlappend) oder sich die Rollen strikt ausschließen (disjunkt). Zudem wird bestimmt, ob jeder Eintrag der Haupttabelle zwingend auch in einer Untertabelle auftauchen muss (total) oder nicht (partiell).
