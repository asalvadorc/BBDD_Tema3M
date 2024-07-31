# 1\. Introducció



En 1970 **E.F. Codd** va introduir la teoria matemàtica de les relacions en el
camp dels SGBD. El model de dades que va crear s'anomena **MODEL RELACIONAL**
, amb una base matemàtica (la de les relacions) molt sòlida, on les dades
s'estructuren en forma de relacions (taules) que són estructures de dades
simples i uniformes, que permeten una fàcil comprensió.

En el moment en què va sorgir, els models que funcionaven eren el jeràrquic i
el de xarxa (també anomenat Codasyl, pel grup de treball que va estandaritzar-
lo). Com a model els va superar perquè, com va dir el mateix Codd,
"_proporciona un mitjà per a descriure les dades amb la seua estructura
únicament, sense haver de superposar cap estructura addicional per a
representar-se en la màquina " _(és a dir, sense punters ni històries).

A pesar d'això va estar uns anys en competència amb aquells, amb molta gent
molt reticent, ja que els productes comercials que eixien no eren
suficientment eficients, potser perquè la tecnologia de l'època no ho
permetia. A partir dels anys 80, quan la tecnologia ho va permetre, van eixir
productes millors, com per exemple l'**ORACLE** (1979), i aleshores la seua
implantació va ser aplastant.

Els objectius del Model Relacional són:

  * **Fidelitat** , per a originar esquemes que representen fidelment la informació (els objectes i relacions entre ells) que existeix en el domini del problema.
  

  * **Independència física**[1], per a que la manera de guardar les dades no influesca en la seua manipulació lògica, i així els usuaris que accedeixen a aquestes dades no hagen de modificar els seus programes per canvis en l'emmagatzematge físic.
  

  * **Independència lògica** , per a que les vistes externes no es vegen afectades per canvis en l'esquema conceptual de la B.D.
  

  * **Flexibilitat** , per a poder oferir les dades a cada usuari de la forma més adequada a la seua aplicació.
  

  * **Uniformitat** , les estructures lògiques de les dades presenten un aspecte simple i uniforme (les taules), cosa que facilita la concepció i manipulació per part dels usuaris.
  

  * **Senzillesa** , les característiques anteriors, unides a uns llenguatges d'usuari senzills, fan que el M. Relacional siga fàcil d'entendre i d'utilitzar per l'usuari final.

Recordeu que les **relacions** del Model Relacional són les **taules**. No són
el mateix que les relacions del Model Entitat-Relació. Per evitar confusions
intentarem anomenar-les sempre taules.  

* * *

[1]En realitat tant la independència física com lògica les han intentades aconseguir tots els
models.


Llicenciat sota la  [Llicència Creative Commons Reconeixement NoComercial
CompartirIgual 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)

