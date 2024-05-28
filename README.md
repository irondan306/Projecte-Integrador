## Día 09/04
- Organización del rack para la instalación de los diferentes dispositivos y su conexión.
- Parte inferior del rack: 3 Dell que funcionan como servidores, el SAI y el Mikrotik.
- Parte central: Switch de la DMZ (Longshine), de datos (Baseline), patch panel que conectan con el switch cisco configurable para los 3 Dell servidores, la planta 0 (producción y almacén), además de la DMZ y datos.
- Parte superior: Switch TP-Link TL-SG2216 configurable (troncal de la primera planta), Switch Cisco Catalyst 3750 configurable (troncal de la sede) y patch panel de la planta 1.
## Día 12/04
- Configuración e instalación base del servidor 1 en Dell 1.
- Creación del RAID1 en el servidor 1.
- Creación de los cables RJ45 necesarios para la conexión de los distintos dispositivos (equipos clientes a switches - switch a switch - switch patch panel y patch panel a equipos).
- Clonación de la configuración y del sistema base del servidor 1 (Dell 1) con clonezilla, a los otros dos Dell (Dell 2 y 3). 
## Día 30/04
- Configuración e instalación patch panel planta 0.
- Puertos para Mikrotik, Dell 1, Dell 2, Dell 3, DMZ (que van al switch cisco troncal)
- Puertos para clientes producción y almacén.
- Configuración ssh e IP de los 3 Dell (servidores).
## Día 03/05
- Instalación sitema operativo base para Cliente 1 (Administración)
- Creación de las Vlans, habilitar conexión a la intranet para los servicios implementados
- Configuración del acceso a internet desde las Vlans.
## Día 06/05
- Instalación y configuración sistema operativo base en el Cliente 4, además de VirtualBox para la virtualización de los dos departamentos que albergará (producción y almacén).
- Instalación y configuración sistema operativo base en el Cliente 3, además de VirtualBox para la virtualización de los dos departamentos que albergará (técnico y laboratorio).
## Día 07/05
- Reorganización de la sede, para mantener el orden del cableado correctamente.
- Nueva organización de los equipos clientes en mesa principal.
## Día 10/05
- Reparación de problemas con la red, no disponiamos de acceso a la misma.
## Día 13/05
- Sustitución y reparación de cableado que daba problemas de conectividad con los equipos clientes y servidores.
## Día 17/05
- Configuración de TP-Link y Vlans restantes de la red.
## Día 20/05
- Configuración de
## Día 21/05
- Reinstalación del servidor 1 en Dell 1 debido a problemas con la ejecución del virtualbox (maquinas virtuales con los servidores ya creadas)
- Creación pukets en AWS (web para la extranet). Habilitar estáticos
- Instlación y configuración de un servidror web en AWS.
## Día 24/05
- Reinstalación del servidor 3 en Dell 3 debido a problemas con la ejecución del virtualbox (maquinas virtuales con los servidores ya creadas)
- Servidor 1 - Añadir directivas
- Acabar de organizar y conectar los cables definitivos que van del patch panel superior a los equipos cliente que se encuentran en la planta 1 y planta 0.
## Día 27/05
- Creación de los usuarios en el DC, de los distintos departamentos existentes, para que una vez añadidos al puedan acceder.
- Instalación sistema operativo en Cliente 5 (Gerencia), configuración del mismo. Añadirlo al dominio.
- Instalación en el servidor Dell 2 zabbix, para la monitorización de nuestra red (incluyendo los distintos dispositivos que la componen).

## Día 28/05
- Terminar de configurar zabbix (adherir los distintos dispositivos de la red, para su monitorización)
- Creación del script para la creación de los usuarios y grupos del DC.
