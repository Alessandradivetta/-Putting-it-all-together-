# Putting it all together
Scopri come tutti i singoli componenti del web lavorano insieme per dare accesso ai tuoi siti web preferiti.

# Load Balancers
Il bilanciatore di carico (o load balancer) è una componente di infrastruttura che distribuisce in modo intelligente il traffico in ingresso tra più server per garantire che nessun server venga sovraccaricato. Questo è particolarmente utile quando il traffico di un sito web o di un'applicazione è molto intenso o quando la disponibilità e la resilienza del sistema sono cruciali.

Funzioni principali di un bilanciatore di carico:
Distribuire il traffico: Un bilanciatore di carico assicura che le richieste degli utenti vengano suddivise in modo equilibrato tra i server backend. Questo non solo migliora le prestazioni, ma consente anche di utilizzare le risorse in modo più efficiente.
Gestire la disponibilità e il failover: Quando un server si guasta o non è più in grado di gestire correttamente le richieste, il bilanciatore di carico può smettere di indirizzare traffico verso quel server, garantendo che il traffico venga reindirizzato ai server funzionanti. Questo processo è supportato dal controllo dello stato di salute (health checks), che monitora costantemente le performance dei server.
Un bilanciatore di carico utilizza diversi algoritmi per determinare come distribuire il traffico tra i server. Alcuni dei più comuni includono:
round-robin che invia la richiesta a ciascun server a turno, Weighted Round-robin che controlla quante richieste sta gestendo un server e la invia al server meno occupato.
I bilanciatori di carico eseguono anche controlli periodici con ogni server per assicurarsi che funzionino correttamente; questo è chiamato "health check". Se un server non risponde in modo appropriato o non risponde, il bilanciatore di carico interrompe l'invio di traffico finché non risponde di nuovo in modo appropriato.

# CDN (Content Delivery Networks)
Un CDN può essere una risorsa eccellente per ridurre il traffico su un sito web molto trafficato. Permette di ospitare i file statici del vostro sito web, come JavaScript, CSS, immagini e video, e di ospitarli su migliaia di server in tutto il mondo. Quando un utente richiede uno dei file ospitati, la CDN individua il server fisicamente più vicino e invia la richiesta lì, invece che potenzialmente dall'altra parte del mondo.

# WAF (Web Application Firewall)
Un WAF si colloca tra la richiesta web e il server web; il suo scopo principale è proteggere il server web da attacchi di hacking o denial of service. Analizza le richieste web per verificare le tecniche di attacco più comuni e se la richiesta proviene da un browser reale piuttosto che da un bot. Inoltre, controlla se viene inviata una quantità eccessiva di richieste web utilizzando un sistema chiamato rate limiting, che consente solo un certo numero di richieste da un IP al secondo. Se una richiesta è considerata un potenziale attacco, viene eliminata e non viene mai inviata al server web.


