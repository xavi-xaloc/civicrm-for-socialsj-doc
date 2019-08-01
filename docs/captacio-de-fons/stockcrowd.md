# Integració Stockcrowd (EN DESENVOLUPAMENT)

[Strockcrowd](https://www.stockcrowd.com) és una plataforma de captació de fons.
Aquesta plataforma ens permet exportar en el moment que vulguem un llistat amb les
dades dels donatius per a cada campanya que tinguem definida.

En aquesta pàgina establim alguns dels circuits que ens han de permetre importar
aquesta informació al CiviCRM.

## Importació de donants

Un cop ens descarreguem el full de càlcul de la campanya de la qual volem importar
donacions d'Stockcrowd ens caldrà fer d'entrada la següent segmentació.

- Seleccionar les donacions que volem importar (potser ens interessa filtrar a partir d'una data determinada, columna `Fecha Confirmación`).
- Separar les donacions de caràcter **puntual** dels de caràcter **periòdic** (columna `Tipo de donación` que pot ser `Donación puntual` o `Donación periòdica`)
- Separar les donacions de **persones** i **organitzacions** (columna `Tipo de persona` que pot ser `Persona física` de `Persona jurídica`).
- Separar els que volen rebre comunicacions dels que no (columna `Acepta comunicaciones` que pot ser `1` en cas afirmatiu `0` altrament)

### Importació de donants puntuals

Haurem de preparar un CSV de persones i un altre d'organitzacions que contingui
les donacions puntuals que volem importar.

A continuació definim la relació de camps que venen d'Stockcrowd i la seva
correspondència amb els de CiviCRM.

`Fecha de la Transacción` =>

`Número de Pedido` => `Identificació de transacció`

`Importe` =>

`Nombre del Inversor` => `Nom del contacte`

`Apellidos del Inversor` => `Cognoms del contacte`

`Razón Social` => ``

`Teléfono` => Cal separar els telèfons mòbils i fixs en dues columnes

`Correo Electrónico` => `Correu electrònic`

`Dirección Postal` =>

`Código Postal` =>

`Ciudad` =>

`Provincia` =>

`País` =>

`Número de documento` => `NIF` `CIF`

`Acepta comunicaciones` => Afegir al grup butlletí

`Fundraiser` =>

Totes les contribucions han de quedar associades a la campanya i pàgina de contribució corresponent.
