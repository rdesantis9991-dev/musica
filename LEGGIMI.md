# Musica: come metterla sull'iPhone

L'app è fatta da questi file, da tenere insieme nella stessa cartella:
`index.html`, `sw.js`, `manifest.json`, `icon-180.png`, `icon-192.png`, `icon-512.png`.

## 1. Pubblicala su GitHub Pages
Il procedimento è lo stesso della app Palestra, ma in un **repository nuovo**:
1. Su GitHub: **+ → New repository**, nome `musica`, **Public**, poi **Create repository**.
2. Clicca **uploading an existing file** e trascina **i file**, non la cartella. Poi **Commit changes**.
3. Vai in **Settings → Pages**: *Deploy from a branch*, branch **main**, cartella **/ (root)**, poi **Save**.
4. Dopo 1–2 minuti l'app è online su `https://TUONOME.github.io/musica/`.

⚠️ **Non caricare i tuoi MP3 su GitHub.** Il repository è pubblico: i brani si caricano direttamente nell'app, dal telefono.

## 2. Installala
1. Apri il link con **Safari** sull'iPhone.
2. Tocca **Condividi → Aggiungi a schermata Home**.
3. Aprila **una volta dall'icona con internet attivo**. Da lì in poi funziona anche offline.

## 3. Carica i brani
1. Porta gli MP3 nell'app **File** dell'iPhone. Il modo più comodo da Windows è **iCloud Drive**: installa iCloud per Windows oppure usa icloud.com, e trascina gli MP3 in una cartella. Vanno bene anche OneDrive o Google Drive, se ce li hai.
2. Nell'app tocca **+** (oppure **Aggiungi brani**), apri la cartella, tocca **Seleziona** e scegli i brani, oppure **Seleziona tutto**.
3. L'app copia i brani nella sua memoria e legge da sola titolo, artista, album e copertina. Se un MP3 non ha i tag, usa il nome del file: un file chiamato `Artista - Titolo.mp3` viene riconosciuto.

## Come si usa
- **Libreria**: playlist, artisti, album, brani e gli ultimi aggiunti.
- Tocca un brano per ascoltarlo. Con **Riproduci** e **Casuale** ascolti tutto un album, un artista o una playlist.
- **•••** accanto a un brano apre il menu: riproduci dopo, aggiungi in coda, aggiungi a una playlist, vai all'album, elimina.
- Tocca il **mini player** in basso per aprire la schermata grande. Trascinala verso il basso per chiuderla. In basso trovi casuale, coda ("A seguire") e ripeti (tocca più volte: tutto → un brano → spento).
- **Cerca**: trova brani, album e artisti nella tua libreria.
- **Resoconto**: quanto tempo hai ascoltato (7 giorni, 30 giorni, 12 mesi o da sempre), il confronto con il periodo precedente e il grafico giorno per giorno (tocca una barra per vedere il dettaglio). Trovi anche i top 5 artisti, i top 5 brani, i top 3 album, i giorni di fila in cui hai ascoltato e il momento della giornata in cui ascolti di più. Un brano conta come ascoltato dopo 30 secondi, o dopo metà brano se è più corto. Le statistiche si azzerano da Impostazioni.
- **Impostazioni**: l'opzione *Controlli sempre attivi in pausa* (il trucco della pausa finta) e lo spazio occupato.

## Da sapere
- **I brani esistono solo nel telefono.** Se togli l'icona dalla Home si cancellano, quindi tieni gli originali su iCloud o sul PC.
- **Pausa finta**: quando metti in pausa, l'app in realtà continua a riprodurre silenzio, così il tasto ▶︎ sulla schermata di blocco risponde sempre. Dopo 30 minuti si ferma davvero. Se dà fastidio, ad esempio con altre app audio, la spegni dalle Impostazioni.
- **È un trucco, non una garanzia.** iOS tratta le web app peggio delle app native, e un aggiornamento di iOS potrebbe cambiare questo comportamento.
- I formati sicuri sono **MP3** e **M4A/AAC**. Per gli M4A titolo e artista vengono presi dal nome del file.
- **Per aggiornare l'app** modifichi i file su GitHub. Sul telefono la nuova versione arriva alla seconda apertura, con internet attivo. I brani e le playlist restano.
