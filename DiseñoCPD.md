# Pràctica 3.2. Disseny del CPD i organització de la seu

## Parte inferior del rack

- 3 PC Dell que funcionarán como servidores de la sede
- 1 switch 1U no configurable
- Cables de red y latiguillos
- 7 Adaptadores de red para las máquinas virtuales
- 1 switch TP-Link configurable de 8 puertos no enrackable

#### Observaciones

- El switch 1U no configurable está conectado al switch Cisco troncal y a los 3 PC Dell, a través de los adaptadores.
- El switch TP-Link configurable de 8 puertos no enrackable está conectado al Mikrotik por un lado y, por otro lado, a la DMZ.

## Parte central del rack

- 1 Mikrotik que sirve como servidor de comunicaciones con el exterior
- 1 switch Cisco 1U configurable que es el switch troncal de la sede
- Cables de red y latiguillos

#### Observaciones

- El Mikrotik está conectado a internet y al switch Cisco troncal (también está conectado al switch de la DMZ, como hemos especificado arriba).

## Parte superior del rack

- 1 switch TP-Link 1U configurable que es el switch troncal de la 1a planta
- 1 punto de acceso inalámbrico
- Cables de red y latiguillos

#### Observaciones

- El switch TP-Link 1U configurable está conectado al switch Cisco troncal y al punto de acceso inalámbrico.

## Fuera del rack

- 5 PC para funcionar como clientes de la red
- 5 monitores, 5 teclados y 5 ratones
- 1 SAI
- 1 punto de acceso inalámbrico
- Cables de red y latiguillos
- 1 switch 1U no configurable

#### Observaciones

- El switch 1U no configurable está conectado al switch troncal y a los 5 PC.
- Los 5 PC tendrán sus propias VLANs por departamento.

### Sobrantes
- 1 switch 1U no configurable

