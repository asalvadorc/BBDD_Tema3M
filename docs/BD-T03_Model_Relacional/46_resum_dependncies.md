# 4.6 Resum dependències





Anem a fer un quadre resum amb distints graus de dependència entre dues
relacions i com es traduiria al Model Relacional:

![](T3_4_6_1.png)

Per una altra banda, si ens trobem una entitat dèbil que depèn en
identificació a través d'una relació 1:1, és suficient amb la clau principal
de A com a clau principal de B

![](T3_4_6_2.png)







Una altra qüestió que pot dur a confusió és el cas de les claus externes
formades per 2 camps. Ens basarem en l'exemple de sempre, en la taula
FAMILIAR, ja que té una clau principal formada per 2 camps. Suposem que hi ha
en el Model Entitat-Relació una taula que depèn d'ella, com podria ser
comunicacions que se li han fet (cartes). Les entitats i la relació entre
elles podria ser aquesta:

![](T3_4_6_3.png)

Com que la relació és de tipus 1:N la traduirem per una clau externa en
CARTES. I quina serà la clau externa? Com que la taula FAMILIAR té una clau
principal formada per 2 camps, haurem de posar una clau externa formada per 2
camps. Alerta! no seran 2 claus externes, sinó una clau externa formada per 2
camps. Com sempre, representarem la clau externa amb un doble subratllat, que
ara agafarà als 2 camps.

![](T3_4_6_4.png)


Llicenciat sota la  [Llicència Creative Commons Reconeixement NoComercial
CompartirIgual 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)

