# Grups

Definirem una jerarquia de grups que ens ajudi a segmentar els contactes de voluntariat per facilitar processos com la cerca d'informació, comunicació per mailing i generació d'informes entre d'altres.

* **Voluntariat**

    * **Voluntaris – actius** (grup intel·ligent)

        Criteri del grup – Existeix almenys una relació activa de voluntariat entre el voluntari i l'organització.

    * **Voluntariat – puntual** (grup intel·ligent)

        Criteri del grup – Persones que han participat com a voluntaris a esdeveniments de l'entitat sense tenir o haver tingut cap relació de voluntariat activa.

    * **Voluntaris – històric** (grup intel·ligent)

        Criteri del grup – No existeix cap relació activa i existeix almenys una relació inactiva de voluntariat entre el voluntari i l'organització.


    * **Interessats en voluntariat pendents de contactar/benvinguda** (grup intel·ligent)

        Criteri del grup – La persona té una activitat "[Voluntariat] Persona interessada" amb estat de l'activitat com a `Pendent de revisar` o `Pendent de contactar`.

    * **Interessats en voluntariat pendents d'incorporar** (grup intel·ligent)

        Criteri del grup – La persona té una activitat "[Voluntariat] Sessió o Entrevista d'acollida i valoració" amb estat de l'activitat com a `Pendent de revisar`.

    * **Interessats en voluntariat (no voluntaris)** (grup intel·ligent)

        Criteri del grup – La persona té una activitat "[Voluntariat] Persona interessada" amb estat de l'activitat com a "Completada" i no ha arribat a ser voluntària de l'entitat (no té el subtipus de contacte Voluntari).

    * **Persones amb entrevista o sessió d'acollida de voluntariat** (grup intel·ligent)

        Criteri del grup – La persona té una activitat "[Voluntariat] Sessió o Entrevista d'acollida i valoració".

    * **Interessats en voluntariat (no voluntaris) sense activitat acollida** (grup intel·ligent)

        Criteri del grup – Persones que es troben en el grup "Interessats en voluntariat (no voluntaris)" però no en el grup "Persones amb entrevista o sessió d'acollida de voluntariat"


* **\# per a cada grup corresponent a un programa de l'organització**

    * **Voluntaris del programa** – actius (grup intel·ligent)

        Criteri del grup – Existeix almenys una relació activa de voluntariat entre el voluntari i l'organització vinculada al programa.

    * **Voluntaris del programa – històric** (grup intel·ligent)

        Criteri del grup – No existeix cap relació activa i existeix almenys una relació inactiva de voluntariat entre la persona i l'organització vinculada al programa.
