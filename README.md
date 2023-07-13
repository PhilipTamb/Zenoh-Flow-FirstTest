# Zenoh-Flow-FirstTest

in zenoh-flow abbiamo un file yaml principale chiamato ad esempio data-flow.yaml che è quello che dice al nostro Zenoh Flow Deamon come configuarare la nostra rete.
Infattidentro questo file .yaml ci sono specificati i nodi, i loro input e output e i link che questi nodi hanno nella nostra configurazione zenoh flow.

poi per ogni nodo specificato nel file .yaml della configurazione abbiamo una cartella dove troviamo:
Cargo.toml
src                        →  cartella
nome-nodo.yaml  → dove viene specificato dove si trova il codice del nodo “lib.sr”, ovvero lo specifico codice che verrà eseguito dal nodo e ne caratterizzerà il comportamento. questo file specifica anche input ed output del nodo che devono essere coerenti con la descrizione del file “data-flow.yaml”

src è una cartella dentro la quale troviamo il file di configurazione del nodo, che sarà la libreria del nostro nodo.
questa è caratterizzata da delle funzioni in rust che ne specificano il comportamento.
context
configuration
input
output
