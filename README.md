# 09/04
- Organización del rack para la instalación de los diferentes dispositivos y su conexión.
- Parte inferior del rack: 3 Dell que funcionan como servidores, el SAI y el Mikrotik.
- Parte central: Switch de la DMZ (Longshine), de datos (Baseline), patch panel que conectan con el switch cisco configurable para los 3 Dell servidores, la planta 0 (producción y almacén), además de la DMZ y datos.
- Parte superior: Switch TP-Link TL-SG2216 configurable (troncal de la primera planta), Switch Cisco Catalyst 3750 configurable (troncal de la sede) y patch panel de la planta 1.
# 12/04
- Configuración e instalación base del servidor 1 en Dell 1.
- Creación del RAID1 en el servidor 1.
- Creación de los cables RJ45 necesarios para la conexión de los distintos dispositivos (equipos clientes a switches - switch a switch - switch patch panel y patch panel a equipos).
- Clonación de la configuración y del sistema base del servidor 1 (Dell 1) con clonezilla, a los otros dos Dell (Dell 2 y 3). 
# 30/04
- Configuración e instalación patch panel planta 0.
- Puertos para Mikrotik, Dell 1, Dell 2, Dell 3, DMZ (que van al switch cisco troncal)
- Puertos para clientes producción y almacén.
- 
# 03/05
- 
# 06/05
- 
# 07/05
- 
# 10/05
- 
# 13/05
- 
# 17/05
- Instalación 
# 20/05
- Configuración de
# 21/05
- Reinstalación del servidor 1 en Dell 1 debido a problemas con la ejecución del virtualbox (maquinas virtuales con los servidores ya creadas)
- 
# 24/05
- Reinstalación del servidor 3 en Dell 3 debido a problemas con la ejecución del virtualbox (maquinas virtuales con los servidores ya creadas)
- Servidor 1 - Añadir directivas
- Acabar de organizar y conectar los cables definitivos que van del patch panel superior a los equipos cliente que se encuentran en la planta 1 y planta 0.
# 27/05
- Creación de los usuarios en el DC, de los distintos departamentos existentes, para que una vez añadidos al puedan acceder.
- Instalación sistema operativo en cliente 5, configuración del mismo. Añadirlo al dominio
- Instalación en el servidor Dell 2 zabbix, para la monitorización de nuestra red (incluyendo los distintos dispositivos que la componen)

# 28/05
