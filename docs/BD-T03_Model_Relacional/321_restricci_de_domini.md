# 3.2.1 Restricció de domini

El valor d'un atribut ha de ser un valor atòmic del domini. Definint clarament
el domini ens assegurem (dins del possible) que l'atribut no puga agafar
valors incorrectes.

Per una banda, el domini serà d'un tipus determinat, triat d'una gamma prou
extensa: enter curt, enter, enter llarg, real, doble precisió, caràcter,
cadena de caràcters (text), data, hora, ...

Així, per exemple, definint el _Sou_ com un número real impedirem que per
error puga agafar el valor 2.**R** 00'00, o que la _data de naixement_ , amb
domini de tipus data, siga 15-**14** -1958 o **31** -**2** -1958.

També es podran definir dominis que estiguen en un determinat interval (nota
d'un examen: 0-10) o d'un tipus enumerat (nota d'avaluació: MD, IN, SUF, BE,
NOT, EXC).

Es poden definir regles de verificació o validació (**CHECK**) que ens ajuden
a perfilar molt bé el domini. Aquest seria un exemple d'exigir que el
treballador tinga de 18 a 65 anys. La sintaxi és inventada, només per a
entendre-ho, amb una hipotètica funció que trau l'any, i una altra que ens
dóna la data d'avui.

CHECK ( Any(avui - data_n) >= 18) and (Any(avui - data_n) < 65) )

> **_Nota_**

> En **Access** la regla de validació seria:

AgregFecha("aaaa";18;[data_n])<=Ahora() Y
AgregFecha("aaaa";65;[data_n])>=Ahora()

> on es veu que la fórmula és afegir 18 anys a la data de naixement i
> comprovar que no supera la data d'avui; i afegir 65 anys a la data de
> naixement i comprovar que sí supera la data d'avui.

Per exemple, **Empleat** podria quedar:

EMPLEAT (_dni_ :caràcter(10), nom:caràcter(30), adreca:caràcter(30),
telefon:enter(9), sou:numèric(6,2), data_n:data)

amb la regla de validació:

CHECK Sou > 0

a banda de la mencionada anteriorment.

Si utilitzem la manera de representar alternativa, ho tindríem així:

![](T3_3_2_1_0.png)

La següent imatge mostra com es faria en **Access** la primera regla de
validació, aplicada al camp **data_n**

![](T3_3_2_1.png)

**_Nota_**

En Base de LibreOffice resulta més complicada la creació de regles de
validació. S'ha de fer per mig de Macros associades a formularis



Llicenciat sota la  [Llicència Creative Commons Reconeixement NoComercial
CompartirIgual 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)

