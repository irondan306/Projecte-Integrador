# 

## Servidor 1

| Componentes                    | Maquina 1                                                  | Maquina 2                                                     |
|--------------------------------|------------------------------------------------------------|---------------------------------------------                  |
| Funcionalidad Principal        | Servidor empresarial                                       | Servidors de aplicaciones i utilidades                        |
| Sistema Operativo              | Windows Server 2022 Standard                               | Windows Server 2022 Standard                                  |
| Nucleos                        | 3-Nucleos 3-Hilos                                          | 3-Nucleos 3-Hilos                                             |
| Ram                            | 8GB                                                        | 8GB                                                           |
| Discos: Particiones, Capacidad | * Disco: NVME  --- Particion 1: Sistema  --- Tamaño: 70GB  | * Disco: NVME --- Particion 1: Sistema --- Tamaño: 70GB       |
|                                | * Disco: SSD*3 --- Particion 2: Raid 5   --- Tamaño: 256GB | * Disco: SSD*3 --- Particion 2: Raid 5   --- Tamaño: 256GB    |
|                                |                                                            |                                                               |
| Targetas de red                | Targeta red 1 --- Targeta de red 2                         | Targeta red 1 --- Targeta de red 2                            |
| Observaciones                  |                                                            |                                                               |

## Servidor 2

| Componentes                    | Maquina 1                                                  | Maquina 2                                                     |
|--------------------------------|------------------------------------------------------------|---------------------------------------------------------------|
| Funcionalidad Principal        | Servidor empresarial secundari                             | Servidor monitorizacion                                       |
| Sistema Operativo              | Windows Server 2022 Standard (NO GUI)                      | Linux Red Hat Enterprise Linux 9.0                            |
| Nucleos                        | 2-Nucleos 2-Hilos                                          | 2-Nucleos 2-Hilos                                             |
| Ram                            | 8GB                                                        | 4GB                                                           |
| Discos: Particiones, Capacidad | * Disco: NVME --- Particion 1: Sistema --- Tamaño: 50GB    | * Disco: NVME --- Particion 1: Sistema --- Tamaño: 50GB       |
|                                | * Disco: SSD*3 --- Particion 2: Raid 5   --- Tamaño: 256GB | * Disco: SSD*3 --- Particion 2: Raid 5   --- Tamaño: 256GB    |
| Targetas de red                | Targeta red 1                                              | Targeta red 1                                                 |
| Observaciones                  |                                                            |                                                               |   |

## Servidor 3

| Componentes                    | Maquina 1                                                  | Maquina 2                                                     |
|--------------------------------|------------------------------------------------------------|---------------------------------------------------------------|
| Funcionalidad Principal        | Servidor web intranet                                      | Servidor de datos                                             | 
| Sistema Operativo              | Windows Server 2022 Standard (NO GUI)                      |  Windows Server 2022 Standard                                 | 
| Nucleos                        | 2-Nucleos 2-Hilos                                          | 2-Nucleos 2-Hilos                                             | 
| Ram                            | 8GB                                                        | 4GB                                                           |
| Discos: Particiones, Capacidad | * Disco: NVME --- Particion 1: Sistema --- Tamaño: 50GB    | * Disco: NVME --- Particion 1: Sistema --- Tamaño: 50GB       |
|                                | * Disco: SSD*3 --- Particion 2: Raid 5   --- Tamaño: 256GB | * Disco: SSD*3 --- Particion 2: Raid 5   --- Tamaño: 256GB    |
| Targetas de red                | Targeta red 1                                              | Targeta red 1                                                 |
| Observaciones                  |                                                            |                                                               |                                                                |




