Campi del form di iscrizione su sezione scura, anche sopra una foto: testo, select, radio e checkbox. Il campo è un bordino beige su un fondo bianco trasparente.

**Cosa fornisce chi lo usa:** etichette e placeholder in italiano, e una sezione scura (`umber` o `navy`) o una foto scurita come fondo.

- Campo di testo: bordo 1px `field-border` (`sand`), fondo `field-bg` (bianco al 19%), `radius-field` (4px), padding `space-10`, testo `field-text` a 18px.
- Select: stesso bordo e raggio, ma fondo `field-select-bg` (bianco al 12%, come da CSS) e senza la freccia nativa; la freccia è disegnata a parte in `field-text`. Testo di default "Seleziona la regione".
- Placeholder in `field-placeholder` a 0.8em, interlettera 0.01em.
- Al focus il bordo diventa di 2px (stesso colore, senza outline del browser).
- Etichette dei campi e delle scelte in `field-label`; sopra il campo, DM Sans 18px peso 500 (peso stimato dalla schermata).
- Radio e checkbox usano `field-check` (#D2C8BB): contorno 1px, diametro 15px, interno trasparente; se selezionati si riempiono di `field-check` con il pallino (radio) o la spunta (checkbox) nel colore della sezione. Non usare mai il blu del browser: imposta `accent-color` su `field-check` per i controlli nativi.
- Campi condizionali (marca e modello del veicolo) appaiono solo se la risposta è "Sì" e si svuotano quando si nascondono.
- Non usare questi campi su sezioni chiare: i fondi sono bianchi semitrasparenti.
- Raggio, padding e peso delle etichette sono misurati da una schermata, non da un file sorgente: se il builder mostra altri valori, correggi i token.
