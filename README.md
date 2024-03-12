 # 

## DELL 1 = Servidor 1

    Sistema operativo: Lubuntu 22.04
    Disco: NVMe 100GB
           RAID 5 con tamaño de 256GB (128GB copia de seguridad)

| Componentes                    | Maquina 1                                                  | Maquina 2                                               |
|--------------------------------|------------------------------------------------------------|---------------------------------------------------------|
| Funcionalidad Principal        | Servidor empresarial                                       | Sistemas de copias de seguridad                         |
| Sistema Operativo              | Windows Server 2022 Standard                               | Open media vault 7.0-32                                 |
| Nucleos                        | 3-Nucleos 3-Hilos                                          | 2-Nucleos 2-Hilos                                       |
| Ram                            | 8GB                                                        | 2GB                                                     |
| Discos: Particiones, Capacidad | * Disco: NVME  --- Particion 1: Sistema  --- Tamaño: 70GB  | * Disco: NVME --- Particion 2: Sistema --- Tamaño: 25GB |
|                                | * Disco: Raid 5 --- Particion 1          --- Tamaño: 128GB | * Raid 5 con tamaño de 256GB y 128GB de seguridad       |
| Targetas de red                | Targeta red 1 --- Targeta de red 2                         | Targeta de red 1                                        |
| Observaciones                  |                                                            |                                                         |



## DELL 2 = Servidor 2

    Sistema operativo: Lubuntu 22.04
    Disco: NVMe 100GB
           RAID 5 con tamaño de 256GB (128GB copia de seguridad)

| Componentes                    | Maquina 1                                                  | Maquina 2                                                     |
|--------------------------------|------------------------------------------------------------|---------------------------------------------------------------|
| Funcionalidad Principal        | Servidor empresarial secundari                             | Servidor monitorizacion                                       |
| Sistema Operativo              | Windows Server 2022 Standard (NO GUI)                      | Fedora Linux 39                                               |
| Nucleos                        | 3-Nucleos 3-Hilos                                          | 3-Nucleos 3-Hilos                                             |
| Ram                            | 8GB                                                        | 6GB                                                           |
| Discos: Particiones, Capacidad | * Disco: NVME --- Particion 1: Sistema --- Tamaño: 50GB    | * Disco: NVME --- Particion 2: Sistema --- Tamaño: 50GB       |
|                                | * Disco: Raid 5 --- Particion 1          --- Tamaño: 128GB | * Disco: Raid 5 --- Particion 2 --- Tamaño: 128GB             |
| Targetas de red                | Targeta red 1                                              | Targeta red 1                                                 |
| Observaciones                  |                                                            |                                                               |   


## DELL 3 = Servidor 3
  
    Sistema operativo: Lubuntu 22.04
    Disco: NVMe 100GB

| Componentes                    | Maquina 1                                                  | Maquina 2                                                     | Maquina 3                                               |
|--------------------------------|------------------------------------------------------------|---------------------------------------------------------------|---------------------------------------------------------|
| Funcionalidad Principal        | Servidor web intranet                                      | Servidor de datos                                             | Servidors de aplicaciones i utilidades                  |
| Sistema Operativo              | Windows Server 2022 Standard (NO GUI)                      |  Windows Server 2022 Standard                                 | Windows Server 2022 Standard                            |
| Nucleos                        | 2-Nucleos 2-Hilos                                          | 2-Nucleos 2-Hilos                                             | 3-Nucleos 3-Hilos                                       |
| Ram                            | 6GB                                                        | 6GB                                                           | 6GB                                                     |
| Discos: Particiones, Capacidad | * Disco: NVME --- Particion 1: Sistema --- Tamaño: 50GB    | * Disco: NVME --- Particion 2: Sistema --- Tamaño: 50GB       | * Disco: NVME --- Particion 2: Sistema --- Tamaño: 70GB |
|                                |                                                            |                                                               | * Disco: Raid 5 --- Particion 2 --- Tamaño: 128GB        |
| Targetas de red                | Targeta red 1                                              | Targeta red 1 --- Targeta de red 2                            | Targeta de red 1                                        |
| Observaciones                  |                                                            |                                                               |                                                         




