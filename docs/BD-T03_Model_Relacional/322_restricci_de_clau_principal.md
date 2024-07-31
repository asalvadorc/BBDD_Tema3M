# 3.2.2 Restricció de clau principal

Permet declarar un atribut o un conjunt d'atributs com a **CLAU PRINCIPAL** o
**PRIMÀRIA** (Primary Key). Aquesta clau principal servirà per a identificar
unívocament cadascuna de les files.

Com a conseqüència de l'anterior, la clau principal no podrà agafar valors
nuls ni repetits, ja que en cas contrari no es podria assegurar la
identificació de les files.

Aquestes últimes característiques també les podran tenir altres atributs, cosa
que dóna lloc als tipus de restricció que es veuen en els següents punts.

Nosaltres sempre definirem una clau principal. Si tenim claus candidates,
triem una d'elles com a clau principal. Si no en tenim, ens inventem un camp
que servirà de clau principal (bé un número o bé un codi alfanumèric).

No és convenient que la clau principal estiga formada per un número excessiu
de camps. Podríem dir que 3 és el màxim. Si la clau candidata està formada per
més de 3 camps, o bé triem una altra clau candidata, o bé ens inventem una.

En **Access** es marca la clau principal amb una figura d'una clau. En la
figura es veu com fer que el camp **dni** siga la clau principal de la taula
**EMPLEAT** :

![](T3_3_2_2.png)

En **LibreOffice Base** es fa de la mateixa manera:

![](T03_3_2_2_2.png)



Llicenciat sota la  [Llicència Creative Commons Reconeixement NoComercial
CompartirIgual 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)

