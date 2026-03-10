# github_action_demo
Demo per una action che fa il deployment di un sito PHP, aggiornando i parametri di connessione al db con quelli di hosting piuttosto che quelli per l'uso locale con xampp.

Per ridurre all'osso l'esempio ci sono due file:

`connessione.php` :  memorizza i parametri di connessione, in locale saranno i classici di xampp localhost,root ... )
quando si fa l'upload devoono essere cambiati con i parametri dell'hosting (es. ftp.altervista miouser passwordftp..)

`index.php`: include il file connessione.php per configurarsi, nella demo stampa i valori (tanto nei secrets sono inventati )

si potrebbe fare a mano ogni volta che faccimo l'upload dal pannello di controllo di altervusta 
ma gli lo facciamo fare a github action...

Happy deployment
