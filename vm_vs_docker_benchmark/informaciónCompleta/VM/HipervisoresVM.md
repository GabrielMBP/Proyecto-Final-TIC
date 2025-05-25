[Que son las Máquinas Virtuales ⏮️](QueSonVM.md)

## Hipervisores

Para comprender plenamente el funcionamiento de las máquinas virtuales, es fundamental entender el papel del hipervisor, también conocido como monitor de máquina virtual (VMM por sus siglas en inglés, Virtual Machine Monitor). El hipervisor es el software esencial que permite la creación y ejecución de máquinas virtuales. Actúa como una capa intermedia entre el hardware físico y los sistemas operativos invitados que se ejecutan en las máquinas virtuales, orquestando el acceso de estos últimos a los recursos de hardware, como la CPU, la memoria, el almacenamiento y la red.

La función principal del hipervisor es aislar los sistemas operativos invitados entre sí y del hardware subyacente, al mismo tiempo que gestiona y distribuye los recursos del host de manera eficiente. Esto asegura que un fallo o un problema en una máquina virtual no afecte el rendimiento o la estabilidad de otras máquinas virtuales ni del sistema físico. Existen dos tipos principales de hipervisores, clasificados por su arquitectura y su relación con el hardware del host:

- [Hipervisores de Tipo 1 ⬇️](Hipervisores/Tipo1.md)

- [Hipervisores de Tipo 2 ⬇️](Hipervisores/Tipo2.md)