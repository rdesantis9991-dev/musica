# Musica 3.0 per iPhone

L'app è fatta da questi file, da tenere insieme nella stessa cartella:
`index.html`, `sw.js`, `manifest.json`, `icon-180.png`, `icon-192.png`, `icon-512.png`.

## Novità della versione 3.0
- **Artisti in ordine.** Artista e titolo si prendono dal **nome del file** ("Geolier - STELLE.mp3"), non più dal tag che YouTube riempie con il nome del canale ("Geôlier2 OFFICIAL", "FedezChanneL"…). Nella lista Artisti restano solo gli artisti veri; chi compare solo come "feat." è in **Artisti → Ospiti nei brani**. Maiuscole, accenti e spazi non creano più doppioni ("ANNA" = "Anna", "ImagineDragons" = "Imagine Dragons").
- **Metti in ordine con Apple Music.** In Libreria (o in Impostazioni → Completa album e copertine) l'app cerca ogni brano nel catalogo di Apple Music e aggiunge album, numero di traccia, anno, genere e **copertina in alta qualità**. Nella pagina di un artista trovi Album, **Singoli ed EP** e "Appare in". Se un brano finisce nell'album sbagliato: menu **••• → Scegli l'album…**. Tutto si annulla da Impostazioni → Ripristina le informazioni originali.
- **Avanti e indietro nel mini player**, e scorrendo il mini player a sinistra o a destra cambi brano. Sulla schermata di blocco compaiono brano precedente/successivo invece di ±10 secondi.
- **Solo nell'app installata con Sideloadly:**
  - **cartella Musica**: copia brani o intere cartelle nella cartella "Musica" dell'app, dall'app File (Sul mio iPhone → Musica) o dal PC con iTunes (icona dell'iPhone → Condivisione file → Musica). All'apertura l'app li importa da sola e li toglie dalla cartella;
  - **vibrazione leggera** quando tocchi i comandi.
- Le categorie di YouTube ("Music", "Gaming") non compaiono più come generi.

## Aggiornare alla 3.0
1. Su GitHub, nel repository `musica`: **Add file → Upload files**, trascina **`index.html` e `sw.js`** di questa cartella e fai **Commit changes**.
2. Poi apri `.github/workflows/build-ios.yml`, clicca la **matita**, cancella tutto il contenuto, incolla quello del file `build-ios.yml` di questa cartella e fai **Commit changes**.
3. Quando in **Actions** compare la spunta verde, scarica il nuovo **Musica.ipa** da **Releases** e installalo con Sideloadly come la prima volta. **Brani, playlist e resoconto restano**: al primo avvio l'app sistema da sola artisti e titoli.

## Aggiornare dalla versione 1 alla 2
Nel repository `musica` su GitHub ricarica **`index.html`, `sw.js` e `manifest.json`**, sostituendo i vecchi file. Poi apri l'app sull'iPhone con internet attivo, chiudila e riaprila: compare la versione 2.0.
**Brani, playlist e resoconto restano tutti.** Al primo avvio l'app rilegge i brani già importati per aggiungere anno, genere, testi e i nomi di tutti gli artisti.

## Prima installazione
1. Su GitHub: **+ → New repository**, nome `musica`, **Public**, poi **Create repository**.
2. Clicca **uploading an existing file**, trascina **i file** (non la cartella), poi **Commit changes**.
3. Vai in **Settings → Pages**: *Deploy from a branch*, branch **main**, cartella **/ (root)**, poi **Save**.
4. Dopo 1–2 minuti apri `https://TUONOME.github.io/musica/` con **Safari** sull'iPhone, poi **Condividi → Aggiungi a schermata Home**.
5. Aprila **una volta dall'icona con internet attivo**. Da lì in poi funziona anche offline.

⚠️ **Non caricare gli MP3 su GitHub**: il repository è pubblico. I brani si caricano dal telefono, con il tasto **+** della Libreria.

## Le sezioni
- **Home**
  - mix pronti da ascoltare in ordine casuale: tutta la libreria, Preferiti, "Il tuo mese", "Da riascoltare", Aggiunti di recente;
  - ascoltati di recente;
  - brani in alta rotazione;
  - i tuoi artisti.
- **Libreria**
  - in alto ci sono gli elementi segnati con la ☆, cioè album, artisti e playlist preferiti;
  - sotto trovi Playlist, Artisti, Album, Brani e Generi.
- **Resoconto**
  - tempo di ascolto e top artisti, brani e album;
  - in quali momenti della giornata ascolti.
- **🔍 Cerca**
  - artisti, album e brani;
  - senza scrivere niente puoi sfogliare per genere.
- **👤 in alto a destra**: le Impostazioni.

## Artisti
- Un brano con più artisti finisce sotto **ciascun artista**. Valgono tutti questi casi:
  - "Lazza feat. Sfera Ebbasta";
  - "Lazza, Sfera Ebbasta";
  - "Lazza & Sfera Ebbasta";
  - "Brano (feat. Lazza)" nel titolo.

  L'album invece resta unito sotto l'artista principale.
- La **pagina di un artista** mostra:
  - prima i brani, ordinati dai più ascoltati;
  - poi i suoi album;
  - poi "Appare in", cioè gli album di altri artisti dove compare.
- **Preferiti**: tocca la ☆ in alto. Gli artisti preferiti compaiono in cima alla lista Artisti, in Libreria e nella Home.
- Se un gruppo con "&" o la virgola nel nome viene diviso per errore, hai due modi per sistemarlo:
  - dalla sua pagina tocca **••• → Non separare "…"**;
  - oppure aggiungi il nome in **Impostazioni → Artisti**.

  Molti gruppi famosi, come Simon & Garfunkel o Earth, Wind & Fire, sono già riconosciuti.

## Altre funzioni
- **Testi**: nella schermata "In riproduzione" tocca il fumetto in basso a sinistra.
  - L'app legge i testi salvati nei file MP3 e M4A.
  - Puoi incollarne uno da **••• → Modifica informazioni**.
  - Se il testo è in formato LRC (`[01:23.45] riga`) scorre a tempo di musica, e toccando una riga si salta a quel punto.
- **A seguire**: tocca l'icona in basso a destra.
  - Lì trovi casuale e ripeti, e puoi togliere brani dalla coda.
  - Ripeti cambia a ogni tocco: tutto, poi un brano, poi spento.
- **Timer di spegnimento**: nella schermata "In riproduzione" tocca **•••**. Puoi scegliere 15, 30 o 45 minuti, 1 ora o la fine del brano.
- **Modifica informazioni**: dal menu ••• di un brano puoi cambiare titolo, artista, album, anno, genere, testo e copertina, scegliendo una foto.
- **Modifica album**: dal menu ••• di un album le modifiche valgono per tutti i brani.
  - Per le raccolte scrivi "Artisti vari" come artista album.
- **Ordina**: in Brani e Album, con il pulsante con le frecce. In Brani c'è anche l'indice A–Z sul lato destro.
- **Indietro**: scorri dal bordo sinistro dello schermo, come nelle app Apple.
- **AirPlay**: il pulsante compare in basso al centro della schermata "In riproduzione" quando c'è un dispositivo AirPlay disponibile.

## Da sapere
- **I brani esistono solo nel telefono.** Se togli l'icona dalla Home vengono cancellati, quindi tieni gli originali su iCloud o sul PC.
- **Pausa finta** (Impostazioni): in pausa l'app continua a riprodurre silenzio, così il tasto ▶︎ sulla schermata di blocco risponde sempre. Dopo 30 minuti si ferma davvero. È un trucco e non una garanzia: un aggiornamento di iOS potrebbe cambiare questo comportamento.
- **Formati**: MP3 e M4A/AAC, con titolo, artista, album, anno, genere, copertina e testo letti dai tag.

## App vera per iPhone (con Sideloadly)
Oltre alla versione web, GitHub può trasformare l'app in un'app installabile (Musica.ipa), con la musica che continua a schermo spento.
1. **Una volta sola**: nel repository `musica` su GitHub clicca **Add file → Create new file**. Come nome scrivi `.github/workflows/build-ios.yml`, incolla tutto il contenuto del file `build-ios.yml` di questa cartella, poi **Commit changes**.
2. Da lì in poi, ogni volta che carichi file nuovi GitHub ricompila l'app da solo (circa 5–10 minuti). L'avanzamento si vede nella scheda **Actions**.
3. Quando ha finito, nella pagina del repository apri **Releases** (colonna destra) e scarica **Musica.ipa**.
4. Installala con **Sideloadly**: iPhone collegato via cavo, trascina il file, inserisci l'Apple ID, **Start**.
5. Sull'iPhone: Impostazioni → Generali → VPN e gestione dispositivi → il tuo Apple ID → **Autorizza**.
- Con l'Apple ID gratuito l'app va rinnovata ogni 7 giorni con Sideloadly; i brani restano.
- L'app vera e la versione web hanno archivi separati: la prima volta i brani vanno ricaricati.
