# Captació de fons

## Guia d'ús

### Gestió de socis i contribucions recurrents

    **NOTA** - En un futur no gaire llunyà es té previst automatitzar alguns dels
    processos de gestió de socis i contribucions de tal manera que definint una
    pertinença de tipus soci amb un import periòdic associat es vagin generant
    periòdicament les seves respectives contribucions i inclús es puguin generar els fitxers de domiciliació per poder enviar al banc.

Quan no es disposa d'un sistema integrat de gestió de contribucions recurrents,
com per exemple les domiciliacions dels socis de l'entitat, i es desitja mantenir
dins del CRM el registre de contribucions, fer el manteniment manual d'aquest
registre de contribucions es pot convertir en una tasca tediosa.

Per això el CiviCRM ofereix algunes eines que ens poden ajudar a facilitar aquesta
gestió. A continuació descriurem alguns dels processos previstos per a la gestió
de socis i contribucions recurrents.

#### Alta de socis nous

Els socis es defineixen al CiviCRM mitjançant les pertinences.

    **NOTA** - Quan avancem en l'automatització de les domiciliacions definirem
    amb més precissió les pertinences. Per ara només ens hem de preocupar de crear-les i cancel·lar-les quan s'escaigui per reflectir l'estat dels socis (actual i
    històric de l'entitat).

L'alta de socis nous es pot produir per dues vies:

**En línia** per la qual és el mateix soci que mitjançant el formulari de la web
es dona d'alta i es genera un registre al CRM amb la seva corresponent pertinença.

    **NOTA** - Actualment quan un soci es dona d'alta a través de la web es crea un
    contacte al CRM amb les seves dades i una contribució amb estat pendent i tipus financer quota de pertinença. Cal afegir manualment la pertinença com a soci de
    l'entitat.

**Manual** per la qual es crea el contacte en el CRM directament i se li afegeix
la pertinença com a soci.

##### Revisió de contactes duplicats

Quan es produeix una alta de soci a través d'un formulari de la web el CRM sempre
genera un contacte nou amb l'ànim de no trepitjar mai cap dada existent al CRM
i delegant en una posterior revisió la verificació de les dades introduïdes i
la possible combinació de contactes duplicats quan es doni el cas.

#### Baixa de socis

> PENDENT DE DOCUMENTAR

#### Generació de contribucions anuals de socis

**Manual**

Si volem generar una contribució corresponent a la quota de soci d'un contacte
hem d'afegir una contribució amb **tipus financer** 'Quotes de pertinences', definir
la **data de recepció** prevista, l'**import** de la contribució en qüestió i el
**mètode de pagament** 'Domiciliació bancària' a la vegada que definirem l'**estat
de la contribució** actual bé sigui 'Pendent' o bé 'Completat'.

**En lots**

Per tal d'agilitzar l'entrada de les contribucions recurrents vinculades als socis
ens podem valer de l'eina d'**Importació de contribucions** que ens proporciona
el CiviCRM.

D'aquesta manera podem introduir d'una tacada totes les contribucions previstes
per un any dels socis actuals (com a pendents) per posteriorment poder anar
actualitzant el seu estat com a completat a mesura que anem rebent els pagaments
corresponents.

Per importar les contribucions ens caldrà un fitxer CSV amb les següents columnes:

- **Identificador del contacte**
- **Import total**
- **Data de recepció**
- **Estat de la contribució** - valors possibles: *Completed* i *Pending*
- **Tipus financer** - valor per defecte: *Quotes de pertinences*
- **Mètode de pagament** - valor per defecte: *Domiciliació bancària*

Un cop tinguem el fitxer CSV amb les contribucions a importar ja podrem procedir
amb la importació de les contribucions.

> Vegeu [CiviCRM - Guia de l'usuari > Fluxos de treball comuns > Importació de dades
en el CiviCRM](https://docs.civicrm.org/user/ca/latest/common-workflows/importing-data-into-civicrm/) per a més informació de com importar contribucions al CRM.


#### Actualització d'estat de contribucions en bloc

Els pagaments de les contribucions de socis programades i registrades com a pendents
es poden anar actualitzant a mesura que es vagin rebent. Normalment farem
l'actualització un cop al mes quan el banc hagi domiciliat els imports del mes
actual. Per tal de no haver de fer aquesta acció manualment contacte a contacte i
contribució a contribució el CRM ofereix una eina per poder fer aquesta acció en
bloc.

Per fer-ho ens cal cercar les contribucions que volem actualitzar (per exemple les
contribucions de **tipus financer** 'Quotes de pertinences' amb **data de recepció** 'El mes actual' i amb **estat de la contribució** 'Pendent') i utilitzar
l'acció **Actualitza l'estat de les contribucions pendents**.

> Vegeu [CiviCRM - Guia de l'usuari > Contribucions > Cerca i visualització de contribucions](https://docs.civicrm.org/user/ca/latest/contributions/finding-and-viewing-contributions/) per a més informació de com actualitzar l'estat de les contribucions pendents.

## Conceptes clau

### Tipus financers

> Vegeu informació sobre els tipus financers a [CiviCRM - Guia de l'usuari > Contribucions > Conceptes claus i configuracions](https://docs.civicrm.org/user/ca/latest/contributions/key-concepts-and-configurations/#tipus-financers).

- Donatius
- Quotes de pertinences
-

### Estats de contribució

> Vegeu informació sobre els estats de contribució a [CiviCRM > Contribucions](/civicrm/contribucions/#estats-de-pagament).
