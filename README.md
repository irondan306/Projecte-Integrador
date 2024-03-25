
Departament d’Informàtica
Cicle Formatiu de Grau Superior
Administració de Sistemes Informàtics en Xarxa
Projecte Integrador: Sistema Informàtic Empresarial
Curs: 2023-2024 / 2024-2025
Versió 18-març-2024
Fase 3 - Implantació bàsica del sistema
Pràctica 3.2. Disseny del CPD i organització de la seu

Enunciat
Introducció
Una vegada analitzat i dissenyat el sistema sobre el cas teòric, és el moment de dur a terme la
implementació del nostre sistema. Com no disposem físicament de les seus sobre les que
implementaríem i configuraríem el sistema, ho farem sobre un entorn simulat o de proves: al taller
d’informàtica. A continuació teniu una modificació i adaptació del projecte per a desenvolupar-lo al
taller en el temps del que disposem i amb les limitacions que tenim
Aquesta pràctica correspon a l’adaptació al taller de les pràctiques 2.1 (Disseny del CPD), 2.2
(Dimensionament del maquinari) i 2.3 (Elecció dels S.O.).
En aquesta pràctica organitzarem l’espai de treball del taller per a simular la nostra seu. Es suposa
que la seu té diferents departaments dividits en 2 plantes:
• Planta 0: ací trobem el CPD i a més els departaments de
o Producció
o Magatzem
• Planta 1
o Gerència
o Departament administratiu
o Comercials
o Tècnics
o Laboratori
Tasques obligatòries
Primer que tot farem una introducció sobre el material del que disposarem i dels requisits o tasques a realitzar
en els diferents mòduls. Posteriorment, hi ha un apartat sobre tasques a realitzar abans de començar la
implementació al taller.
Material disponible
El primer que farem és veure amb quin espai i maquinari físic contem per a desenvolupar el nostre projecte.
Respecte al maquinari teniu ho indicat en el vostre inventari. Cada seu dispossarà de:
○ Una cara del rack (l’altra serà per a la seu del costat), dividida en 3 zones:
■ La part inferior (fins el separador) és on estaran els servidors
■ La part central (fins el Cisco) fa de rack del CPD
■ La part superior és el rack de la planta 1
○ 1 Mikrotik que fa de servidor de comunicacions amb l’exterior
○ 1 switch Cisco 1U configurable que és el switch trocal de la seu
○ 1 switch TP-Link 1U configurable que és el switch troncal de la 1a planta
○ 1 switch TP-Link configurable de 8 ports no enrackable
○ 3 switches 1U no configurables
○ 2 punts d’accés inalàmbric
○ 3 PC Dell que faran de servidors de la seu
○ 5 PC per a fer de clients de la xarxa
○ 5 monitors, 5 teclats i 5 ratolins

○ 1 SAI
○ Adaptadors (heu de indicar quants en l’inventari)
○ Cables de xarxa i latiguillos
3.1 Disseny del CPD i els racks
Ho simularem en el rack que tenim en el taller per a la nostra seu. En realitat el rack el compartim entre 2 seus
i cadascuna d’elles utilitza una cara del mateix per la qual cosa haurem de posar-se d’acord per a no molestar
amb el nostre equipament i cablejat a la seu de l’altre costat.
El rack està organitzat verticalment en 3 zones:
• La part inferior, on podem deixar els servidors
• La resta del rack dividit en 2 parts pel switch Cisco. Aquest switch és el principal de la nostra seu i NO
ES POT CANVIAR DE LLOC. Suposem que la nostra seu te 2 plantes i:
o la meitat superior del rack serà per a la planta 1 i ací tindrem el switch TP-Link que és el switch
troncal d’eixa planta
o la part inferior serà el nostre CPD en la planta 0
Mòdul Fonaments de maquinari
A continuació es defineixen les configuracions a realitzar que fan referència a aquest mòdul:
 Rack
○ Organització i muntatge de cada seu (utilitzant Racks i taules per a definir els diferents espais
físics de les diferents seus).
○ Organització i divisió de l’armari de connexions (NO heu de menejar el switch Cisco).
○ Organització del cablejat d’alimentació per les seus i els diferents espais.
 SAIs
○ Configuració d’un sai per a configurar un sistema d’alimentació addicional. Aquest haurà de
configurar-se per als diferents servidors existents en l’empresa.
○ Configurar un servidor d’alimentació que serà l’encarregat de controlar el nivell de càrrega i
d’aturar per ordre d’importància els diferents servidors de l’empresa. Cal fer una llista dels
diferents servidors (fer almenys 2 tipus de servidors segons la seua importància).
 A més de rack cada seu disposa de una taula de trebal on es situaran els diferents equips clients de la
seu amb els seus monitors i teclats.
Apartat ampliació
A aquest apartat es tindrà en consideració qualsevol observació, aportació i/o millora sobre l’enunciat
obligatori. Cada grup podrà aportar tot allò que considere interessant i que puga donar un plus sobre
la part obligatòria.
