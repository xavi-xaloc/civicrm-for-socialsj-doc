# Permisos

CiviCRM permet definir diferents nivells d'accés a les dades per als diferents tipus d'usuaris que l'han d'utilitzar.
Aquests diferents nivells d'accés es corresponen a diferents rols que s'assignen a uns grups d'usuaris.
En el nostre cas hem definit dos rols principals assignats als grups tècnics administradors i tècnics CIE
respectivament:

## Rol tècnic administrador

El tècnic administrador té la capacitat de fer qualsevol acció i visualitzar totes les dades de la plataforma exceptuant aquells estrictament relacionats amb la configuració i administració del CiviCRM.

## Rol tècnic CIE

El tècnic CIE, pel contrari, només està capacitat per operar amb aquells contactes estrictament lligats al programa CIE.
En el següent full de càlcul es defineixen amb més detall els permisos assignats a cada rol tant a nivell de CiviCRM (més específics) com a nivell de Drupal (més genèrics):

| Drupal Permissions                       |     usuari anonim       | usuari autenticat  | tècnic administrador | tècnic CIEs |
|:---------------------------------------- |:-----------------------:|:------------------:|:--------------------:|:-----------:|
| CiviCRM: Afegir contactes                |            No           |         No         |           Si         | No |
| CiviCRM: Visualitzar tots els contactes  |            No           |         No         |           Si         | No |
| CiviCRM: Editar tots els contactes       |            No           |         No         |           Si         | No |
| CiviCRM: Eliminar contactes              |            No           |         No         |           Si         | Si |
| CiviCRM: Accés als contactes eliminats   |            No           |         No         |           Si         | No |
| CiviCRM: Importar contactes              |            No           |         No         |           Si         | No |
| CiviCRM: Editar grups                    |            No           |         No         |           Si         | No |
| CiviCRM: Administrar el CiviCRM          |            No           |         No         |           No         | No |
| CiviCRM: Accés als arxius pujats        |            Si           |         Si         |           Si         | Si |
| CiviCRM: Fitxes de perfil i formularis   |            No           |         No         |           No         | No |
| CiviCRM: Fitxes de perfil                |            No           |         No         |           No         | No |
| CiviCRM: Crear un perfil                 |            No           |         No         |           Si         | No |
| CiviCRM: Editar un perfil                |            No           |         No         |           Si         | No |
| CiviCRM: Visualitzar un perfil           |            No           |         No         |           Si         | No |
| CiviCRM: Accedir a totes les dades personalitzades |  No           |         No         |           Si         | No |
| CiviCRM: Visualitzar totes les activitats |           No           |         No         |           Si         | No |
| CiviCRM: Eliminar activitats             |            No           |         No         |           Si         | Si |
| CiviCRM: Accés al CiviCRM                |            No           |         No         |           Si         | Si |
| CiviCRM: Accés al tauler del contacte    |            No           |         No         |           Si         | Si |
| CiviCRM: Traduir el CiviCRM              |            No           |         No         |           No         | No |
| CiviCRM: Administrar grups reservats     |            No           |         No         |           Si         | No |
| CiviCRM: Administrar Tagsets             |            No           |         No         |           Si         | No |
| CiviCRM: Administrar etiquetes reservades |           No           |         No         |           Si         | No |
| CiviCRM: Administrar normes de deduïts   |            No           |         No         |           Si         | No |
| CiviCRM: Fusionar contactes duplicats    |            No           |         No         |           Si         | No |
| CiviCRM: Veure sortida de depuració      |            No           |         No         |           No         | No |
| CiviCRM: Visualitzar totes les notes     |            No           |         No         |           Si         | No |
| CiviCRM: Accedir a l'API d'AJAX          |            No           |         No         |           No         | No |
| CiviCRM: Accedir als camps de referència del contacte |    No      |         No         |           No         | No |
| CiviCRM: Crear un lot manual             |            No           |         No         |           No         | No |
| CiviCRM: Editar lots de manuals propis   |            No           |         No         |           No         | No |
| CiviCRM: Editar tots els lots de manuals |            No           |         No         |           No         | No |
| CiviCRM: Visualitzar lots de manuals propis   |       No           |         No         |           No         | No |
| CiviCRM: Visualitzar tots els lots de manuals |       No           |         No         |           No         | No |
| CiviCRM: Esborrar lots de manuals propis   |          No           |         No         |           No         | No |
| CiviCRM: Esborrar tots els lots de manuals |          No           |         No         |           No         | No |
| CiviCRM: Exportar lots de manuals propis   |          No           |         No         |           No         | No |
| CiviCRM: Exportar tots els lots de manuals |          No           |         No         |           No         | No |
| CiviEvent: Accedir al CiviEvent            |            No           |         No         |           Si         | No |
| CiviEvent: Editar participants de l'esdeveniment |      No           |         No         |           Si         | No |
| CiviEvent: Editar tots els esdeveniments   |            No           |         No         |           Si         | No |
| CiviEvent: Registrar-se per esdeveniments  |            Si           |         Si         |           Si         | Si |
| CiviEvent: Veure informació dels esdeveniments  |       Si           |         Si         |           Si         | Si |
| CiviEvent: Veure participants de l'esdeveniment |       No           |         No         |           Si         | No |
| CiviEvent: Esborrar al CiviEvent           |            No           |         No         |           Si         | No |
| CiviContribute: Accedir al CiviContribute  |            No           |         No         |           Si         | No |
| CiviContribute: Editar contribucions       |            No           |         No         |           Si         | No |
| CiviContribute: Fer contribucions online   |            No           |         No         |           No         | No |
| CiviContribute: Esborrar al CiviContribute |            No           |         No         |           Si         | No |
| CiviMail: Accedir al CiviMail              |            No           |         No         |           No         | No |
| CiviMail: Accedir a les pàgines de subscripció/anul·lació de CiviMail |         Si         |        Si        |       Si       | Si |
| CiviMail: Esborrar al CiviMail             |            No           |         No         |           No         | No |
| CiviMail: Veure contignut públic al CiviMail |          No           |         No         |           No         | No |
| CiviReport: Accedir al CiviReport          |            No           |         No         |           Si         | Si |
| CiviReport: Accedir al Report Criteria     |            No           |         No         |           Si         | Si |
| CiviReport: Administrar informes reservats |            No           |         No         |           Si         | No |
| CiviReport: Administrar informes           |            No           |         No         |           Si         | No |


| Rol            |     Descripció permís              | Operació      | Tipus de dades                               | Objecte                     |
|:---------------|:---------------------------------- |:------------- |:-------------------------------------------- |:--------------------------- |
|Tècnic CIE      | Edita Programa CIEs                | Edita         | Un grup de contactes                         | Interns CIE                 |
|Tècnic CIE      | Edita visites CIE                  | Edita         | Un conjunt de camps de dades personalitzades | Visites CIE                 |
|Tècnic CIE      | Edita visites grupals              | Edita         | Un conjunt de camps de dades personalitzades | Visites grupals             |
|Tècnic CIE      | Edita entrada i arrelament         | Edita         | Un conjunt de camps de dades personalitzades | Entrada i arrelament        |
|Tècnic CIE      | Edita detenció i internament       | Edita         | Un conjunt de camps de dades personalitzades | Detenció i internament      |
|Tècnic CIE      | Edita nacionalitat i documentació  | Edita         | Un conjunt de camps de dades personalitzades | Nacionalitat i documentació |
|Tècnic CIE      | Gestiona perfil de nou intern CIE  | All           | Un perfil                                    | Nou intern CIE              |
