# Subnetting4
4 sottoreti

obiettivo:
In questo caso si dovrà creare il piano di indirizzamento per una rete così composta:
- la rete principale è la 172.130.20.0/24
- si vuole fare subnetting in modo da ottenere 4 sottoreti della stessa dimensione

Strumenti utilizzati:
- 1 router con 4 porte
- 8 PC
- 4 switch
- Ciascuna sottorete ha 1 switch e 2 PC, il router permette la comunicazione tra le 4 sottoreti

Conoscenze teoriche: 
Come per due sottoreti per diminuire il traffico in rete ci si affida al subnetting. Quello che cambia in questo caso è il numero di sottoreti e di conseguenza il numero di bit che dovremo prendere dall'hostID per calcolare la subnetmask. Per il resto la configurazione sarà sempre la stessa tenendo presente degli indirizzi per l'identificazione di rete e di broadcast.


Procedimento:
Qua bisogna dividere il numero di ip assegnabili (numero che varia in base alla classe a cui appartiene l'ip) per il numero di sottreti che si vogliono ottnere (4)
per ottnere i range di ip asseganbili. Per la subnetmask invece considerato che 4 = 2^2 dovremo utilizzare due dei bit appartenenti all'hostID. Tenendo presente che saranno due i bit da bloccare nella subnetmask otteniamo, partendo da un'inidrizo di classe C ( con subnet di base di 255.255.255.0), otterremo la seguente :
11111111.11111111.1111111.11000000 -> in decimale: 255.255.255.192. Dopo i calcoli si porcede su filius all'assegnazione degli ip e della subnet ricordando i evitare gli ip che non possiamo utilizzare.


