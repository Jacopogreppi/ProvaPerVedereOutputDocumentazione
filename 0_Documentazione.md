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
|**Prerequisiti**|Bisogna aver creato la tabella sismografo e shake e la procedura storePreviousValues.|
|**Procedura**     |In sismografo si inseriscono dei valori non interessanti. Successivamente si inserisce un valore interessante e dopo altri dati di cui valore non è importante. |
|**Risultati attesi** |Nella tabella shake ci devono essere i dati a partire da quando c'è stato il picco. |
