# Pràctica 3.2. Disseny del CPD i organització de la seu

## Part inferior del rack

- 1. 3 PC Dell que faran de servidors de la seu
- 2. 1 switch 1U no configurable
- 3. Cables de xarxa i latiguillos
- 4. 7 Adaptadors de xarxa per a les màquines virtuals
- 5. 1 switch TP-Link configurable de 8 ports no enrackable

#### Observacions

- El switch 1U no configurable va connectat al switch cisco troncal i als 3 PC Dell, a través dels adaptadors
- El switch TP-Link configurable de 8 ports no enrackable va connectat al mikrotik per un costat i, per altre costat, a la DMZ

## Part central del rack

1. 1 Mikrotik que fa de servidor de comunicacions amb l’exterior
2. 1 switch Cisco 1U configurable que és el switch trocal de la seu
3. Cables de xarxa i latiguillos

#### Observacions

- El Mikrotik estè connectat a l'internet i al switch cisco troncal ( també va connectat al switch de la DMZ, com hem especificat dalt )

## Part superior del rack
1. 1 switch TP-Link 1U configurable que és el switch troncal de la 1a planta
2. 1 punt d’accés inalàmbric
3. Cables de xarxa i latiguillos

#### Observacions

- El switch TP-Link 1U configurable va conectat al switch cisco troncal i al punt d'acces inalambric

## Fora del rack
1. 5 PC per a fer de clients de la xarxa
2. 5 monitors, 5 teclats i 5 ratolins
3. 1 SAI
4. 1 punt d’accés inalàmbric
5. Cables de xarxa i latiguillos
6. 1 switch 1U no configurable

#### Observacions

- El switch 1U no configurable va conectat al switch troncal i als 5 PC
- Els 5 PC tindran les seues propies VLANS per departament

### Sobrants
1. 1 switch 1U no configurable
