# Mòdul Xarxa d'Hospitalitat

Dependències amb d'altres mòduls:

- Mòdul adults
- Mòdul de voluntariat

## Contactes

> Vegeu més informació sobre els contactes a [CiviCRM > Contactes](/civicrm/contactes/).

Crearem un nou tipus de contacte llar que ens permetrà identificar un dels 3 actors que conformen el mòdul de Xarxa d'Hospitalitat. Els altres dos tipus de contactes _Persona migrant_ + _Adult_ i _Voluntari_ ja queden definits per les dependències del mòdul Xarxa d'Hospitalitat.

### Persones

- **Adult**

 > Vegeu a [Mòdul adults > Contactes](/adults/contactes/#persones)

- **Persona migrant**

 > Vegeu a [CiviCRM > Contactes](/civicrm/contactes/#persones)

- **Voluntari**

 > Vegeu a [CiviCRM > Mòdul voluntariat, pràctiques i educació en el lleure > Voluntariat > Contactes](/voluntariat-practiques-educacio-lleure/voluntariat/contactes/#voluntariaria).

### Llars

- **Llar d'acollida:** Llar implicada en l'acollida de persones migrants.

## Activitats

### [Xarxa Hospitalitat] Seguiment

#### Camps personalitzats - Seguiment Xarxa Hospitalitat

* **Àmbit**

    Selecció múltiple - Acompanyament, Acollida

* **Observacions**

    Resposta oberta

## Relacions

### Relació d'acompanyament Xarxa d'Hospitalitat

- Contacte A: Voluntari
- Contacte B: Persona migrant
- Relació A>B: acompanya en Xarxa d'Hospitalitat a
- Relació B>A: és acompanyat en Xarxa d'Hospitalitat per

### Relació d'acollida en llar de Xarxa d'Hospitalitat

- Contacte A: Persona migrant
- Contacte B: Llar d'acollida
- Relació A>B: és acollida en Xarxa d'Hospitalitat a
- Relació B>A: acull en Xarxa d'Hospitalitat a

### Relació de voluntariat

> Vegeu a [CiviCRM > Mòdul voluntariat, pràctiques i educació en el lleure > Voluntariat > Relacions](/voluntariat-practiques-educacio-lleure/voluntariat/relacions/#es-voluntariaria-a-te-de-voluntariaria-a).

## Grups

> Vegeu més informació sobre els grups a [CiviCRM > Grups](/civicrm/grups/).

El mòdul definirà per defecte la següent jerarquia de grups:

- **Xarxa d'Hospitalitat**

    - **Llars d'acollida en Xarxa d'Hospitalitat - actives (grup intel·ligent)**
    - **Llars d'acollida en Xarxa d'Hospitalitat - històriques (grup intel·ligent)**
    - **Voluntaris d'acollida en Xarxa d'Hospitalitat - actius (grup intel·ligent)**
    - **Voluntaris d'acollida en Xarxa d'Hospitalitat - històrics (grup intel·ligent)**
    - **Voluntaris d'acompanyament en Xarxa d'Hospitalitat - actius (grup intel·ligent)**
    - **Voluntaris d'acompanyament en Xarxa d'Hospitalitat - històrics (grup intel·ligent)**
    - **Persones acollides en Xarxa d'Hospitalitat - actius (grup intel·ligent)**
    - **Persones acollides en Xarxa d'Hospitalitat - històric (grup intel·ligent)**
