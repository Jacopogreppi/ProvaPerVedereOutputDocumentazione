# Survey Station


## Implementazione

### Database
Una volta terminata la progettazione del database bisogna implementare/mettere in pratica ciò che si è fatto in maniera teorica. Come primissimo passo ho iniziato a scrivere il codice sql delle tabelle presenti sul database dato che senza di esse non è possibile lavorare. 
<br>
<img src="prime 2 tabelle.PNG" />
<br>
L'immagine qui sopra rappresenta il codice che ho ideato e scritto per la creazione delle tabelle "utenti" e "configurazione". La struttura delle linee è la classica di quando si crea una semplicissima tabella. Una piccola particolarità è l'attributo "unique" nel campo "email". Dato che quest'ultimo è la chiave primaria e che non ci saranno mai due indirizzi email uguali tra di loro, ho fatto in modo che queste restrizioni vengano rispettare tramite quell'attributo.
<br>
<br>
<img src="altre 2 tabelle.PNG" />
<br>
L'immagine appena inserita mostra il codice sql che ho scritto per la creazione delle tabelle "sismografo" e "shake". Potrebbe saltare subito all'occhio il fatto che non sono collegate tra di loro tramite delle foreign key. Ciò non è una dimenticanza o un errore di progettazione, ma semplicemente riflettendo sulla situazione che si è presentata, sono giunto alla conclusione che non fosse necessario relazionarle.
<br>
<br>
COSE
<br>
<img src="conf.PNG" />
<br>
