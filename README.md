# Configuración de Servidores

## DELL 1 = Servidor 1
---

- **Sistema operativo:** Lubuntu 22.04
- **Disco:** NVMe con tamaño de 100GB


| **Componentes**                    | **Maquina 1**                                               | **Maquina 2**                                                                                    |
|------------------------------------|-------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| **Funcionalidad Principal**        | Servidor empresarial                                        | Sistemas de copias de seguridad                                                                  |
| **Sistema Operativo**              | Windows Server 2022 Standard                                | OpenMediaVault 7.0-32                                                                            |
| **Nucleos**                        | 3 Nucleos 3 Hilos                                           | 2 Nucleos 2 Hilos                                                                                |
| **Ram**                            | 8GB                                                         | 2GB                                                                                              |
| **Discos: Particiones, Capacidad** | * Disco: NVMe --- Particion 1: Sistema --- Tamaño: 70GB     | * Disco: NVMe --- Particion 3: Sistema --- Tamaño: 25GB                                          |
|                                    | * Disco: NVMe --- Particion 2: Datos --- Tamaño: 50GB       | * Raid 5 con tamaño de 256GB y 128GB de seguridad                                                |
| **Tarjetas de red**                | Tarjeta red 1 --- Tarjeta de red 2                          | Tarjeta de red 1                                                                                 |
| **Observaciones**                  |                                                             | Almacenamiento de datos, DFS. Copias incrementales lunes, martes, jueves y viernes. Diferenciales miércoles y completas el sábado |
| **Software Adicional**             | Active Directory, WDS                                       | Rsync, herramientas de gestión de OpenMediaVault para backups                                    |
| **Prioridad SAI**                  | Alta                                                        | Alta                                                                                            |


## DELL 2 = Servidor 2
---

- **Sistema operativo:** Lubuntu 22.04
- **Disco:** NVMe con tamaño de 100GB y RAID 5 con tamaño de 256GB (128GB copia de seguridad)

| **Componentes**                    | **Maquina 1**                                               | **Maquina 2**                                                             |
|------------------------------------|-------------------------------------------------------------|---------------------------------------------------------------------------|
| **Funcionalidad Principal**        | Servidor empresarial secundario                             | Servidor monitorización                                                   |
| **Sistema Operativo**              | Windows Server 2022 Standard (NO GUI)                       | Fedora Linux 39                                                           |
| **Nucleos**                        | 3 Nucleos 3 Hilos                                           | 3 Nucleos 3 Hilos                                                         |
| **Ram**                            | 8GB                                                         | 6GB                                                                       |
| **Discos: Particiones, Capacidad** | * Disco: NVMe --- Particion 1: Sistema --- Tamaño: 70GB     | * Disco: NVMe --- Particion 2: Sistema --- Tamaño: 50GB                   |
|                                    | * Disco: Raid 5 --- Particion 1 --- Tamaño: 128GB           | * Disco: Raid 5 --- Particion 2 --- Tamaño: 128GB                         |
| **Tarjetas de red**                | Tarjeta red 1                                               | Tarjeta red 1                                                             |
| **Observaciones**                  | Hará de soporte del dominio principal.                      | Zabbix para monitorizar infraestructura (equipos y dispositivos de la red)|
| **Software Adicional**             | Herramientas de administración sin GUI                      | Zabbix, agentes SNMP, SSH para monitorización                             |
| **Prioridad SAI**                  | Media                                                       | Baja                                                                      |


## DELL 3 = Servidor 3
---

- **Sistema operativo:** Lubuntu 22.04
- **Disco:** NVMe 100GB y RAID 5 con tamaño de 256GB (128GB copia de seguridad)

| **Componentes**                    | **Maquina 1**                                               | **Maquina 2**                                               | **Maquina 3**                                                 |
|------------------------------------|-------------------------------------------------------------|-------------------------------------------------------------|---------------------------------------------------------------|
| **Funcionalidad Principal**        | Servidor web intranet                                       | Servidor de datos                                           | Servidor de aplicaciones y utilidades                         |
| **Sistema Operativo**              | Windows Server 2022 Standard (NO GUI)                       | Windows Server 2022 Standard                                | Windows Server 2022 Standard                                  |
| **Nucleos**                        | 2 Nucleos 2 Hilos                                           | 2 Nucleos 2 Hilos                                           | 3 Nucleos 3 Hilos                                             |
| **Ram**                            | 6GB                                                         | 6GB                                                         | 6GB                                                           |
| **Discos: Particiones, Capacidad** | * Disco: NVMe --- Particion 1: Sistema --- Tamaño: 50GB     | * Disco: NVMe --- Particion 2: Sistema --- Tamaño: 50GB     | * Disco: NVMe --- Particion 3: Sistema --- Tamaño: 50GB       |
|                                    |                                                             |                                                             | * Disco: Raid 5 --- Particion 1 --- Tamaño: 128GB             |
| **Tarjetas de red**                | Tarjeta red 1                                               | Tarjeta red 1 --- Tarjeta de red 2                          | Tarjeta de red 1                                              |
| **Observaciones**                  | No lleva disco secundario, ya que por sus funciones no lo requiere. | No lleva disco secundario, ya que por sus funciones no lo requiere. | Aplicaciones para los clientes (LibreOffice, GIMP, etc)            |
| **Software Adicional**             | IIS, configuración para intranet                            | DFS para gestión de recursos compartidos                     | Servicios de Escritorio Remoto para aplicaciones               |
| **Prioridad SAI**                  | Baja                                                        | Media                                                       | Media                                                          |


- **Mantenimiento y Monitoreo:**
  - El mantenimiento regular se realiza fuera del horario laboral para minimizar el impacto en los usuarios.
  - Se utilizan herramientas como Zabbix para monitorear el rendimiento y la disponibilidad de las máquinas.

- **Recuperación ante Desastres:**
  - Las copias de seguridad se almacenan tanto localmente en el Servidor 1 como en la nube para redundancia.
  - Se dispone de un protocolo para restaurar rápidamente los servicios a partir de las copias de seguridad más recientes en caso de fallo del hardware.
 
- **Políticas de Seguridad:**
  - Las actualizaciones de seguridad se aplican mensualmente.
  - Se implementan políticas de contraseñas fuertes.

