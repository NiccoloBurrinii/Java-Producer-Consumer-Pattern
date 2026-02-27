# Java Producer-Consumer Pattern

Implementazione classica del problema del **Produttore-Consumatore** utilizzando il multithreading in Java.

## ⚙️ Architettura del Progetto
Il progetto dimostra la comunicazione tra thread attraverso una risorsa condivisa, gestendo i problemi di sincronizzazione.



### Componenti principali:
* **Risorsa**: Funge da buffer monitorato. Utilizza i metodi `wait()` per sospendere i thread quando la risorsa è piena/vuota e `notify()` per risvegliarli.
* **Produttore**: Genera valori casuali e li deposita nella risorsa.
* **Consumatore**: Preleva i valori dalla risorsa e li stampa a video.
* **Start**: Classe principale che orchestra l'avvio e l'arresto controllato di 2 produttori e 4 consumatori.

## Concetti Chiave
* **Monitor & Sincronizzazione**: Uso della keyword `synchronized`.
* **Thread Lifecycle**: Gestione dell'avvio (`start`) e della terminazione pulita tramite un flag `running`.
* **Wait/Notify**: Coordinamento degli stati della risorsa per evitare *race conditions*.
