Bases de Dades


# <a name="main"></a>**4.2 Relacions 1:N**

Per cada relació 1:N entre les entitats **A** i **B**, on **A** és la que participa amb grau de cardinalitat 1, i **B** amb grau N, s'inclou un nou camp en **B** (del mateix tipus que la clau principal de **A**) que a més serà **clau externa** que apuntarà a **A**, més concretament a la clau principal de **A**. En moltes ocasions al camp nou de **B** se li posa el mateix nom que a la clau principal de **A**, però no és necessari, depén del gust de cadascú.

També s'inclouran en **B** tots els possibles atributs de la relació.

La següent animació intenta explicar-ho millor:

Si a més l'entitat que participa amb grau N ho fa de forma **total** (com en la figura de baix), la clau externa **no pot ser nula** (és a dir sempre ha de tenir un valor).

![ref1]

En l'exemple nostre:

- Per la relació **Pertany** (figura de dalt) inclourem l'atribut **departament** a **Empleat**, que a més haurà de ser no nul.
- Per la relació **Controla** inclourem l'atribut **departament** a **Projecte** (no nul).
- Per la relació **Supervisa** inclourem l'atribut **supervisor** a **Empleat** (és reflexiva), però aquest sí que pot ser nul. Encara que semble estrany, un camp pot ser clau externa que apunta a la clau principal de la mateixa taula.
- Per la relació **Té** entre empleat i familiar, inclourem en **FAMILIAR** l'atribut **dni\_e**, però com que Familiar és dèbil la veurem millor un poc més endavant.

![ref2]

[« Anterior](41_entitats.md) | [Següent »](43_relacions_mn.md)

Llicenciat sota la [Llicència Creative Commons Reconeixement NoComercial CompartirIgual 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)
**Created with an evaluation copy of Aspose.Words. To discover the full versions of our APIs please visit: https://products.aspose.com/words/**

[ref1]: 42_relacions_1n.002.png
[ref2]: 42_relacions_1n.003.png
