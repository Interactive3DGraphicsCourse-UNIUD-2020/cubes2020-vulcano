![scena](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/Scene_with_text.png)

# Progetto
Il progetto consiste in una scena interattiva che rappresenta un ambiente non realistico, ed è nato ispirandosi ai [pianeti del gioco *Cat Bird*](https://cat-bird.fandom.com/wiki/Grasi). La scena presenta un terreno roccioso irregolare sopra a cui fluttuano un'isola di grandi dimensioni, a forma di teschio, e due isolette minori. L'accuarata scelta di colori e i movimenti lenti, appena accenati, delle isole sono pensati per collocare gli oggetti nell'atmosfera calma e "sospesa" tipica delle albe e dei tramonti, con l'intenzione di suggerire l'idea dello scorrere-non scorrere del tempo. In aggiunta, la scritta posta al di sopra delle isole, che lega il luogo rappresentato alla capacità di controllare il tempo, è pensata per attirare definitivamente l'attenzione verso tale idea. 

È all'interno di questa minima cornice narrativa che si pongono le possibili interazioni - non esplicitamente indicate, ma semplici da scoprire - dell'utente con la scena: passando il mouse sulle isolette è possibile passare velocemente dalla notte all'alba (grazie all'isoletta bianca) e, viceversa, tornando indietro nel tempo, dall'alba alla notte (grazie all'isoletta marrone).

# File e strumenti utilizzati
La scena è stata costruita a partire dal codice sorgente dotato di luci e dal codice per l'estrazione dei valori dalla heightmap. Il codice della scena è contenuto nel file index.html, mentre gli script esterni, i modelli 3D, le texture e gli screenshot per l'illustrazione del progetto sono organizzati in directory. Per facilitare il lavoro di aggiornamento dei file si è fatto uso di GitHub Desktop.

Gli oggetti sono stati, in parte, realizzati con l'uso dell'editor di three.js (l'isola-teschio, compresa la vegetazione che la ricopre) e, in parte, sono stati programmati direttamente nel file index.html (le isolette e il terreno). L'immagine in scala di grigi con funzione di heightmap, invece, è stata disegnata con il software Gimp.

# Animazioni
Tutte e tre le isole compiono piccoli movimenti oscillatori (l'isola-teschio trasla verticalmente, le isolette ruotano attorno al centro della scena) per conferire l'illusione che stiano fluttuando in aria. Al mouseover, le isolette effettuano inoltre un movimento rotatorio su uno dei loro assi locali di riferimento (Y per l'isoletta scura, X per quella chiara) e comportano la modifica dei valori di intensità delle luci e di opacità dello sfondo della scena, che è sovrapposto al body colorato della pagina html e invisibile (opacità 0) al primo render. Lo screenshot posto a inizio di questo file illustra la scena durante il giorno (o, per meglio dire, all'alba), mentre le immagini seguenti mostrano la scena durante la fase di transizione dal giorno alla notte e durante la notte.

Quasi notte                |  Notte
:-------------------------:|:-------------------------:
![scena quasi notte](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/Scene_almost_night.png)  |  ![scena notte](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/Scene_night.png)

# Terreno
Sulla base dell'idea di rappresentare tramite cubi un terreno roccioso irregolare, si è scelto di usare i valori contenuti nella heightmap come fattori per scalare i cubi lungo il loro asse Y locale. Per sottolineare la natura irreale dell'ambiente di fantasia, si è inoltre scelto di disegnare chiaramente gli spigoli dei cubi.

# Processo
La prima fase del progetto ha previsto la ricerca in rete di esempi da cui trarre ispirazione e, trovata l'idea, l'esecuzione di schizzi su carta dei vari oggetti e della scena nel suo complesso. Il passo successivo è stato familiarizzare con l'editor di three.js per modellare l'isola-teschio. Dpodiché, si è iniziata la creazione della scena, con l'aggiunta di oggetti, la regolazione delle luci e la scelta dei colori. L'animazione giorno-notte non era compresa nella prima idea di progetto, che si focalizzava principalmente sull'animazione delle isole, e si è aggiunta solo dopo la scelta dei colori per lo sfondo. A seguito della suddetta animazione di luci e sfondo con mouseover, l'ultimo passo è consistito nella programmazione del terreno.
