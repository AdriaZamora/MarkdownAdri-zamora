## Pregunta 5

### a) Quina opció és més ràpida d'escriure i més fàcil de llegir?

L'**Opció B (Markdown)** és més ràpida d'escriure i més fàcil de llegir en un editor de text pla. Cada tasca ocupa una sola línia i no cal obrir ni tancar etiquetes. L'estat de la tasca es veu d'un cop d'ull amb `[x]` o `[ ]`, i el text és gairebé una llista normal. En canvi, l'Opció A (XML) necessita escriure cada etiqueta dues vegades (obertura i tancament), té molts més caràcters i la informació queda amagada entre etiquetes i atributs, cosa que fa el fitxer més llarg i més pesat de llegir.

### b) Per què un sistema o una base de dades preferiria XML entre servidors?

Perquè XML és un format **estructurat i no ambigu**, pensat perquè les màquines el processin de forma fiable. Alguns motius:

- **Estructura explícita:** cada dada té un nom (`tasca`, `descripcio`, `estat`) i una posició clara dins la jerarquia. Un programa pot llegir "l'estat de la tasca" sense interpretar el text. En Markdown, `[x]` només és una convenció de format i no una dada amb significat propi.
- **Validació:** es pot comprovar que el document és correcte amb un esquema (XSD o DTD), de manera que el servidor receptor sap que les dades tenen el format esperat i rebutja les que no.
- **Estàndard d'intercanvi:** hi ha analitzadors (parsers) i eines per a XML en tots els llenguatges, i serveis com SOAP o fitxers de configuració l'utilitzen.
- **Escalabilitat:** permet representar dades complexes (nivells, atributs, llistes d'objectes) que Markdown no pot expressar bé.

En resum, Markdown està pensat perquè **una persona** llegeixi i escrigui, i XML perquè **dos sistemes** s'entenguin entre ells sense errors d'interpretació.