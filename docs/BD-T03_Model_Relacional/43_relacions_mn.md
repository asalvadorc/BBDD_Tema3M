# 4.3 Relacions M:N

Per cada relació **M:N** construirem una **nova taula** on s'inclouran com a
clau externa les claus principals de les dues entitats, i a més la seua
combinació constituirà (o formarà part de) la clau principal. Inclourem també
els possibles atributs de la relació.

En l'exemple:

![](T3_4_3_1.png)

Cada vegada que ens trobem amb una relació M:N i la traduïm per una nova taula
haurem de**preguntar-nos si és suficient amb la clau principal** formada per
les dues claus externes, o si fa falta afegir un altre camp. Hem de ser
conscients que la clau principal no puga repetir-se, que hi haja 2 files amb
la mateixa clau principal. Així, en l'exemple, ens hauríem de fer la següent
pregunta: pot un empleat treballar en el mateix projecte més d'una vegada? En
aquest cas la contestació és negativa, i per tant és suficient amb aquesta
clau principal.

Però suposem que la resposta és que sí que pot treballar més d'una vegada al
llarg del temps. En aquest cas seria una espècie d'històric, on faria falta, a
més, saber quan comença i quan acaba de treballar en un projecte un determinat
treballador (serien atributs de la relació):

![](T3_4_3_2.png)

  
Aleshores, com no és suficient amb la clau principal formada per les dues
claus externes, inclourem un altre camp en la clau principal. Sembla que el
més adequat seria **Data_c** (ja no es pot donar el cas que el mateix
treballador treballe més d'una vegada en el mateix projecte, començant el
mateix dia)

![](T3_4_3_3.png)

Però per una altra banda, les claus principals molt llargues no són
operatives, i encara que la traducció literal siga com hem dit, per motius
pràctics podem canviar la clau principal. Considerarem que el nombre màxim de
camps en la clau principal és de 3. 4 ja són massa, i aleshores buscarem una
altra clau principal (un codi de treball, per exemple). Les claus externes
continuarien sent-ho.



Llicenciat sota la  [Llicència Creative Commons Reconeixement NoComercial
CompartirIgual 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)

