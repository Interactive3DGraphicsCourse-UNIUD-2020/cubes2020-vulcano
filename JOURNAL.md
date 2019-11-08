# 5 novembre
- ricerca in rete di immagini e video da cui trarre ispirazione. Interessante l'idea di creare uno scenario non realistico: prendendo spunto dal gioco *Cat Bird*, la scena sarà un'isola fluttuante ricoperta di vegetazione. L'idea è di creare un ambiente con i cui componenti è possibile interagire;
- schizzi su carta per decidere la forma dell'isola. La scelta cade su un teschio, per richiamare alla mente storie di pirati/avventurieri ("un'isola leggendaria difficile da raggiungere e che nasconde grandi ricchezze...");
- uso dell'editor di three.js per iniziare a costruire l'isola;
- idea: far ruotare attorno all'isola altre isole più piccole, come se l'isola fosse un pianeta e le isolette i satelliti.

![Alt text](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/Skull_1.png)

# 6 novembre
- tamite editor di three.js: piccole modifiche alla morfologia dell'isola e aggiunta di texture ai cubi;
- tramite editor di three.js: modellazione di un oggetto albero e di un oggetto cespuglio;

![Alt text](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/albero_obj.png)

![Alt text](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/cespuglio_obj.png)

- aggiunta dei nuovi oggetti alla scena dell'isola;
- dopo aver eliminato le luci aggiunte per esigenze di comodità durante la modellazione, esportazione della scena finale.

![Alt text](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/Skull_2.png)

# 7 novembre
- studio dello starting code con le luci;
- sostituzione degli oggetti presenti nella scena con i nuovi (isola fluttuante grande e due isolette minori);
- problema: il modello dell'isola grande è lento ad essere caricato e mostrato a scehrmo;
- regolazione delle luci;
- colorazione del background così da richiamare il concetto di alba/tramonto.

![Alt text](https://github.com/Interactive3DGraphicsCourse-UNIUD-2020/cubes2020-vulcano/blob/master/screenshots/Scene_1.png)

# 8 novembre
- idea: invece di far ruotare le isolette, farle muovere solo lievemente per suggerire l'idea che siano sospese in aria. Dotata di un tipo di movimento simile anche l'isola grande.
- idea: rendere possibile l'interazione con le isolette tramite un evento mouseover. All'hover, le isole ruotano su loro stesse e causano un cambiamento di illuminazione della scena e di colorazione dello sfondo. L'effetto finale vuole essere la simulazione del passaggio accelerato da notte a giorno (e viceversa), ovvero dello scorrere accelerato del tempo. L'isola (con relative isolette-satelliti) si configura dunque come luogo misterioso e magico.
