Bases de Dades


# <a name="main"></a>**4.6 resum dependències**

Anem a fer un quadre resum amb distints graus de dependència entre dues relacions i com es traduiria al Model Relacional: 

![ref1]

Per una altra banda, si ens trobem una entitat dèbil que depèn en identificació a través d'una relació 1:1, és suficient amb la clau principal de A com a clau principal de B 

![ref2]







Una altra qüestió que pot dur a confusió és el cas de les claus externes formades per 2 camps. Ens basarem en l'exemple de sempre, en la taula FAMILIAR, ja que té una clau principal formada per 2 camps. Suposem que hi ha en el Model Entitat-Relació una taula que depèn d'ella, com podria ser comunicacions que se li han fet (cartes). Les entitats i la relació entre elles podria ser aquesta: 

![ref3]

Com que la relació és de tipus 1:N la traduirem per una clau externa en CARTES. I quina serà la clau externa? Com que la taula FAMILIAR té una clau principal formada per 2 camps, haurem de posar una clau externa formada per 2 camps. Alerta! no seran 2 claus externes, sinó una clau externa formada per 2 camps. Com sempre, representarem la clau externa amb un doble subratllat, que ara agafarà als 2 camps. 

![ref4]

[« Anterior](45_entitats_dbils.md) | [Següent »](47_relacions_ternries.md)

Llicenciat sota la [Llicència Creative Commons Reconeixement NoComercial CompartirIgual 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)
**Created with an evaluation copy of Aspose.Words. To discover the full versions of our APIs please visit: https://products.aspose.com/words/**

[ref1]: 46_resum_dependncies.002.png
[ref2]: 46_resum_dependncies.003.png
[ref3]: 46_resum_dependncies.004.png
[ref4]: 46_resum_dependncies.005.png
