# Rust
+ Si può fare il catch di alcuni panic con catch unwind:
	+ i panic unwind sono panic che risalgono lo stack, questi possono essere catturati e sono quelli generati da panic!()
	+ ci sono panic non catturabili che abortiscono il processo subito come le chiamate ad abort()
+ Any in rust serve a simulare il sub typing 
+ downcast_ref serve a provare a castare un tipo in un sottotipo

# Akka
+ per gestire failure restart più usato di resume

# Raft
+ possiamo simulare la rete localmente con più attori Raft

# Actum
+ in Actum non definiamo attori come enum, ma come funzioni asincrone che prendono i messaggi in arrivo e fanno cose in base al messaggio ricevuto
+ queste funzioni sono spesso composte da un loop che continua ad essere eseguito fino a quando la macchina a stati non deve cambiare stato
+ le variabili associate ad uno stato (e solo uno) vanno nella funzione che gestisce quello stato in questo modo vanno fuori di scope da sole quando lo stato cambia


