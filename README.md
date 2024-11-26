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
