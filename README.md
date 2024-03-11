# 
## Servidor 1

| Componentes                    | Maquina 1                                                 | Maquina 2                                                     | 
|--------------------------------|-----------------------------------------------------------|---------------------------------------------                  |
| Funcionalidad Principal        | Servidor empresarial                                      | Servidors de dades i aplicacions                              |  
| Sistema Operativo              | Windows Server 2022 Standard                              | Windows Server 2022 Standard (NO GUI)                         |
| Nucleos                        | 3-Nucleos 3-Hilos                                         | 3-Nucleos 3-Hilos                                             |
| Ram                            | 8GB                                                       | 8GB                                                           |
| Discos: Particiones, Capacidad | * Disco: NVME --- Particion 1: Sistema --- Tamaño: 70GB   | * Disco: SSD  --- Particion 3: Raid 1  --- Tamaño: 128GB      |
|                                | * Disco: SSD  --- Particion 2: Datos   --- Tamaño: 128GB  | * Disco: SSD  --- Particion 3: Raid 1  --- Tamaño: 128GB      |
|                                |                                                           |                                                               |
| Targetas de red                | Cell 2                                                    | Cell 3                                                        |

## Servidor 2

| Componentes                    | Maquina 1                                                 | Maquina 2                                                     | Maquina 3                                 |
|--------------------------------|-----------------------------------------------------------|---------------------------------------------------------------|-------------------------------------------|
| Funcionalidad Principal        | Servidor empresarial secundari                            | Servidor de copias de seguridad                               | Servidor aplicaciones y utilidades        |
| Sistema Operativo              | Windows Server 2022 Standard                              |                                                               |
| Nucleos                        | 3-Nucleos 3-Hilos                                         |                                                               |
| Ram                            | 8GB                                                       |                                                               |
| Discos: Particiones, Capacidad | * Disco: NVME --- Particion 1: Sistema --- Tamaño: 70GB   | * Disco: SSD  --- Particion 3: Raid 1  --- Tamaño: 128GB      |
|                                | * Disco: SSD  --- Particion 2: Datos   --- Tamaño: 128GB  | * Disco: SSD  --- Particion 3: Raid 1  --- Tamaño: 128GB      |
|                                |                                                           |                                                               |
| Targetas de red                | Cell 2                                                    | Cell 3                                                        |

## Servidor 3

| Componentes                    | MAQUINA 1                        | MAQUINA 2             | MAQUINA 3
|--------------------------------|----------------------------------|-----------------------|-----------------------|
| Funcionalidad Principal        | Servidor monitorizacion          | Servidor web intranet | Servidor web externo  |
| Sistema Operativo              | Windows Server 2022 Standard     |                       |                       |
| Nucleos                        | 3-Nucleos 3-Hilos                |                       |                       |
| Ram                            | 8GB                              |                       |                       |
| Discos: Particiones, Capacidad | Cell 2                           |                       |                       |
| Targetas de red                | Cell 2                           |                       |                       |

