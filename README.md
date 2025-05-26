## Proyecto Final TIC

[Máquinas virtuales (MV) 📎](vm_vs_docker_benchmark/informaciónCompleta/VM/OrigenVM.md) y [Docker 📎](vm_vs_docker_benchmark/informaciónCompleta/Docker/OrigenDocker.md) son tecnologías que optimizan el uso de recursos y proporcionan entornos aislados para aplicaciones, aunque con enfoques distintos.

# [Máquinas Virtuales (MV) ](vm_vs_docker_benchmark/informaciónCompleta/VM/OrigenVM.md)

Las MV surgieron en la década de 1960 para optimizar el uso de los costosos recursos de los mainframes. Permiten que múltiples entornos operativos compartan un mismo hardware físico mediante la abstracción del hardware. Un hito fue el sistema CP-40 y CP-67 de IBM, que permitió ejecutar múltiples sistemas operativos en un solo mainframe.

- [Importancia de las Máquinas Virtuales📎](vm_vs_docker_benchmark/informaciónCompleta/VM/ImportanciaVM.md)

 Han revolucionado la eficiencia de los centros de datos al permitir la consolidación de servidores, reduciendo costos de hardware, energía y espacio físico. También son cruciales para la gestión de carga de trabajo, la flexibilidad operativa, la recuperación ante desastres y la continuidad del negocio. Además, ofrecen seguridad y aislamiento, ya que las fallas en una MV no suelen afectar a otras o al sistema host.

- [Qué son las Máquinas Virtuales 📎](vm_vs_docker_benchmark/informaciónCompleta/VM/QueSonVM.md)

Una MV es la emulación de un sistema informático, una "computadora dentro de una computadora". Desacoplan el software del hardware, permitiendo que aplicaciones y sistemas operativos se ejecuten independientemente del hardware físico específico. Son el motor del cloud computing, ya que los proveedores de servicios en la nube las utilizan para ofrecer recursos a demanda.

- [Hipervisores 📎](vm_vs_docker_benchmark/informaciónCompleta/VM/HipervisoresVM.md)

Son el software esencial que permite la creación y ejecución de MV, actuando como una capa intermedia entre el hardware físico y los sistemas operativos invitados. Existen dos tipos:

 - [Tipo 1 (Bare-Metal o Nativo) 📎](vm_vs_docker_benchmark/informaciónCompleta/VM/Hipervisores/Tipo1.md)

 Se instalan directamente sobre el hardware físico y ofrecen alto rendimiento y baja latencia. Ejemplos incluyen VMware ESXi y Microsoft Hyper-V.

 - [Tipo 2 (Hosted o Alojado) 📎](vm_vs_docker_benchmark/informaciónCompleta/VM/Hipervisores/Tipo2.md)

 Se ejecutan como una aplicación dentro de un sistema operativo host convencional. Ejemplos son VMware Workstation y Oracle VirtualBox.

# [Docker 📎](vm_vs_docker_benchmark/informaciónCompleta/Docker/OrigenDocker.md)

Docker popularizó el uso de contenedores de Linux a partir de 2013, buscando resolver los problemas de inconsistencia entre entornos de desarrollo y producción. Empaqueta la aplicación y todas sus dependencias en un paquete autocontenido y portátil, llamado contenedor. A diferencia de las MV, los contenedores comparten el kernel del sistema operativo host, lo que les confiere ligereza y eficiencia.

- [Importancia de Docker📎](vm_vs_docker_benchmark/informaciónCompleta/Docker/ImportanciaDocker.md)

Ha mejorado la portabilidad y consistencia del entorno, eliminando la fricción entre equipos de desarrollo y operaciones. Ofrece eficiencia en el uso de recursos al ser más ligeros y rápidos que las MV, permitiendo ejecutar más aplicaciones en un solo servidor físico. Ha sido un catalizador para la adopción de arquitecturas de microservicios, facilitando el desarrollo y escalado independiente de componentes de una aplicación.

- [Qué es Docker 📎](vm_vs_docker_benchmark/informaciónCompleta/Docker/QueSonDocker.md)

Docker es una plataforma para desarrollar, enviar y ejecutar aplicaciones en entornos ligeros y portátiles llamados contenedores. Un contenedor encapsula todo lo necesario para que una aplicación funcione, virtualizando el sistema operativo en lugar del hardware completo. Esto permite que múltiples contenedores compartan el mismo kernel del sistema operativo, pero estén aislados entre sí. Docker facilita la inmutabilidad de la infraestructura y la entrega continua de software.

- [Contenedores 📎](vm_vs_docker_benchmark/informaciónCompleta/Docker/Contenedores.md)

Son una forma ligera y eficiente de empaquetar, distribuir y ejecutar aplicaciones. Comparten el mismo kernel del sistema operativo del host, pero se ejecutan en entornos aislados del espacio de usuario. Sus características clave incluyen:


- **Ligereza:** Son más pequeños y consumen menos recursos que las MV, iniciando en segundos.
- **Portabilidad:** Pueden ejecutarse en cualquier sistema con un motor de contenedores.
- **Aislamiento:** Están aislados entre sí a nivel de procesos, red y sistema de archivos.
- **Consistencia:** El entorno encapsulado garantiza un comportamiento uniforme en todos los entornos.
- **Eficiencia:** Permiten una mayor densidad de aplicaciones por servidor físico.

# [Máquinas Virtuales vs. Docker](vm_vs_docker_benchmark/informaciónCompleta/README.md)

Ambas tecnologías comparten objetivos como el aislamiento de aplicaciones, la portabilidad, la consistencia de entorno, la eficiencia en el uso de recursos, y el despliegue y escalabilidad.

- [Diferencias clave 📎](vm_vs_docker_benchmark/informaciónCompleta/VM_vs_Docker/Diferencias.md)

- **Capa de virtualización:** Las MV emulan hardware completo, mientras que Docker virtualiza el sistema operativo, compartiendo el kernel del host.
- **Sistema Operativo:** Cada MV tiene su propio SO completo; los contenedores comparten el SO del host.
- **Tamaño de la imagen:** Las imágenes de MV son de gigabytes (SO + aplicación); las de Docker son de megabytes (aplicación + dependencias).
- **Consumo de recursos:** Las MV tienen un consumo alto; Docker es mucho más ligero y eficiente.
- **Tiempo de arranque:** Las MV tardan minutos; los contenedores, segundos o milisegundos.
- **Granularidad de aislamiento:** Las MV ofrecen aislamiento completo a nivel de hardware; Docker, aislamiento a nivel de proceso y espacio de nombres.
- **Portabilidad:** Las MV son portátiles entre hipervisores compatibles; Docker, entre cualquier host con motor Docker (generalmente Linux).
- **Casos de uso típicos:** Las MV son ideales para ejecutar múltiples SO diferentes, aplicaciones legacy y servidores dedicados; Docker es preferido para microservicios, CI/CD y aplicaciones modernas.

- [Perspectivas de la comunidad 📎](vm_vs_docker_benchmark/informaciónCompleta/VM_vs_Docker/Diferencias.md)

- **Rendimiento y Ligereza:** Docker es el preferido para microservicios y aplicaciones que necesitan escalar rápidamente debido a su mínimo overhead y rápido tiempo de inicio.
- **Aislamiento y Seguridad:** Las MV suelen ser preferidas cuando el aislamiento absoluto y la seguridad a nivel de kernel son primordiales.
- **Entornos Heterogéneos y Legado:** Las MV son la única opción viable para ejecutar sistemas operativos completamente diferentes o aplicaciones legacy con dependencias específicas del SO.
- **Simplicidad para Desarrolladores:** Docker ha simplificado el flujo de trabajo de los desarrolladores para el empaquetado y la distribución de aplicaciones.

En muchos entornos modernos, ambas tecnologías coexisten. Es común ejecutar contenedores Docker dentro de máquinas virtuales, aprovechando lo mejor de ambos mundos: la capa de aislamiento de hardware de las MV y la agilidad y eficiencia de los contenedores.

[Conlusión Personal 📎](vm_vs_docker_benchmark/informaciónCompleta/Conclusión%20Personal/ConPersonal.md)