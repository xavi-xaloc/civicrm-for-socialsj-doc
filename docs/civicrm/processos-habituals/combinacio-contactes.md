# Combinació de contactes

El CRM pot tenir contactes duplicats per diversos motius però aquesta circumstància es dona principalment per l'entrada de nous contactes a través de formularis (donatius, butlletí, etc.) i per la falta de verificació prèvia de l'existència d'un contacte abans de crear-lo.

Per fer una revisió a fons de possibles contactes duplicats, el CRM ofereix una **eina de desdupicació**. S'hi pot accedir a través del menú **Contactes > Cerca i combina contactes duplicats**.

En canvi si fem una comprovació de duplicats més específica, persona a persona, aleshores ho farem des dels **resultats d'una cerca**, seleccionant els contactes a combinar i clicant a l'acció **Combina contactes duplicats**.

!!! tip "Indicacions"

    A continuació es llisten algunes indicacions a tenir en compte abans de procedir amb la combinació de dos contactes:

    - En general sempre considerarem com a **contacte original aquell que tingui l'identificador de contacte de CRM més baix**. Aquest serà el contacte que es conservarà. Abans de fer cap combinació haurem de verificar que és així. En cas contrari intercanviarem les posicions del contacte original i el duplicat.

    - No sobreescriurem el camp **Origen** (del contacte) i per tant desmarcarem la casella que per defecte queda seleccionada. En general sempre voldrem conservar des de quin mitjà ha entrat a la nostra base de dades el contacte.

    - Sempre que es pugui és recomanable **previsualitzar ambdós contactes**, p.ex. obrint-los en dues pestanyes noves per poder analitzar visualment cada un dels contactes.

    - A la pantalla de comparació de camps entre els dos contactes a combinar hi ha l'opció `Mostra/oculta files amb la mateixa informació en cada registre de contacte` que permet centrar l'atenció en els camps sobre els quals cal prendre una decisió.

    - Si els dos contactes formen part d'un mateix **grup**, cal tenir en compte que la casella de combinació de grups està marcada per defecte i si no es desmarca, la data d'addició al grup serà sobreescrita amb la del contacte duplicat. Com que en general els grups els utilitzem com a llistes de distribució de mailings aquest comportament ja és acceptable: primarà la darrera data que la persona ens hagi confirmat que vol rebre les comunicacions corresponents al grup.

!!! warning "Atenció"

    Un cop els contactes han estat combinats **el procés no és reversible**.

    No obstant, el contacte combinat i eliminat queda a la paperera de reciclatge per si hi ha hagut algun error o per si es vol revisar alguna dada que sospitem que no ha estat processada.

    En el registre d'activitats del contacte original hi trobarem una activitat del tipus *Contacte combinat* i també registrat l'identificador de CRM del contacte que ha estat combinat i eliminat.


!!! info "Documentació oficial"
    Per a més detall [veure la documentació oficial de CiviCRM](https://docs.civicrm.org/user/ca/latest/common-workflows/deduping-and-merging/)
