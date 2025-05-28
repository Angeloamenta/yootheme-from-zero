# Filtri Avanzati per Loop Dinamici

### Filtri con Espressioni Regolari (Regex)

Quando crei un loop su elementi dinamici, puoi **escludere specifici elementi** utilizzando espressioni regolari:

**Esempio pratico**:

- **Scenario**: Loop dinamico su post, ma vuoi escludere determinate categorie
- **Soluzione**: Seleziona "regex" come tipo di filtro e applica:
    - `(^(?!Uncategorized|News|ANAC).*)` - Esclude le categorie specificate
    - `((?i)^(?!Uncategorized|News|Anac).*)` - Versione case-insensitive (ignora maiuscole/minuscole)

**Spiegazione del codice**:

- `^` = inizio stringa
- `(?!...)` = negative lookahead (esclude se corrisponde al pattern)
- `.*` = qualsiasi carattere
- `(?i)` = flag per ignorare maiuscole/minuscole
