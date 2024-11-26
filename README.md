# Simulación de juegos

## Descripción de la Tarea 1

En la Tarea 1, se implementó un simulador del juego Rock, Paper, Scissors, Lizard, Spock. Este juego amplía las reglas del tradicional Piedra, Papel o Tijera, incorporando dos nuevas estrategias (Lizard y Spock), con reglas específicas para determinar el ganador entre las elecciones de dos jugadores.

## Detalles de la implementación:
Definición de estrategias y reglas del juego:

Se definieron las estrategias posibles: 'Rock', 'Paper', 'Scissors', 'Lizard', y 'Spock'.
Las reglas del juego se almacenaron en un data.frame, donde cada fila representa las interacciones entre la estrategia de un jugador (Player1) contra las posibles estrategias de su oponente (Player2).
Cálculo del resultado del juego:

## Se implementó la función get_result, que compara las elecciones de ambos jugadores y devuelve un puntaje para cada uno:
1 si un jugador gana.
0 si pierde.
0, 0 en caso de empate.
Simulación de jugadores:

Se crearon dos jugadores (John y Mary) con nombres, puntuaciones iniciales en 0, y estrategias elegidas de manera aleatoria usando la función sample.
Ejecución de la partida:

Se determinaron las estrategias de ambos jugadores y se calculó el resultado de la partida utilizando la función get_result.
Las puntuaciones de cada jugador se actualizaron en función de los resultados.
Visualización de resultados:

Se generó un data.frame para mostrar las puntuaciones finales de los jugadores.
Se determinó el ganador en base a la puntuación más alta.
Ejemplo de ejecución:
## Decisiones tomadas:
John's strategy: Paper
Mary's strategy: Rock
## Resultados:
John obtiene 1 punto.
Mary obtiene 0 puntos.
## Ganador:
John es declarado el ganador de la partida.
Este código sirve como base para simular partidas entre dos jugadores, permitiendo expandir o modificar las reglas según sea necesario. Además, es un excelente ejercicio para modelar sistemas de decisión y puntuación en R.

## Descripción de la Tarea 2
La Tarea 2 implementa un modelo ampliado del juego Rock, Paper, Scissors, Lizard, Spock en el que participan múltiples jugadores y se simulan varias rondas. El objetivo principal es permitir que los jugadores compitan entre sí en un formato de todos contra todos, calculando las puntuaciones acumulativas y determinando el ganador al final. Además, se utiliza una visualización dinámica con ggplot2 para mostrar los puntajes al término de cada ronda.

## Características principales:
Definición de estrategias y reglas del juego:

## Las estrategias disponibles son: Rock, Paper, Scissors, Lizard, Spock.
Se define una matriz de pagos que determina el resultado entre dos estrategias dadas.
Configuración del juego:

Se inicializan 5 jugadores, cada uno con un nombre, un puntaje inicial de 0 y una estrategia que se selecciona aleatoriamente antes de cada ronda.
Se establecen 5 rondas de juego.
## Simulación del juego:

En cada ronda, cada jugador selecciona una estrategia aleatoria.
Todos los jugadores compiten entre sí en formato de todos contra todos:
Se calcula el resultado de cada enfrentamiento utilizando la matriz de pagos.
Se actualizan los puntajes acumulativos de ambos jugadores.
Visualización dinámica:

## Al final de cada ronda, se genera un gráfico de barras que muestra los puntajes actualizados de los jugadores. La librería ggplot2 se utiliza para crear gráficos estilizados y fáciles de interpretar.
## Resultados finales:

Se muestra una tabla con los puntajes finales acumulados de todos los jugadores.
Se determina al ganador (o ganadores en caso de empate), basándose en el puntaje más alto.
## Ejemplo de resultados:
En cada ronda, se registran las estrategias seleccionadas por los jugadores y los resultados de cada enfrentamiento.
Al final de todas las rondas, se anuncia el o los ganadores. Por ejemplo, en este caso:
Los ganadores fueron Player 3 y Player 5, quienes empataron con el puntaje más alto.
Este enfoque no solo automatiza la simulación del juego, sino que también incorpora elementos visuales y dinámicos para facilitar el análisis de los resultados en tiempo real.

![image](https://github.com/user-attachments/assets/642873e2-d1dc-4ab1-a907-422817c6327a)


