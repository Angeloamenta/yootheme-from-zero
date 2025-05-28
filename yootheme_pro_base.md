# Guida YOOtheme Pro

## Introduzione

YOOtheme Pro è un potente tema/template per WordPress che include un builder visuale avanzato. Permette di creare facilmente siti web professionali e offre la possibilità di generare contenuti dinamici collegati direttamente al database di WordPress.

## Struttura Fondamentale

### Template e Layout

YOOtheme è basato su un framework coerente che mantiene uniformità tra tutti i template. Questo significa che:

- **Compatibilità universale**: Se importi un template, tutti condividono lo stesso core framework
- **Intercambiabilità**: Puoi prendere una pagina da un template (scaricando il quick_start) e importarla in un altro
- **Adattamento automatico**: La pagina importata adatterà automaticamente il suo stile a quello già presente nel sito di destinazione

### Componenti del Builder

Il builder di YOOtheme si articola in una **struttura gerarchica a tre livelli**:

1. **Sezioni**: Macroaree della pagina (es: hero, contenuto principale, testimonianze)
2. **Righe**: Suddivisioni orizzontali all'interno delle sezioni
3. **Colonne**: Suddivisioni verticali all'interno delle righe, che contengono gli elementi finali

**Principio di posizionamento**: Ogni elemento può essere posizionato uno sotto l'altro (verticalmente) o affiancato ad altri elementi (orizzontalmente).

### Gestione della Visibilità

#### Disabilitazione Temporanea

- È possibile **disabilitare** temporaneamente una sezione dalle impostazioni avanzate
- La sezione disabilitata rimane visibile nel builder (per facilità di gestione) ma non verrà mostrata online
- **Caso d'uso**: Utile per contenuti stagionali o che vengono inseriti e rimossi frequentemente

#### Ridistribuzione Intelligente dello Spazio

YOOtheme gestisce automaticamente lo spazio disponibile: se disabiliti un elemento (es. una colonna centrale in un layout a 3 colonne), lo spazio non rimarrà vuoto ma verrà ridistribuito automaticamente tra gli elementi rimanenti (le altre due colonne occuperanno il 50% ciascuna).

## Contenuti Dinamici

### Creazione di Contenuti Dinamici

**Procedimento passo-passo**:

1. **Aggiungi un elemento multiplo** (es. Grid, Gallery, Slider)
2. **Accedi alle impostazioni avanzate** e seleziona "contenuto dinamico"
3. **Scegli la fonte dei contenuti** (es. "articoli personalizzati", "pagine", "prodotti WooCommerce")
4. **Imposta i filtri** per tag, categorie o altri parametri di selezione
5. **Configura visualizzazione**: imposta l'indice di partenza e la quantità di contenuti da visualizzare
6. **Definisci l'ordinamento** (cronologico, alfabetico, o anche per custom fields)

**Suggerimento avanzato**: L'ordinamento tramite custom fields è particolarmente utile per gestioni complesse, come un calendario eventi ordinato per data.

### Condizioni Dinamiche

Puoi impostare **condizioni di visualizzazione** per mostrare contenuti solo se soddisfano determinati criteri:

- Caricare l'articolo solo se il contenuto non è vuoto
- Visualizzare elementi solo se il titolo è presente
- Mostrare sezioni solo per determinate categorie di utenti
- Altri criteri personalizzabili basati sui campi disponibili

### Selezione del Contenuto Effettivo

**Dopo aver impostato la fonte dei contenuti dinamici**:

1. **Torna alla scheda "Contenuto"** dell'elemento
2. **Vedrai apparire la dicitura "Dinamico"** accanto ai campi disponibili
3. **Cliccando su questa opzione** potrai selezionare quale contenuto specifico inserire (titolo, excerpt, immagine in evidenza, etc.) e dove posizionarlo

## Stile e Formattazione

### Impostazioni di Stile

Nella sezione "Stile" puoi configurare:

- **Colori di sfondo**: Tinte unite, gradienti o immagini
- **Stili predefiniti**: Template di design già pronti inclusi nel tema
- **Colore del testo**: Modalità light/dark per adattarsi al contrasto dello sfondo
- **Larghezza massima**: Controllo della larghezza del contenuto (indipendente dall'immagine di sfondo)

### Effetti Speciali

#### Sticky Effect (Effetto Appiccicoso)

- **Cover**: La sezione viene gradualmente coperta dalla sezione successiva durante lo scrolling
- **Reveal**: La sezione viene rivelata progressivamente dalla sezione precedente durante lo scrolling

#### Intestazione Trasparente

- **Limitazione**: Funziona esclusivamente per la prima sezione della pagina
- **Comportamento**: Posiziona la sezione sotto il menu principale, integrando la header nella prima sezione (es. sezione hero)
- **Opzione "Spingi il contenuto"**: Garantisce che l'altezza della sezione sia calcolata correttamente partendo dall'inizio effettivo del contenuto

## Layout delle Colonne

### Dimensionamento e Ordinamento

- **Dimensionamento responsive**: Puoi modificare la grandezza di ogni colonna in base al dispositivo di visualizzazione
- **Sistema frazionario**: Il formato standard 1/1 occuperà il 100% dello spazio disponibile, 1/2 occuperà il 50%, ecc.
- **Riordinamento**: Possibilità di cambiare l'ordine delle colonne in base alla dimensione del dispositivo (es. su mobile invertire l'ordine rispetto al desktop)

### Effetto Sticky per Colonne

#### Funzionamento Base

- **Opzione sticky**: Rende una colonna "appiccicosa" durante lo scrolling
- **Comportamento adattivo**: La colonna sticky può seguire l'altezza della colonna adiacente
- **Risultato**: Mantiene visibile il contenuto importante durante lo scrolling della pagina

#### Sticky Offset (Distanza dall'Alto)

Controlla la distanza dalla parte superiore della finestra:

- **Valore 0**: La colonna inizia l'effetto sticky quando tocca il bordo superiore della finestra
- **Valore personalizzato** (es. 100px): La colonna inizierà l'effetto sticky mantenendo 100px di distanza dal bordo superiore (utile se hai un header fisso)

## Impostazioni Avanzate

### CSS Personalizzato

- **Inserimento codice**: Possibilità di aggiungere codice CSS specifico per ogni elemento
- **Sistema di suggerimenti**: Il builder suggerisce gli elementi CSS da selezionare
- **Targeting selettivo**: Il CSS viene applicato in modo specifico - se modifichi lo stile di un elemento (es. `.item {color: red;}`), il cambiamento sarà applicato solo all'elemento selezionato e non a tutti gli elementi simili nella pagina

### Attributi Personalizzati

- **Attributi HTML custom**: Possibilità di aggiungere attributi HTML personalizzati agli elementi
- **Casi d'uso**: Utile per integrazioni JavaScript, tracciamento analytics, o compatibilità con plugin specifici

## Header e Footer Personalizzabili

### Footer Personalizzabile

**Procedimento**:

1. Accedi a **Layout > Footer** nel pannello di amministrazione
2. **Crea un nuovo layout** utilizzando lo stesso builder drag-and-drop
3. **Applicazione automatica**: Il footer creato sarà automaticamente visibile in tutte le pagine del sito

### Header Personalizzabile

**Procedimento**:

1. Accedi a **Appearance > Customize** (o YOOtheme > Customize)
2. Nella sezione **Builder**, seleziona la scheda **"Header"**
3. **Personalizzazione completa**: Utilizza lo stesso builder per personalizzare l'header
4. **Elementi disponibili**: Logo, menu di navigazione, pulsanti, widget, elementi social e qualsiasi altro componente

**Funzionalità avanzate**:

- Header sticky (che rimane fisso durante lo scrolling)
- Header trasparenti con effetti di transizione
- Effetti di cambio stile durante lo scrolling
- Header condizionali in base al tipo di pagina o sezione del sito


## Suggerimenti per l'Uso Efficiente

### Best Practices

- **Sfrutta i preset**: Utilizza i layout predefiniti per velocizzare la creazione di sezioni comuni
- **Sezioni riutilizzabili**: Crea e salva sezioni personalizzate per mantenere coerenza visiva in tutto il sito
- **Automazione**: Utilizza i contenuti dinamici per automatizzare l'aggiornamento delle informazioni
- **Test responsive**: Verifica sempre la visualizzazione su diversi dispositivi e dimensioni schermo

### Ottimizzazione del Workflow

- Pianifica la struttura delle sezioni prima di iniziare
- Utilizza naming conventions consistenti per sezioni e elementi
- Sfrutta le condizioni dinamiche per content personalizzato

