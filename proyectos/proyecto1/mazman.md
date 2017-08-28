

## Ambiente
 * Laberinto
   * [Generador](http://www.delorie.com/game-room/mazes/genmaze.cgi)
     * Modificarlo para que tengan espacios abiertos
 * Objetivo del juego: (Que les parece)
   * Salir del laberinto
   * Encontrar X cosa y salir
   * ???
   
## Monstruo
 * LeftEye capaza de navegar todo el laberinto pero solo hacia la izquierda
   * Ataca todo lo que se mueve
   * Camina durante N ciclos y descancansa N ciclos
   * Tiene una vision limitada de N cuadros
   * Conoce todo el laberinto
 * RigthEye capaza de navegar todo el laberinto pero solo hacia la derecha
   * Ataca todo lo que se mueve
   * Camina durante N ciclos y descancansa N ciclos
   * Tiene una vision limitada de N cuadros
   * Conoce todo el laberinto
 * Zap no se mueve
   * Tiene una vision limitada de N cuadros
   * Ataca todo lo que **NO** se mueve en forma continua
     * Si el movimiento es cuadro a cuadro no ataca
 * Guardia
   * Se mueve hacia puntos de control donde espera N ciclos y luego continua

## TODO

 * Determinar como es la interaccion entre el jugador y los otros agentes


