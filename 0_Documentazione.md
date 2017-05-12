# Survey Station


## Test

### Protocollo di test

|Test Case      | TC-001                               |
|---------------|--------------------------------------|
|**Nome**       |Dati da sismografo a shake. |
|**Riferimento**|REQ-003                               |
|**Descrizione**|Quando si chiama la procedura i dati non più vecchi di un determinato valore vengono inseriti dalla tabelle sismografo nella shake.  |
|**Prerequisiti**|Bisogna aver creato la tabella sismografo e shake.|
|**Procedura**     | Si inserisce qualche dato nella tabella sismografo. Si aspettano 2 minuti e si chiama la procedura passandole un Id e come quantitativo dei minuti si inserisce 5.|
|**Risultati attesi** |Nella tabella shake ci devono essere i dati che ho inserito 2 minuti fa. |

<br>

|Test Case      | TC-002                               |
|---------------|--------------------------------------|
|**Nome**       | Individuamento picco di dati.|
|**Riferimento**|REQ-003                               |
|**Descrizione**| Quando viene rilevato un dato interessante i dati cominciano ad essere inseriti nella tabella shake. |
|**Prerequisiti**|Bisogna aver creato la tabella sismografo, shake, configurazione e la procedura storePreviousValues.|
|**Procedura**     |In sismografo si inseriscono dei valori non interessanti. Successivamente si inserisce un valore interessante e dopo altri dati di cui valore non è importante. |
|**Risultati attesi** |Nella tabella shake ci devono essere i dati a partire da quando c'è stato il picco. |

<br>

|Test Case      | TC-003                               |
|---------------|--------------------------------------|
|**Nome**       | Cancellare dati vecchi.|
|**Riferimento**|REQ-003                               |
|**Descrizione**| La procedura, una volta chiamata, deve cancellare i dati più vecchi di un determinato lasso temporale (specificato nel parametro) dalla tabella sismografo. |
|**Prerequisiti**|Bisogna aver creato la tabella sismografo e configurazione.|
|**Procedura**     | Si inseriscono dei dati nella tabella sismografo. Se il parametro che specifica dopo quanto tempo eliminare i dati equivale ad 2, si aspettano 2 minuti. Si chiama la procedura deleteOldData.|
|**Risultati attesi** |Nella tabella sismografo non ci devono più essere dati. |

<br>

|Test Case      | TC-004                               |
|---------------|--------------------------------------|
|**Nome**       | Cancellare dati vecchi.|
|**Riferimento**|REQ-003                               |
|**Descrizione**| La procedura, una volta chiamata, deve cancellare i dati più vecchi di un determinato lasso temporale (specificato nel parametro) dalla tabella sismografo. |
|**Prerequisiti**|Bisogna aver creato la tabella sismografo e configurazione.|
|**Procedura**     | Si inseriscono dei dati nella tabella sismografo. Se il parametro che specifica dopo quanto tempo eliminare i dati equivale ad 2, si aspettano 2 minuti. Si chiama la procedura deleteOldData.|
|**Risultati attesi** |Nella tabella sismografo non ci devono più essere dati. |

<br>

|Test Case      | TC-005                               |
|---------------|--------------------------------------|
|**Nome**       | Cancellare dati vecchi.|
|**Riferimento**|REQ-003                               |
|**Descrizione**| La procedura, una volta chiamata, deve cancellare i dati più vecchi di un determinato lasso temporale (specificato nel parametro) dalla tabella sismografo. |
|**Prerequisiti**|Bisogna aver creato la tabella sismografo e configurazione.|
|**Procedura**     | Si inseriscono dei dati nella tabella sismografo. Se il parametro che specifica dopo quanto tempo eliminare i dati equivale ad 2, si aspettano 2 minuti. Si chiama la procedura deleteOldData.|
|**Risultati attesi** |Nella tabella sismografo non ci devono più essere dati. |

<br>

|Test Case      | TC-006                               |
|---------------|--------------------------------------|
|**Nome**       | Immagazzinare dati ogni minuto.|
|**Riferimento**|REQ-003                               |
|**Descrizione**| Tramite un evento, la procedura storePreviousData viene chiamata autonomamente ogni minuto. |
|**Prerequisiti**|Bisogna aver creato la tabella sismografo, shake e la procedura storePreviousData.|
|**Procedura**     |Si fa partire l'evento (quando si crea il database). Si inseriscono dei dati in sismografo. |
|**Risultati attesi** |Dopo un minuto i dati devono essere nella tabella shake. |

<br>

|Test Case      | TC-007                               |
|---------------|--------------------------------------|
|**Nome**       | Cancellare dati ogni ora.|
|**Riferimento**|REQ-003                               |
|**Descrizione**| Tramite un evento, la procedure deleteOldData viene chiamata autonomamente ogni minuto. |
|**Prerequisiti**|Bisogna aver creato la tabella sismografo, shake e la procedure deleteOldData.|
|**Procedura**     |Si fa partire l'evento (quando si crea il database). Si inseriscono dei dati in sismografo.|
|**Risultati attesi** |Dopo un minuto nella tabella sismografo non ci deve essere più nessun dato. |


































### Mancanze/limitazioni conosciute
Per quanto riguarda l'ambiente database un'ostacolo è stata la mancanta d'esperienza di creazione e d'utilizzo dei trigger, procedure ed eventi (quest'ultimi mai trattati). Sono convinto del fatto che se avessi avuto un pò più d'esperienza in quest'ambito sarei riuscito ad arrivare alla soluzione auspicata in minor tempo. Inoltre per quanto riguarda il capitolo degli eventi, non avendolo mai accennato in classe, mi sono dovuto affidare totalmente ad internet. Infatti un evento non funzionava e non sono riuscito a capire il perché. Ritengo che un'infarinatura di base mi avrebbe permesso di trovare una possibile soluzione.


### Considerazioni personali
* Jacopo Greppi
  * Inizialmente quando ci è stato assegnato il progetto ero totalmente spiazzato poiché mi sembrava un lavoro talmente impegnativo e complicato che non pensavo che ce l'avessi potuta fare. Piano piano abbiamo iniziato a suddividerci il lavoro, io ero incaricato di progettare, creare e gestire il database, e quella nebbia di incertezze ha iniziato a diradarsi. L'idea del progetto l'ho trovata molto interessante poiché ci ha permesso di creare qualcosa che si può applicare per un uso reale nella vita di tutti i giorni. Ovviamente ci sono state diverse difficoltà durante tutto il percorso, ma questo mi ha permesso di mettermi alla prova e di valutare le mie capacità. Ho ovviamente imparato alcune nozioni che durante i vari moduli non abbiamo trattato e ciò è molto positivo perché ho avuto l'opportunità di ampliare il mio bagaglio culturale.
