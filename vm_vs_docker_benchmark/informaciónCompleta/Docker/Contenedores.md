[Que es Docker 📎](QueSonDocker.md)

## Contendores

Los contenedores representan una forma ligera y eficiente de empaquetar, distribuir y ejecutar aplicaciones. A diferencia de las máquinas virtuales, que virtualizan la capa de hardware y ejecutan un sistema operativo completo para cada instancia, los contenedores virtualizan el sistema operativo. Esto significa que comparten el mismo kernel del sistema operativo del host, pero se ejecutan en entornos aislados del espacio de usuario.

Cada contenedor incluye la aplicación y todas sus dependencias necesarias: bibliotecas, herramientas del sistema, código y configuraciones. Este empaquetamiento completo asegura que la aplicación se ejecutará de manera consistente en cualquier entorno, desde la máquina de desarrollo hasta el servidor de producción, eliminando los problemas de "funciona en mi máquina".

Las características clave de los contenedores incluyen:

- **Ligereza:** Al compartir el kernel del host, los contenedores son significativamente más pequeños y consumen menos recursos (CPU, RAM, almacenamiento) que las máquinas virtuales. Se inician en segundos, en lugar de minutos.

- **Portabilidad:** Una vez que una aplicación está empaquetada en un contenedor, puede moverse y ejecutarse en cualquier sistema que tenga un motor de contenedores (como Docker) instalado, independientemente del sistema operativo subyacente (siempre que el kernel sea compatible, generalmente Linux).

- **Aislamiento:** Aunque comparten el kernel, los contenedores están aislados entre sí a nivel de procesos, red y sistema de archivos. Esto garantiza que las aplicaciones dentro de un contenedor no interfieran con las de otro.

- **Consistencia:** El entorno encapsulado garantiza que la aplicación se comporte de la misma manera en todos los entornos, desde el desarrollo hasta la producción.

- **Eficiencia:** Permiten una mayor densidad de aplicaciones por servidor físico, optimizando la utilización de recursos y reduciendo los costos operativos. Tecnologías como Docker han popularizado masivamente los contenedores al proporcionar herramientas intuitivas para construirlos, ejecutarlos y gestionarlos. Han sido fundamentales para el auge de las arquitecturas de microservicios, los pipelines de CI/CD (Integración Continua/Despliegue Continuo) y la computación en la nube, al ofrecer una forma estandarizada y eficiente de desplegar y escalar aplicaciones modernas.
