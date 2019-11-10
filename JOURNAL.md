# 5 novembre
- ricerca in rete di immagini e video da cui trarre ispirazione. Interessante l'idea di creare uno scenario non realistico: prendendo spunto dal gioco *Cat Bird*, la scena sarà un'isola fluttuante ricoperta di vegetazione. L'idea è di creare un ambiente con i cui componenti è possibile interagire;
- schizzi su carta per decidere la forma dell'isola. La scelta cade su un teschio, per richiamare alla mente storie di pirati/avventurieri ("un'isola leggendaria difficile da raggiungere e che nasconde grandi ricchezze/misteri...");
- uso dell'editor di three.js per iniziare a costruire l'isola;
- idea: far ruotare attorno all'isola altre isole più piccole, come se l'isola fosse un pianeta e le isolette i satelliti.

![modello isola incompleto](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/Skull_1.png)

# 6 novembre
- decido di lavorare con il codice sorgente che prevede le luci e scelgo di conseguenza MeshPhongMaterial come materiale per i modelli;
- tamite editor di three.js: piccole modifiche alla morfologia dell'isola e aggiunta di texture ai cubi;
- tramite editor di three.js: modellazione di un oggetto albero e di un oggetto cespuglio;

![modello albero](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/albero_obj.png)

![modello cespuglio](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/cespuglio_obj.png)

- tamite editor di three.js: aggiunta dei nuovi oggetti alla scena dell'isola;
- dopo aver eliminato le luci aggiunte per esigenze di comodità durante la modellazione, esportazione della scena finale.

![modello isola completo](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/Skull_2.png)

# 7 novembre
- studio dello starting code con le luci;
- sostituzione degli oggetti presenti nella scena con i nuovi (isola fluttuante grande e due isolette minori);
- regolazione delle luci;
- colorazione del background così da richiamare il concetto di alba/tramonto.
- problema: il browser restituisce warning riguardo alla grandezza delle texture usate nel modello costruito con l'editor.

![scena con sfondo](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/Scene_1.png)

# 8 novembre
- idea: invece di far ruotare le isolette, farle muovere solo lievemente per suggerire l'idea che siano sospese in aria. Dotata di un tipo di movimento simile anche l'isola grande. Ho sperimentato con la funzione Math.sin per ottenere movimenti oscillatori.
- idea: rendere possibile l'interazione con le isolette tramite un evento mouseover. All'hover, le isole ruotano su loro stesse e causano un cambiamento di illuminazione della scena e di colorazione dello sfondo. L'effetto finale vuole essere la simulazione del passaggio accelerato da notte a giorno (e viceversa), ovvero dello scorrere accelerato del tempo. L'isola (con relative isolette-satelliti) si configura dunque come luogo misterioso e magico;
- creata nuova heightmap con Gimp e generato il terreno: ho scelto di scalare ogni cubo lungo l'asse y secondo il valore indicato dalla heightmap. Il risultato vuole assomigliare a un terreno roccioso irregolare, sopra cui fluttuano le isole.
- scelgo di colorare gli spigoli dei cubi del terreno per conferirgli un aspetto più geometrico e meno naturale;

![scena completa](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/Scene_final.png)

- problema: browser restituisce warning: capita più volte che il determinante di una qualche matrice sia 0 e che dunque non si riesca a calcolarne l'inversa. Sospetto che succeda durante la generazione del terreno.

# 9 novembre
- risolto problema determinante uguale a 0: tentavo di impostare il valore dato dalla heightmap per un certo cubo come fattore per la scalatura anche quando tale valore era uguale a zero. Ho risolto aggiungendo un controllo: se il valore è uguale a zero, la scalatura non viene eseguita;
- risolto problema warning texture: ridimensionate le texture del modello dell'isola grande e sostituite alle precedenti tramite l'editor;
- revisione codice e aggiunta di commenti;
- decisione di eliminare gli orbit controls perché non ritenuti adatti alla scena dal punto di visto dell'esperienza utente: guardare da vicino le isole potrebbe diminuire l'aura di mistero in cui sono immerse.

# 10 novembre
- aggiunto testo:

![scena completa con testo](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/Scene_with_text.png)

- decisione di non eliminare completamente gli orbit controls: disibalitata l'opzione di zoom e la rotazione attorno all'asse X;
- stesura file readme.
