# Pràctica 3.2. Disseny del CPD i organització de la seu

## Part inferior del rack

- 3 PC Dell que faran de servidors de la seu
- 1 switch 1U no configurable
- Cables de xarxa i latiguillos
- 7 Adaptadors de xarxa per a les màquines virtuals
- 1 switch TP-Link configurable de 8 ports no enrackable

#### Observacions

- El switch 1U no configurable està connectat al switch cisco troncal i als 3 PC Dell, a través dels adaptadors.
- El switch TP-Link configurable de 8 ports no enrackable està connectat al Mikrotik per un costat i, per l'altre costat, a la DMZ.

## Part central del rack

- 1 Mikrotik que fa de servidor de comunicacions amb l’exterior
- 1 switch Cisco 1U configurable que és el switch trocal de la seu
- Cables de xarxa i latiguillos

#### Observacions

- El Mikrotik està connectat a Internet i al switch Cisco troncal (també està connectat al switch de la DMZ, com hem especificat anteriorment).

## Part superior del rack

- 1 switch TP-Link 1U configurable que és el switch troncal de la 1a planta
- 1 punt d’accés inalàmbric
- Cables de xarxa i latiguillos

#### Observacions

- El switch TP-Link 1U configurable està connectat al switch Cisco troncal i al punt d'accés inalàmbric.

## Fora del rack

- 5 PC per a fer de clients de la xarxa
- 5 monitors, 5 teclats i 5 ratolins
- 1 SAI
- 1 punt d’accés inalàmbric
- Cables de xarxa i latiguillos
- 1 switch 1U no configurable

#### Observacions

- El switch 1U no configurable està connectat al switch troncal i als 5 PC.
- Els 5 PC tindran les seues pròpies VLANs per departament.

### Sobrants

- 1 switch 1U no configurable
