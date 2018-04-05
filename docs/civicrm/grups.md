# Grups

Els grups de contactes són una eina del CiviCRM que permet millorar la categorització, segmentació i cerca de contactes en el sistema.

Hi ha dos tipus de grups: els **grups regulars** que permeten agrupar els contactes manualment; i els **grups intel·ligents** que permeten agrupar els contactes automàticament en funció d'uns criteris definits en una cerca. Igualment, el CiviCRM permet jerarquitzar els grups de tal manera que, un grup pare d'uns altres, està format per la suma de tots els contactes dels seus grups fills.

En el nostre cas utilitzarem els grups per categoritzar contactes, per facilitar-ne la cerca en els camps personalitzats de contactes de referència i perquè ens serveixin per regular-hi l'accessibilitat a la informació per part dels usuaris del CRM.

## Grups dels programes de l'entitat

Per tal de poder segmentar millor els contactes i poder fer cerques i informes sobre els diferents programes de l'entitat habilitarem un seguit de grups per a cada programa i, en general, ho farem de la següent manera i seguint la següent jerarquia:

- \#Nom del programa
    - Nom del programa (curs)
        - Tipus d'esdeveniment (curs) - opcional
            - Nom del tipus de contacte usuari del programa - Nom del tipus d'esdeveniment del programa (curs) (grup intel·ligent)
            - Nom del tipus de contacte usuari del programa - Nom del tipus d'esdeveniment del programa (any) (grup intel·ligent)

La idea és preparar un grup intel·ligent per a cada tipus d'esdeveniment per poder categoritzar tots els contactes usuaris que hi participen.

En general, els criteris de cerca que utilitzarem per definir els grups intel·ligents seran els següents:

- Subtipus de contacte
- Tipus d'esdeveniment
- Interval de dates de l'esdeveniment
- Estat del participant en l'esdeveniment = *Inscrit*
- Rol del participant en l'esdeveniment = *"Rol usuari"*

D'aquesta manera només ens haurem de preocupar de definir aquests grups cada curs i, a mesura que anem inscrivint els usuaris als esdeveniments, aquests quedaran categoritzats automàticament en els grups.

## Grups de l'entitat i xarxa de contactes

- \#Entitat
    - Patronat
        - Patrons - actius *(grup intel·ligent)*
        - Patrons - històric *(grup intel·ligent)*
    - Equip professional
        - Equip professional - actius *(grup intel·ligent)*
        - Equip professional - històric *(grup intel·ligent)*
    - Comptabilitat i captació de fons
        - Socis
        - Donants
        - Finançadors
    - Professionals externs
    - Proveïdors
        - ​Empreses
        - Professionals autònoms
- \#Xarxa de contactes

## Grups per a contactes de referència

- **Treballadors** (grup intel·ligent per contacte de referència en relació realitza pràctiques)
    - contactes treballadors actius
    - contactes treballadors - històric

## Grups per a l'accessibilitat a la informació

- Control d'accés
    - **Tècnics administradors** (grup assignat al rol tècnic administrador)
