# Contribucions

El CiviCRM incorpora un mòdul de contribucions que permet gestionar les contribucions financeres de l'organització. El mòdul s'integra amb altres components de l'eina i per això permet gestionar també els pagaments dels esdeveniments i de les pertinences de l'organització.

## Estats de pagament

Quan es registra una contribució, bé sigui manualment o bé automàticament a través d'algun procés que ho permeti, s'associa un estat de pagament en aquesta contribució.

Podríem classificar els estats de pagament de les contribucions en funció de **(1)** *si es troben en procés o requereixen encara d'alguna acció per donar-les per tancades*

- **Pendent** - S'ha sol·licitat fer el pagament més tard o bé no s'ha rebut resposta del processador de pagaments utilitzat.
- **Pendent de reembossament** - Cal fer el reembossament de la contribució.
- **Parcialment pagat** - S'ha fet un pagament parcial de la contribució.
- **Vençut** - Ja s'hauria d'haver completat el pagament de la contribució.
- **En curs** - Quan ja s'ha realitzat el primer pagament d'un compromís (CiviPledge) i encara en queden per completar-lo.

o **(2)** *si són contribucions que ja no requereixen cap més acció i per tant podem donar per tancades*

- **Completat** - Pagament rebut satisfactòriament.
- **Cancel·lat** - Ja no s'espera rebre el pagament corresponent a la contribució.
- **Fallit** -  El processador de pagament ha retornat un error en processar el pagament de la contribució.
- **Reembossat** - Devolució del pagament de la contribució per part de l'organització.
- **Retrocedit** - Retrocés de la transacció del pagament de la contribució per part de l'entitat emissora de la targeta.
