# 4.5 Entitats dèbils

Les entitats dèbils, com que com a mínim depenen d'una altra, podrem ser més
restrictius que les altres. Una entitat sempre és dèbil a través, com a mínim,
d'una relació que la comunica amb l'entitat principal. A més participa de
forma total (com que no pot existir sense l'altra, tota ocurrència està en la
relació).

Per tant, tota entitat dèbil tindrà una clau externa, que apunta a la
principal i serà no nula. Però encara podem anar més enllà:

  * **Dependència en existència** : farem que la clau externa **esborre i actualitze en cascada** , ja que si deixa d'existir la principal no té sentit la dèbil.

  * **Dependència en identificació** : a més d'esborrar i actualitzar en cascada, la clau externa **formarà part de la clau principal**.

> Si la relació per la qual depèn en identificació és 1:N, farà falta un altre
> camp en la clau principal.

> Si és 1:1, amb la clau externa és suficient com a clau principal

En nostre exemple quedarà així:

![](T3_4_5_1.png)


Llicenciat sota la  [Llicència Creative Commons Reconeixement NoComercial
CompartirIgual 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)

