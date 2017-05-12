# Survey Station


## Test

### Protocollo di test

|Test Case      | TC-001                               |
|---------------|--------------------------------------|
|**Nome**       |Spostare dati da dalla tabella sismografo nella tabella shake. |
|**Riferimento**|REQ-003                               |
|**Descrizione**|Quando si chiama la procedura i dati non più vecchi di un determinato valore vengono inseriti dalla tabelle sismografo nella shake.  |
|**Prerequisiti**|Bisogna aver creato la tabella sismografo e shake.|
|**Procedura**     | Si inserisce qualche dato nella tabella sismografo. Si aspettano 2 minuti e si chiama la procedura passandole un Id e come quantitativo dei minuti si inserisce 5.|
|**Risultati attesi** |Nella tabella shake ci devono essere i dati che ho inserito 2 minuti fa. |
