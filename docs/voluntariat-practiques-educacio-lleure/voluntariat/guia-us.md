# Guia d'ús

Distingirem dos tipus de voluntariat:

- **Voluntariat recurrent**: És el voluntariat que requereix de la persona un compromís prolongat en el temps i en general vinculat a un programa o activitat de l'entitat. Aquest tipus de voluntariat el definirem mitjançant una relació de voluntariat entre la persona i l'entitat. També es podrà (si es desitja o si pertoca) inscriure a la persona amb el rol de voluntari a l'esdeveniment o esdeveniments dels quals participi.

- **Voluntariat puntual**: És el voluntariat que es fa en una acció puntual i que requereix normalment d'un compromís d'un dia i unes hores per part de la persona voluntària. Aquest tipus de voluntariat el definirem mitjançant la inscripció de la persona com a voluntari en l'esdeveniment (activitat) en qüestió. A diferència dels voluntaris recurrents, el voluntariat puntual no tindrà una relació de voluntariat creada.

## Etapes de voluntariat recurrent

En general, el responsable de voluntariat és el principal encarregat de gestionar o coordinar les diferents etapes de les quals participa el voluntari mentre que el responsable de cada programa de l'organització podrà participar també, si es vol, de les etapes d'Incorporació, Acompanyament i Desvinculació. Aquesta breu guia pretén esboçar el recorregut d'aquestes etapes a través dels casos d'ús que ofereix el CRM.

### Interès

Quan una persona mostra el seu interès en fer de voluntari, es donen les següents accions o bé perquè es generen manualment o bé (en general) perquè es generen quan la persona omple el formulari del web habilitat per aquest propòsit.

* Creació de contacte :bust_in_silhouette: **Persona**
* Nova activitat :hourglass_flowing_sand: **[Voluntariat] Persona interessada** per recollir dades bàsiques de la persona i poder concertar l'entrevista

El responsable de voluntariat rebrà una notificació cada vegada que s'ompli el formulari web i podrà veure en l'informe :bar_chart: **Interessats en voluntariat pendents de revisar/contactar** tots aquells contactes que han entrat i els quals a través de l'estat de l'activitat «[Voluntariat] Persona interessada» o bé resten:

- `Pendent de revisar` - cal revisar la informació entrada i veure si ja existien al CRM i per tant cal fer algun tipus de combinació de contactes. Si tenim diversos contactes per revisar podem fer una [cerca i combinació de contactes](https://docs.civicrm.org/user/ca/latest/common-workflows/deduping-and-merging/) acotada al grup *Interessats en voluntariat pendents de revisar/contactar*.
- `Pendent de contactar` - cal donar una primera resposta a l'interès mostrat per exemple mitjançant l'enviament d'un mail tipus "Benvinguda de voluntariat" agraint el contacte i interès i explicant següents passos o concertant directament alguna entrevista.

Un cop la persona ja està contactada l'estat de l'activitat "*[Voluntariat] Persona interessada*" canviarà a `Completat` i restarà així indefinidament a no ser que la persona expliciti que ja no segueix interessada en fer voluntariat. En aquest darrer cas l'estat de l'activitat canviarà a `Obsolet`.

### Acollida (presentació de l'entitat i/o entrevista) i valoració

Una persona interessada en fer voluntariat pot ser convocada a una sessió informativa de voluntariat o bé directament consultada o entrevistada.

En el primer cas podem fer el seguiment de les sessions informatives mitjançant un tipus d'esdeveniment del tipus  :calendar: **Voluntariat, formació, incidència** on es convidarà a totes les persones que estiguin al grup :busts_in_silhouette: **Interessats en voluntariat (no voluntaris) sense activitat acollida**. Les persones que confirmin la seva assistència se les pot inscriure a l'esdeveniment com a participants. Un cop realitzat l'esdeveniment podrem confirmar (canviant l'estat a la inscripció de l'esdeveniment) les persones que finalment no hagin assistit.

A tots aquells que acabin assistint a la sessió o bé en el cas de ser consultats o entrevistats directament se'ls hi crearà una nova activitat del tipus :hourglass_flowing_sand: **[Voluntariat] Sessió o Entrevista d'acollida i valoració** (ho podrem fer a partir dels resultats d'una cerca sobre l'esdeveniment) per validar i consolidar les dades de l'activitat "*[Voluntariat] Persona interessada*" i recollir-ne de noves per poder valorar la incorporació de la persona com a voluntari de l'organització.

L'estat d'aquesta activitat serà `Pendent de revisar` mentre no es decideixi la seva incorporació o no-incorporació. Quan es decideixi l'estat de l'activitat haurà de quedar com a `Completat`.

### Incorporació

A través de l'informe :bar_chart: **Voluntaris pendents d'incorporar** podem fer el seguiment de totes aquelles persones que han vingut a alguna sessió informativa o bé se'ls ha entrevistat i ha quedat pendent decidir la seva incorporació.

Un cop la persona passa a formar part de l'equip de voluntariat de l'organització, es pot procedir a:

* Afegir a la persona el tipus de contacte :bust_in_silhouette: **Voluntari** i consolidar dades de l'activitat *[Voluntariat] Sessió o Entrevista d'acollida i valoració* en els camps personalitzats del contacte com ara "*Perfil competencial*" i "*Perfil acadèmic i professional*".
* Crear relació voluntariat entre el *Voluntari* i la *Organització*.
* Inscriure al voluntari si correspon a l'esdeveniment oportú amb el rol de participant `Voluntari`.

### Acompanyament

* Crear activitat «Registre de seguiment a voluntaris»

### Desvinculació

* Posar data de finalització a la relació de voluntariat amb l'organització i si s'escau detallar-hi els motius de la desvinculació

## Crides de Voluntariat

Per crides puntuals que calgui cobrir ens podem valer del grup :busts_in_silhouette: **Interessats en voluntariat (no voluntaris)** per establir-hi comunicacions.
