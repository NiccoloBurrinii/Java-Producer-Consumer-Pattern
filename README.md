# Java Threads: Producer Consumer

Progetto Java per la gestione di una risorsa condivisa tramite il pattern Produttore-Consumatore.

## Descrizione
Il programma simula lo scambio di dati tra entità diverse utilizzando un buffer monitorato, garantendo che i consumatori non prelevino dati se la risorsa è vuota e i produttori non ne inseriscano se è piena.



## Funzionamento dei Thread:
* **Thread Produttore**: Genera valori casuali e li inserisce nella risorsa condivisa.
* **Thread Consumatore**: Preleva i dati dalla risorsa e li visualizza in console.

Il programma utilizza i metodi `.wait()` e `.notify()` per coordinare l'accesso alla risorsa ed evitare conflitti di sincronizzazione.

## Tecnologie e Concetti
* **Java Core**: Utilizzo della classe `Thread` e della keyword `synchronized`.
* **Sincronizzazione**: Gestione della comunicazione inter-thread (Wait/Notify).
* **Controllo di Flusso**: Utilizzo di flag booleani per l'arresto controllato dei thread dopo un tempo prestabilito.
