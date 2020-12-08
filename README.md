# backgammon

Este programa desarrollará el árbol completo de posibles jugadas de backgammon como un juego "resuelto" al estilo de "3 en raya" o damas.

Backgammon es un juego que involucra estrategia y azar. La idea es generar el árbol completo de posibles jugadas para todos los posibles lanzamientos de datos y posibles moviminetos de fichas y obtener indicadores:

- Cantidad total de caminos: Número total de rutas en el árbol que nacen de la posición actual. Se excluyen loops, es decir caminos que generan un estado ya generado previamente.
- Probabilidad de ganar = cantidad de caminos que a partir de esta posición llevan a la victoria sobre la cantidad total de caminos. La probabilidad de perder = (1 - Probabilidad de ganar)
- Potencial de puntos = (Sumatoria de puntos en caso de ganar - sumatoria de puntos en caso de perder). Se debe tener en cuenta que una victoria o derrota puede valer diferentes puntajes. 1 punto si el perdedor pudo enviar al menos 1 de sus fichas a "home". 2 puntos si el perdedor no pudo enviar fichas a "home", pero no tenía ninguna ficha en la zona de partida. 3 puntos si el perdedor no pudo enviar ningna ficha a "home" y además tiene 1 o más fichas en la zona de partida. 
