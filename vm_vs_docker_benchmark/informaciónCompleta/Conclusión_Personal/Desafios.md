[Conlusión Personal 📎](ConPersonal.md)

## Desafíos en la Implementación: Máquinas Virtuales vs. Docker

La configuración y ejecución de Civilization VI en Máquinas Virtuales (VM) y Docker presentó desafíos notables, si bien con diferencias significativas en su magnitud. La implementación en una Máquina Virtual de Windows 7 resultó ser considerablemente más manejable, atribuyéndose esto a la compatibilidad nativa del juego con el sistema operativo Windows. La configuración inicial fue más directa, y aunque no estuvo exenta de problemas, pude establecer un entorno funcional para las pruebas.
En contraste, la tentativa de ejecutar el juego en Docker fue una tarea extremadamente ardua, casi al punto de la deserción. La complejidad se derivó principalmente de la naturaleza de Docker, que, al operar sobre un núcleo Linux, implicaba la necesidad de emular o traducir las llamadas al sistema de Windows, lo cual es notoriamente complicado para aplicaciones gráficamente intensivas como los videojuegos. Los obstáculos incluyeron problemas de compatibilidad de drivers gráficos, configuraciones de red complejas y una latencia inaceptable, lo que hizo que la obtención de métricas confiables fuera un reto constante y propenso a fallos críticos del sistema.

[Diagramas de Métricas 📎](Diagramas/VM.md)