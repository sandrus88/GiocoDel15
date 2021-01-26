# Gioco Del Quindici

## Il Gioco

Il gioco del quindici e' un rompicapo classico creato nel 1874 da Noyes Palmer Chapman, postino in servizio a Canastota, e popolarizzato nel 1880 da Samuel Loyd. 
Il gioco consiste di una tabellina di forma quadrata, solitamente di plastica, divisa in quattro righe e quattro colonne (quindi 16 posizioni), su cui sono posizionate 15 tessere quadrate, numerate progressivamente a partire da 1. 
Le tessere possono scorrere in orizzontale o verticale, ma il loro spostamento e' ovviamente limitato dall'esistenza di un singolo spazio vuoto. 
Lo scopo del gioco e' riordinare le tessere dopo averle "mescolate" in modo casuale (la posizione da raggiungere e' quella con il numero 1 in alto a sinistra e gli altri numeri 
a seguire da sinistra a destra e dall'alto in basso, fino al 15 seguito dalla casella vuota).
 
![Gioco Del Quindici risolto](./doc/giocoGelQuindiciWikipedia_risolto.png)

## Linguaggio di programmazione utilizzato

Ho implementato il gioco descritto sopra usando il linguaggio di prorammazione Java. 
Qui sotto la schermata del gioco.

![Schermata del Gioco](./doc/schermata-gioco.jpg)

## Architettura del gioco
 
Il gioco e' suddiviso in due classi principali. La classe GiocoDel15Controller racchiude la logica del gioco mentre la classe GiocoDel15 e' la classe java responsabile per i componenti grafici.

![Uml controller](./doc/class-diagram.jpg) ![Front-End layout](./doc/front-end-layout.jpg)
 
In sintesi l'implementazione del gioco e' la seguente:</br>
Ad ogni click del bottone verifico:</br>
- 1) Se e' adiacente al bottone vuoto.</br>
- &nbsp; 1.A) scambia il bottone cliccato con quello vuoto.</br>
- &nbsp; 1.B) verifico se la combinazione dei numeri e' quella finale</br>
- &nbsp;&nbsp;&nbsp; 1.B.1) a questo punto il gioco si blocca e fa vedere la scritta "HAI VINTO!!!"</br>
- 2) Per ricominciare bisogna cliccare su NuovaPartita.</br>

## Avvio del gioco
Per poter lanciare il gioco scaricare il `jar` nella cartella [GiocoDel15/dist/](./dist) e lanciarlo facendo il doppio click.

## See 


* [Gioco del Quindici](https://it.wikipedia.org/wiki/Gioco_del_quindici) - Descrizione del gioco in Wikipedia