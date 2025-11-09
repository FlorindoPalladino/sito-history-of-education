# History of Education Journal Hub

Un portale centralizzato per la ricerca accademica nella Storia dell'Educazione, con ricerca federata su tutte le principali riviste del settore.

## 🎯 Caratteristiche

- **Ricerca Unificata**: Cerca articoli su tutte le riviste di storia dell'educazione da un'unica barra di ricerca
- **Categorizzazione Completa**: Riviste organizzate per livello (Global-Tier, Flagship, Tematiche) e per area geografica/linguistica
- **Design Responsive**: Funziona perfettamente su desktop, tablet e smartphone
- **Open Access**: Completamente gratuito e accessibile

## 📋 Come Attivare la Barra di Ricerca

Per attivare la potente barra di ricerca che consente di cercare articoli in **tutte le riviste**, segui questi 5 semplici passaggi.

⏱️ **Tempo richiesto**: circa 5-10 minuti
💡 **Competenze richieste**: Nessuna competenza di programmazione necessaria!

### Passaggio 1: Vai al sito di Google PSE

1. Apri questa pagina nel tuo browser: [https://programmablesearchengine.google.com/](https://programmablesearchengine.google.com/)
2. Se richiesto, accedi con il tuo account Google

### Passaggio 2: Crea un nuovo Motore di Ricerca

1. Fai clic su **"Aggiungi"** o **"Inizia"** (o "Add" / "Get Started" se l'interfaccia è in inglese)
2. Ti verranno chieste due informazioni:
   - **Nome del motore di ricerca**: Inserisci un nome descrittivo (es. "Ricerca Storia Educazione")
   - **Siti in cui cercare**: Qui è dove specificherai quali siti scansionare (vedi passaggio 3)

### Passaggio 3: Aggiungi gli URL delle Riviste

1. Nella sezione **"Siti in cui cercare"** (o "Sites to search"), devi aggiungere l'elenco di tutti i siti delle riviste
2. **Copia e incolla** l'intero elenco sottostante nella casella. Puoi incollarli tutti insieme, uno per riga:

```
https://www.tandfonline.com/toc/cpdh20/current
https://www.cambridge.org/core/journals/history-of-education-quarterly
https://www.tandfonline.com/toc/thed20/current
https://www.emerald.com/her
https://historicalstudiesineducation.ca/
https://www.infoagepub.com/american-educational-history-journal.html
https://journals.openedition.org/histoire-education/
https://www.dgfe.de/sektionen-kommissionen-ag/sektion-1-historische-bildungsforschung/jahrbuch
https://www.rivistadistoriadelleducazione.it/
https://www.hecl.it
https://revistas.usal.es/tres/index.php/0212-0267
https://revistas.uptc.edu.co/index.php/historia_educacion_latinamerican/
https://www.scielo.br/j/rbhe/
http://seer.ufrgs.br/asphe
https://seer.ufu.br/index.php/che/
https://www.tandfonline.com/toc/cjeh20/current
https://global.oup.com/academic/content/series/h/history-of-universities-series-hou/
```

3. Assicurati che l'opzione **"Cerca nell'intero sito"** (o "Include all pages whose address contains this URL") sia **selezionata** per ciascun URL
4. Fai clic su **"Crea"** (o "Create")

### Passaggio 4: Ottieni il tuo ID Motore di Ricerca (CX ID)

1. Dopo aver fatto clic su "Crea", Google ti porterà a una pagina di congratulazioni o direttamente al pannello di controllo
2. Vai alla sezione **"Panoramica"** o **"Impostazioni di base"** (Overview / Basic settings)
3. Cerca il campo chiamato **"ID motore di ricerca"** (o "Search engine ID")
4. **Copia** questo codice. Assomiglierà a qualcosa come: `a1b2c3d4e5f6g7h8i9`

   🔑 **Questo è il tuo CX ID** - ne avrai bisogno nel prossimo passaggio!

### Passaggio 5: Incolla l'ID nel file `index.html`

1. Apri il file **`index.html`** con un qualsiasi editor di testo (Blocco Note su Windows, TextEdit su Mac, o qualsiasi altro editor)
2. Cerca questa riga di codice (circa alla riga 25):

   ```html
   <script async src="https://cse.google.com/cse.js?cx=IL_TUO_ID_CX_QUI"></script>
   ```

3. **Sostituisci** `IL_TUO_ID_CX_QUI` con il **CX ID** che hai copiato nel passaggio 4

   **Esempio PRIMA:**
   ```html
   <script async src="https://cse.google.com/cse.js?cx=IL_TUO_ID_CX_QUI"></script>
   ```

   **Esempio DOPO** (con un ID fittizio):
   ```html
   <script async src="https://cse.google.com/cse.js?cx=a1b2c3d4e5f6g7h8i9"></script>
   ```

4. **Salva** il file `index.html`

### ✅ Fatto!

Ora **apri il file `index.html`** nel tuo browser (doppio clic sul file, oppure tasto destro → "Apri con" → seleziona il tuo browser preferito).

Il sito web è completo e la **barra di ricerca è attiva e funzionante**! 🎉

## 📚 Riviste Incluse

### Global-Tier (4 riviste)
- Paedagogica Historica (ISCHE)
- History of Education Quarterly (USA)
- History of Education (UK)
- History of Education & Children's Literature (Italia)

### Flagship - Area Anglofona (3 riviste)
- History of Education Review (Australia/NZ)
- Historical Studies in Education (Canada)
- American Educational History Journal (USA)

### Flagship - Area Francofona (1 rivista)
- Histoire de l'éducation (Francia)

### Flagship - Area Germanofona (1 rivista)
- Jahrbuch für Historische Bildungsforschung (Germania)

### Flagship - Area Italofona (1 rivista)
- Rivista di Storia dell'Educazione (Italia)

### Flagship - Area Iberica e Latinoamericana (5 riviste)
- Historia de la Educación. Revista interuniversitaria (Spagna)
- Revista Historia de la Educación Latinoamericana (Colombia)
- Revista Brasileira de História da Educação (Brasile)
- História da Educação - ASPHE (Brasile)
- Cadernos de História da Educação (Brasile)

### Riviste Tematiche (2 riviste)
- Canadian Journal of Education History
- History of Universities (OUP)

## 🛠️ Struttura del Progetto

```
sito-history-of-education/
│
├── index.html          # Pagina principale con la struttura e i dati
├── style.css           # Stili CSS per il design
└── README.md           # Questo file (istruzioni)
```

## 🌐 Hosting del Sito

### Opzione 1: Uso Locale
Semplicemente apri `index.html` nel tuo browser. Non serve un server web!

### Opzione 2: GitHub Pages (Gratuito)
1. Crea un repository su GitHub
2. Carica i file `index.html`, `style.css`, e `README.md`
3. Vai su Settings → Pages
4. Seleziona il branch `main` come sorgente
5. Il tuo sito sarà disponibile a `https://tuo-username.github.io/nome-repository/`

### Opzione 3: Netlify o Vercel (Gratuito)
1. Carica i file su un repository Git (GitHub, GitLab, ecc.)
2. Connetti il repository a Netlify o Vercel
3. Deploy automatico!

## 🔧 Personalizzazione

### Aggiungere una nuova rivista

1. Apri `index.html`
2. Trova la sezione `const data = {` (circa alla riga 39)
3. Aggiungi la tua rivista nell'array appropriato seguendo il formato esistente:

```javascript
{
    "nome": "Nome Rivista",
    "affiliazione": "Organizzazione",
    "editore": "Nome Editore",
    "regione": "Paese/Regione",
    "lingue": "Italiano, Inglese",
    "url": "https://www.esempio.com"
}
```

4. **Non dimenticare** di aggiungere l'URL anche al motore di ricerca Google PSE!

### Modificare i colori

Apri `style.css` e modifica le variabili CSS nella sezione `:root`:

```css
:root {
    --primary-color: #2c3e50;      /* Colore principale */
    --accent-color: #0056b3;       /* Colore accento (link, bottoni) */
    --card-bg: #ffffff;            /* Sfondo delle card */
    /* ... */
}
```

## 🤝 Contributi

Hai suggerimenti per migliorare il sito o vuoi aggiungere altre riviste? Sentiti libero di proporre modifiche!

## 📧 Supporto

Se hai problemi con la configurazione del Google Programmable Search Engine, consulta la [documentazione ufficiale di Google](https://support.google.com/programmable-search/answer/9870091?hl=it).

## 📄 Licenza

Questo progetto è fornito "as is" per facilitare la ricerca accademica. Tutti i link e i contenuti delle riviste appartengono ai rispettivi editori.

---

**Buona ricerca! 📖✨**
