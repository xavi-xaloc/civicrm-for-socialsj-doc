# Preguntes més freqüents

## 5 Tips for Writing Charity Newsletters with CiviCRM

En el següent article hi podeu trobar alguns consells interessants per tenir en compte a l'hora d'elaborar un butlletí de correu electrònic amb el CiviCRM:

[5 Tips for Writing Charity Newsletters with CiviCRM](http://whitefusemedia.com/blog/5-tips-writing-charity-newsletters-civicrm?utm_content=bufferd9b38&utm_medium=social&utm_source=twitter.com&utm_campaign=buffer)

## Personalització de la correspondència mitjançant tokens

Tant amb la composició de correus electrònics des del mòdul CiviMail, com des de la composició de correus electrònics i correus postals que incorpora per defecte el CiviCRM, es poden utilitzar un seguit de tokens que permeten redactar correspondència a més d'un destinatari incloent-hi de manera automàtica valors propis de cada destinatari.

Alguns d'aquests tokens són: contact.first_name (Nom del contacte); contact.last_name (Cognoms del contacte)

No obstant aquesta personalització no permet aprofitar tota la informació intrínseca del contacte, com per exemple fer la salutació en funció del gènere del contacte. Per fer-ho s'ha habilitat una funcionalitat que permet utilitzar els tokens de manera més avançada. Veiem a continuació diferents exemples:

### Salutació

#### bàsica
 > Estimat/da Joan,

``{contact.email_greeting} {contact.first_name},``

### avançada

> Estimat Joan, o Estimada Joana

``{if {contact.gender} == Male}Estimat {elseif {contact.gender} == Female}Estimada {/if} {contact.first_name},``
