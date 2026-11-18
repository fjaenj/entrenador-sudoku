# Entrenador de figuras de sudoku

Banco de ejercicios y tutorial interactivo para aprender a **detectar** las figuras
avanzadas del sudoku, no solo a entenderlas.

Página única, sin dependencias ni servidor: `index.html` lo lleva todo dentro.

## Qué hay

- **Guiado** — te dice qué figura buscar y solo tienes que señalarla. Con filtro por
  técnica, para hacer veinte X-wing seguidos hasta que la forma se quede grabada.
- **Caza libre** — no te dice nada. Puede haber figura o no haberla: 20 de los
  tableros son señuelos con estructura estéril, para entrenar la comprobación del
  mordisco.
- **Tutorial** — doce fichas (dos de método y diez de técnica), cada una con un
  ejemplo real recorrible paso a paso. Se consulta desde dentro del ejercicio.
- **Progreso** — acierto y tiempo medio por técnica, con los falsos positivos
  contados aparte.

## El banco

108 posiciones, todas **reales**: se generaron miles de sudokus, un motor de técnicas
humanas los resolvió paso a paso, y se guardó cada posición en la que la jugada más
simple disponible era una de las que se entrenan.

| Familia | Ejercicios |
|---|---|
| Peces (X-wing, swordfish) | 24 |
| Subconjuntos | 22 |
| Cadenas (rascacielos) | 22 |
| Intersecciones | 20 |
| Señuelos (sin jugada) | 20 |

Entre los señuelos hay seis con un **rascacielos estéril**: la figura está
perfectamente formada y no borra nada.

## Uso

Abrir `index.html` en el navegador. No necesita instalación.

El progreso se guarda en el `localStorage` del navegador, así que es local a cada
dispositivo.
