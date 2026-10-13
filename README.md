Wanderland è un brand di viaggi in 4x4, in italiano, con tre linee: **Wanderland Labs**, **Wanderland Weekends** e **Wanderland Expeditions**. Il sistema si regge su crema e marrone scuro, un blu notte profondo, un oro tenue per le azioni e titoli in Feature Display.

## Contenuti e voce

- Scrivi in italiano. I bottoni sono verbi brevi all'imperativo: "Procedi", "Indietro", "Iscriviti". Le risposte del form sono "Sì" e "No".
- Scrivi il nome delle linee come "Wanderland" seguito dal nome della linea in grassetto: Wanderland **Labs**, Wanderland **Weekends**, Wanderland **Expeditions**.
- Il titolo di esempio della landing parte dalla prima persona plurale ("Progettiamo itinerari, viaggi, …") e mette in corsivo, con il gradiente oro, una sola parola chiave: "Insieme" nell'H1.

## Colore

- Ci sono due temi. `light` per le sezioni chiare, `dark` per quelle scure. Imposta `data-theme` sul contenitore della sezione.
- Sezioni chiare: `cream` (principale), `white`, `mist`. Sezioni scure: `umber` (marrone) e `navy` (blu notte). Nei temi usa `surface` e `surface-alt` invece dei valori fissi.
- Titoli H1-H6 con `text-heading`: `navy` su sezioni chiare, `sand-96` su sezioni scure. Non usare `navy` come colore di testo su `navy`.
- Corpo del testo con `text-body`: `slate-70` su sezioni chiare, `amber` su sezioni scure. Le caption usano `text-caption`.
- Il bottone principale è `button-bg` con testo `button-text`. Il bottone secondario "Indietro" vive solo su sezioni scure e usa `button-secondary-bg` e `button-secondary-border`. Tutti i bottoni hanno sempre `radius-pill`.
- I campi del form sono un bordino `field-border` di 1px su `field-bg` trasparente (19%; il select 12%, `field-select-bg`), con `radius-field`. Radio e checkbox usano `field-check` (#D2C8BB), mai blu.
- Oro (`gold`, `gold-glow`, `gold-light`, `gold-deep`) e salvia (`sage`) servono ad azioni e alla parola evidenziata, mai come sfondo di sezione.
- I colori del logo (`forest`, `ember`, `stone`) sono decorativi. `forest` si usa solo su sezioni chiare; `ember` e `stone` non vanno usati per testo piccolo.
- Due coppie della sorgente sono sotto la soglia 4.5:1 e restano esatte: `slate-70` come testo corrente sulle sezioni chiare (3.7-4.1:1) e `button-text` bianco su `button-bg` (2.3:1). Se ti serve la leggibilità piena, usa `slate` (solido) per il corpo e `navy` sul bottone (7.0:1), e dichiaralo.

## Tipografia

- I titoli H1-H4 usano Feature Display (stile `h1` … `h4`). `h1` è Regular 400; `h2`-`h4` sono Medium 500 (file `FeatureDisplay-NormalMedium.ttf`). La famiglia non ha un SemiBold: non dichiarare 600, che il browser renderebbe con il Bold.
- H5 è Inter Semi Bold (`h5`). H6 è DM Sans Bold con tracking 3px (`h6`), senza trasformazione in maiuscolo.
- Gli eyebrow, le etichette brevi sopra i titoli H1-H4 ("IL PERCORSO", "PROGRAMMA"), vanno sempre in MAIUSCOLO: stile `eyebrow`, cioè DM Sans Bold 14px con tracking 3px e `text-transform: uppercase`. Scrivi il testo normalmente e lascia il maiuscolo al CSS.
- Il corpo del testo è DM Sans Regular 18px (`body`); le caption sono DM Sans Light 14px (`caption`).
- Su mobile usa `h1-mobile`, `h2-mobile` e `h3-mobile`. Tablet, laptop e desktop condividono gli stessi valori; H4-H6, body e caption sono uguali ovunque.
- Per la parola evidenziata in corsivo usa Feature Display Regular Italic (file nel sistema).
- DM Sans e Inter sono Google Fonts: caricale dal CSS di Google Fonts nelle pagine che consumano il sistema (DM Sans 300, 400, 700; Inter 600). Feature Display è un font con licenza: i file sono in `fonts/` e vanno caricati con `@font-face` come descritto in `tokens.json`.

## Forme, spazio e ombre

- I bottoni usano `radius-pill` (9999px, il massimo); i campi del form `radius-field` (4px).
- Le card polaroid usano `radius-card` (14px) per la cornice e `radius-photo` (10px) per la foto, con `shadow-polaroid`; la card in primo piano usa `shadow-polaroid-active`.
- La spaziatura documentata è quella dei componenti noti: `space-10` nei campi, `space-12` tra bottoni, `space-14` e `space-26` nelle cornici e nei bottoni, `space-18` sui bottoni stretti. Non esiste una scala generale: non inventare passaggi intermedi.
- Le foto hanno una leggera correzione: saturazione 0.95, contrasto 1.02.

## Movimento

- Effetto di lettura allo scroll: le parole passano da `read-off` a `read-on` (sezioni chiare) con una transizione colore di 200ms lineare.
- La parola evidenziata fluttua con un gradiente tra `gold-glow`, `gold-light`, `gold-deep` e `sage` in un ciclo di 5.2s.
- Le card a ventaglio si muovono con 420ms e curva `cubic-bezier(.2,.8,.2,1)`.
- Rispetta sempre `prefers-reduced-motion`: niente animazioni e gradiente fermo.

## Logo e favicon

- Il simbolo esiste in tre versioni con sfondo trasparente: a colori (`forest`, `ember`, `stone`), sabbia (`sand`) e bianco. Usa quello a colori su `cream`, `white` e `mist`; sabbia o bianco su `umber` e `navy`.
- Non ridisegnare il simbolo: usa sempre i file del gruppo `Logos`.
- Per la favicon usa i PNG del gruppo `Favicon` (16, 32, 48, 64, 180, 192, 512 px). Per i loghi in pagina usa le versioni `-trim`, ritagliate sul simbolo.
- Il logo è disponibile solo come PNG, senza versione con la scritta né SVG.

## Immagini

Le immagini si definiscono per gruppi. Gruppi definiti finora: il ruolo del veicolo; colore e momenti di vita quotidiana.

### Il veicolo è un elemento secondario

Il fuoristrada non è mai il protagonista. Un'immagine Wanderland regge anche se togli il veicolo con la mente: restano il paesaggio e i suoi dettagli, l'emozione del viaggio, le persone, il gruppo e l'avventura nel suo complesso.

- Il veicolo occupa una frazione ridotta dell'inquadratura; il paesaggio (terra, cielo, acqua, bosco) ne occupa la maggior parte.
- Mai frontale e centrato come in un catalogo. Preferisci inquadrature laterali, lontane, di tre quarti, tagliate dal bordo o viste da dentro (cornice dello sguardo verso l'esterno).
- Per avvicinarti usa controluce e silhouette, sfocato di movimento, oppure dettagli: portapacchi, portiera aperta, fari accesi, un fuoco accanto.
- Le persone ci sono o sono evocate: di spalle, in silhouette, piccole nello spazio, in gruppo mentre fanno qualcosa. Non posano e non guardano in camera.
- Luce naturale (alba, tramonto, nebbia, pioggia, notte con luci calde); colori spenti e cinematografici, vicini a `forest`, `sand`, `ember`, `umber` e `navy`. Mai saturi.
- Il mezzo è scuro, datato e vissuto, con il portapacchi carico; non lucido né nuovo.
- Le targhe non devono essere leggibili: coprile o scegli un'altra foto.

**Da evitare:** veicolo in posa frontale come hero o in primo piano; foto da concessionario o da studio; veicoli dai colori vivaci che attirano più del paesaggio; scene senza persone né segni di vita con il mezzo solo al centro.

### Vita quotidiana, dettagli e colore

I viaggi Wanderland servono a scoprire il mondo. Le immagini cercano l'intensità in ciò che sembra banale.

- Momenti di vita quotidiana: sempre spontanei, mai in posa. Le persone sono impegnate in un gesto, di profilo, di spalle, tagliate o in silhouette; evita lo sguardo in camera. Il soggetto è il luogo, il gesto e l'atmosfera, non l'oggetto turistico.
- Paesaggio: fotografa un elemento di dettaglio apparentemente insignificante (una scaletta arrugginita, l'erba, un riflesso, la linea di un ruscello) con un taglio deciso, finché mostra tutta la sua bellezza. Lascia spazio al vuoto o alla texture.
- Luoghi noti: mostrali di lato, con una guida visiva (ruscello, strada, sentiero), non a figura intera da cartolina.
- Colore: viene dal luogo, mai aggiunto in post. Base calda e spenta, da pellicola leggermente sbiadita, con al massimo un accento vivo già presente nella scena (cassette, giubbotto, stufa, reti). Riferimenti ai token: ocra e rame vicini a `amber` e `gold`, il verde profondo a `forest`, il crepuscolo a `ember` e `umber`, gli azzurri freddi a `navy` e `stone`.
- Luce naturale e bassa (alba, tramonto, finestra, cielo velato); mai flash o luce da studio.

**Da evitare:** pose da catalogo e sorrisi in camera, scene pulite e sterili, colori saturati o neon in post, monumenti frontali da cartolina, composizioni piene e simmetriche senza respiro.

**Persone e luoghi riconoscibili:** se nella foto si vedono volti riconoscibili, nomi o numeri di imbarcazioni, targhe o simili, servono liberatorie o una scelta diversa prima dell'uso commerciale.

## Componenti

- **Button**: bottone principale e secondario del form multistep.
- **FormField**: campo di testo, select ed etichette radio su sezione scura.
- **PolaroidCard**: card polaroid con foto e caption "Wanderland **Linea**".
- **GradientWord**: parola evidenziata in corsivo con gradiente nell'H1.
