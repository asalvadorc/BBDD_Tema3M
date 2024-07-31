# 4.8 Especialitzacions





Aquest aspecte, com en el cas de les relacions 1:1, també té múltiples
solucions. El problema de les especialitzacions és que, encara que de forma
teòrica la solució siga correcta, en la pràctica suposa moltes taules i amb un
cert grau de manteniment entre elles. Per tant, i aplicant el sentit comú,
moltes vegades es fa una simplificació, llevant bé les subclasses, bé la
superclasse, com veurem a continuació. Aquestes són les possibilitats:

  * Transformar les especialitzacions en taules amb la clau principal heretada i els atributs específics (com si substituírem l'especialització en relacions 1:1, amb les subclasses depenent en identificació de la superclasse). Estaria també bé afegir un atribut a la superclasse per a poder saber de quin tipus és. En l'exemple ens quedaria:

![](T3_4_8_1.png)

  * Simplificar les subclasses. Aleshores tots els atributs d'aquestes haurien de passar a la superclasse. També s'haurien de passar totes les relacions que afecten a les subclasses, "retocant" les participacions totals (que ara ja no ho serien). Ara serà obligatori tenir el camp que distingeix el tipus (sinó, perdríem aquesta informació).

![](T3_4_8_2.png)



  * Simplificar la superclasse. Aleshores tots els atributs d'aquesta passarien a cadascuna de les subclasses. També passarien les relacions a cadascuna d'aquestes, "retocant" les participacions totals.

![](T3_4_8_3.png)



Llicenciat sota la  [Llicència Creative Commons Reconeixement NoComercial
CompartirIgual 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)

