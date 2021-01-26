# GiocoDelQuindici

##Abstract
Il gioco del quindici è un rompicapo classico creato nel 1874 da Noyes Palmer Chapman, postino in servizio a Canastota, e popolarizzato nel 1880 da Samuel Loyd. Il gioco consiste di una tabellina di forma quadrata, solitamente di plastica, divisa in quattro righe e quattro colonne (quindi 16 posizioni), su cui sono posizionate 15 tessere quadrate, numerate progressivamente a partire da 1. Le tessere possono scorrere in orizzontale o verticale, ma il loro spostamento è ovviamente limitato dall'esistenza di un singolo spazio vuoto. Lo scopo del gioco è riordinare le tessere dopo averle "mescolate" in modo casuale (la posizione da raggiungere è quella con il numero 1 in alto a sinistra e gli altri numeri a seguire da sinistra a destra e dall'alto in basso, fino al 15 seguito dalla casella vuota).

* [Gioco del Quindici risolto](doc/gioco-del-quindici-completo.jpg)

##Implementazione
In questo mio progetto realizzero' un'interfaccia con 16 bottoni quadrati, di cui 15 numerati e colorati di rosso e uno vuoto colorato di blue, disposti su 4 righe e 4 colonne.

* [Schermata di Gioco](doc/schermata-gioco.jpg)
 
Il bottone vuoto permette lo scambio tra i bottoni.
Ho separato la logica dalla parte grafica creando un'altra classe col nome GiocoDel15Controller. Ad ogni click del bottone la classe verifica:</br>
1) Se e' adiacente al bottone vuoto.</br>
2) Se si li scambia.</br>
3) Se hai vinto.</br>
4) Se si appare la scritta "HAI VINTO!!!" e avviene il blocco dei bottoni.</br>
5) Per ricominciare bisogna cliccare su NuovaPartita.</br>

##Regole
E' possibile muovere i bottoni sia in senso orizzontale che verticale, cercando di ordinarli in modo crescente. 

##Scopo
Ordinare i bottoni numerati dal numero 1 al numero 15, partendo dalla posizione in alto a sinistra e finendo in quella in basso a destra. 

##Avvio del gioco
Il gioco si avvia eseguendo il file gioco.jar presente nella cartella dist.

* [Avvio del gioco](dist/giocodel15.jar)