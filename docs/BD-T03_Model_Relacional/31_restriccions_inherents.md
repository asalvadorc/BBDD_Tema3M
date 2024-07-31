# 3.1 Restriccions inherents



Com hem dit són les que imposa el propi model. Algunes són característiques
que han d'acomplir les relacions. Per tant no qualsevol taula matemàtica és
una relació. Podem considerar les següents:

  * **Valors atòmics** : cada valor de la taula, és a dir, qualsevol valor de qualsevol atribut de qualsevol tupla ha de ser simple, no divisible. Per tant no valen atributs compostos o repetitius.

> Així, si considerem **Nom** en la relació **Empleat** com a nom de pila més
> cognoms, no serà divisible (no podré agafar posteriorment el nom de pila per
> una banda i els cognoms per una altra; si ho volguera fer, s'haurien de
> definir els atributs simples **Cognom1** , **Cognom2** i **Nom**).

> Tampoc valen valors repetitius, per exemple un vector de 12 entrades. Queden
> per tant descartats els atributs **_multivaluats_**.

  * **Tuples distintes** : no poden haver dues tuples iguals. Això és una diferència respecte a les taules matemàtiques on sí que es poden duplicar files. 

  

  * **L'ordre de les tuples no és significatiu**. 

  

  * **L'ordre dels atributs no és significatiu**. 


Llicenciat sota la  [Llicència Creative Commons Reconeixement NoComercial
CompartirIgual 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)

