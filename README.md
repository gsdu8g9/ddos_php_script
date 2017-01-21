# ddos_php_script

Lo script serve per fare un DDoS UDP flood in PHP

## Come usarlo

Da web server (visita la pagina):

`http://127.0.0.1/ddos.php?pass=apple&host=TARGET&port=PORTA&time=SECONDI&packet=NUMBERO&bytes=NUMBERO`

Da terminale:

`php ./ddos.php host=TARGET port=PORTA time=SECONDI packet=NUMBERO bytes=NUMBERO`

## Parametri

<pre>Aiuto:	Stampa questa pagina ti servira'
host	RECHIESTO specifico IP o HOSTNAME
pass	RECHIESTO selo se utilizzato da webserver
port	OPZIONALE se non specificato verranno utilizzate porte casuali
time	OPZIONALE secondi per tenere attivo il DDoS,necessari se il pacchetto non viene utilizzato
packet	OPZIONALE numero di pacchetti da inviare al target, richiesto se il time non viene specificato
bytes	OPZIONALE dimensioni del pacchetto da inviare, defualt: 65000
format	OPZIONALE formato output , (text,json,xml), default: text
output	OPZIONALE logfile, salva output in un  file
verbose	OPZIONALE 0: debug, 1:info, 2:notice, 3:warning, 4:error, default: info

Nota: 	Se both time e packet sono specificati,solo time sara' utilizzato
</pre>

## Requisiti
- PHP 5.4 versione o successivi

## Crediti

* [@HackPerTutti](https://t.me/hackpertutti) is the creator of the project

## Licensa

GNU General Public License version 2.0 (GPLv2)

