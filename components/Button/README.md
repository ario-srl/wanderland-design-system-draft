Il bottone dei form multistep di Wanderland: principale (oro) per avanzare o iscriversi, secondario trasparente per tornare indietro.

**Cosa fornisce chi lo usa:** l'etichetta (verbo breve in italiano: "Procedi", "Iscriviti", "Indietro") e il contenitore.

- Il principale usa `button-bg` con testo `button-text`. È l'unico bottone pieno di una schermata.
- Il secondario ("Indietro") usa `button-secondary-bg`, bordo 2px `button-secondary-border` e testo `button-secondary-text`; vive solo su sezioni scure.
- Padding `space-14` in verticale e `space-26` in orizzontale (`space-18` sotto i 420px); gap `space-12`; font DM Sans 13px (12px sotto i 420px), line-height 1.1, testo su una riga.
- Su due bottoni affiancati dividono lo spazio in parti uguali; sotto i 340px si impilano.
- Raggio sempre `radius-pill` (9999px, il massimo): tutti i bottoni, principale e secondario, sono a pillola, anche a larghezza piena.
- Il testo bianco su oro ha contrasto 2.3:1: valore della sorgente, da migliorare solo se lo decidi tu. La sorgente non fornisce gli stati hover del bottone principale.
