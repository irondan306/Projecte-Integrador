# Cronograma de Actividades

## Día 09/04
- Organización del rack para la instalación de los diferentes dispositivos y su conexión.
- Parte inferior del rack:
  - 3 PC Dell que funcionarán como servidores de la sede.
  - 1 Mikrotik que sirve como servidor de comunicaciones con el exterior.
  - 1 switch Baseline no configurable para datos.
  - 1 switch Longshine DMZ.
  - Cables de red y latiguillos.
  - 9 Adaptadores de red para las máquinas virtuales.
  - Patch panel planta 0:
    - Mikrotik.
    - Dell 1.
    - Dell 2.
    - Dell 3.
    - Producción.
    - Almacén.
    - DMZ (que van al switch Cisco troncal).
- Parte central:
  - 1 switch Cisco configurable que es el switch troncal de la sede.
- Parte superior:
  - Switch TP-Link TL-SG2216 configurable (troncal de la primera planta).
  - Switch Cisco Catalyst 3750 configurable (troncal de la sede).
  - Patch panel de la planta 1.

## Día 12/04
- Configuración e instalación base del servidor 1 en Dell 1.
- Creación del RAID1 en el servidor 1.
- Creación de los cables RJ45 necesarios para la conexión de los distintos dispositivos (equipos clientes a switches, switch a switch, switch a patch panel y patch panel a equipos).
- Clonación de la configuración y del sistema base del servidor 1 (Dell 1) con Clonezilla a los otros dos Dell (Dell 2 y 3).

## Día 30/04
- Configuración e instalación patch panel planta 0.
  - Puertos para Mikrotik, Dell 1, Dell 2, Dell 3, DMZ (que van al switch Cisco troncal).
  - Puertos para clientes producción y almacén.
- Configuración SSH e IP de los 3 Dell (servidores).

## Día 03/05
- Instalación sistema operativo base para Cliente 1 (Administración).
- Creación de las VLANs, habilitar conexión a la intranet para los servicios implementados.
- Configuración del acceso a internet desde las VLANs.

## Día 06/05
- Instalación y configuración del sistema operativo base en el Cliente 4, además de VirtualBox para la virtualización de los dos departamentos que albergará (producción y almacén).
- Instalación y configuración del sistema operativo base en el Cliente 3, además de VirtualBox para la virtualización de los dos departamentos que albergará (técnico y laboratorio).

## Día 07/05
- Reorganización de la sede, para mantener el orden del cableado correctamente.
- Nueva organización de los equipos clientes en la mesa principal.

## Día 10/05
- Reparación de problemas con la red, no disponíamos de acceso a la misma.

## Día 13/05
- Sustitución y reparación de cableado que daba problemas de conectividad con los equipos clientes y servidores.

## Día 17/05
- Configuración de TP-Link y VLANs restantes de la red.

## Día 20/05
- Creación / Instalación del servidor de datos.
- Creación del DFS
- Instalación y configuración de la máquina del servidor secundario.

## Día 21/05
- Reinstalación del servidor 1 en Dell 1 debido a problemas con la ejecución de VirtualBox (máquinas virtuales con los servidores ya creadas).
- Creación de buckets en AWS (web para la extranet). Habilitar estáticos.
- Instalación y configuración de un servidor web en AWS.

## Día 24/05
- Reinstalación del servidor 3 en Dell 3 debido a problemas con la ejecución de VirtualBox (máquinas virtuales con los servidores ya creadas).
- Servidor 1: Creación de las directivas.
- Acabar de organizar y conectar los cables definitivos que van del patch panel superior a los equipos cliente que se encuentran en la planta 1 y planta 0.

## Día 27/05
- Creación de los usuarios en el DC, de los distintos departamentos existentes, para que una vez añadidos puedan acceder.
- Instalación del sistema operativo en Cliente 5 (Gerencia), configuración del mismo y añadirlo al dominio.
- Instalación en el servidor Dell 2 de Zabbix, para la monitorización de nuestra red (incluyendo los distintos dispositivos que la componen).

## Día 28/05
- Inicio configuración Zabbix (adherir los distintos dispositivos de la red para su monitorización).
- Creación del script para la creación de los usuarios y grupos del DC.

## Día 03/06
- Seguimos con la configuración Zabbix (adherir los distintos dispositivos de la red para su monitorización, algunos problemas con algunos equipos).
- Seguimos con el script para la creación de los usuarios y grupos del DC, problemas con el código ya que no funciona correctamente, nos da fallo en algunas líneas y no termina de ejecutar correctamente lo que queremos.

## Día 08/06
- Instalación del servidor de la intranet y configuración.
- Instalación del servidor de aplicaciones y utilidades.
- Revisión WSUS

## Día 10/06
- Finalizar la configuración del servidor de aplicaciones y utilidades, virtualizado en el Dell 3, y comprobación de su correcto funcionamiento
- Continuación creación de la web.
- Se termina el script, comprobamos su correcto funcionamiento. Creación carpetas personales, móviles y obligatorias

## Día 11/06
- Crear y establecer reglas DMZ.
- Configurar replica DFS
- Se sigue con las tareas no finalizadas (página web)

## Día 13/06
- Corrección de configuraciones erróneas en los permisos de las carpetas de los perfiles de usuarios.
- Creación de la carpeta DOCUMENTACIÓ y subcarpetas necesarias para los departamentos. Modificar permisos de las subcarpetas, en función a los diferentes departamentos que van a tener acceso, según lo solicitado en el enunciado.
- Instalación WAC
- Seguimos con la tarea de la página web, que ya esta casi a punto, falta de acabar unicamente un apartado.
