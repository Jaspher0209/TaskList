# Tasklist Requirements

## Functional requirements


### Notes

- Überlege noch, wie du einzelne Task von **To Do's** zu **In Progress** zu **Done** und hin und her wechseln kannst.
- Achte auf HCD Heuristics (Usability) und überprüfe dein Wireframe nach Workflow
    * Im Falle dessen --> Design etwas ändern

### Tasklist requirements

- **Erstelle eine Task**
    * UniqueID (UID) : **int**
    * Name : **string**
    * Typ von Task : **enum**
    * **(optional)** Beschreibung/Details der Task als Textfeld
    * Status : **enum**
    ///////////////////////**OPTIONAL AUFGRUND DESIGN**/////////////////////////
    * Erstellungsdaten (dd/mm/yyyy) : **string** 
    /////////////////////////////////////////////////////////////////////


- **Lese Tasks aus**
    * Bereiche für ausgegebene Tasks
        * Gebe eine ganze Liste von Tasks aus
        * Gebe ein bestimmte Task aus
            * Mittels Suchergebnis
            * Filtern
            * Sortieren
    * Trenne Tasks in momentanen Zustand **(enum)**
        * Todo
        * In Progress
        * Done

- **Lese einzelnen Task aus**
    * Details anzeigen
        * Name : **string**
        * Typ von Task : **enum**
        * **(optional)** Beschreibung/Details der Task als Textfeld
        * Status : **enum**
        
        ///////////////////////**OPTIONAL AUFGRUND DESIGN**/////////////////////////
        * Erstellungsdaten (dd/mm/yyyy) : **string**

- **Lösche eine Task**
    * Durch ein Delete-Button
        * Abfrage ob:
            * Gelöscht werden soll durch Bestätigung
            * Nicht gelöscht werden soll und Vorgang    abbrechen

- **Bearbeite eine Task**
    * Tasknamen ändern
    * Typ der Task ändern
    * **(optional)** Beschreibung/Details
    * Durch ein Button die Änderungen übernehmen
    * sonst Abbrechen

- **Ändere Status von Task**
    * Todo
    * In Progress
    * Done

- **Lösche ein Task in "*Done*"**
    * Mit einem **[Clear All]** - Button sollen die Tasks gelöscht werden
    * **(optional)** Nach 24h soll der Done gelöscht werden (aus der View)
    


