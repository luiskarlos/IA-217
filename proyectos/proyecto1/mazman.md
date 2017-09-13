## Objetivo
Aplicar la materia vista en clase

## Proyecto
Crear un programa de software que utilice un agente para resolver laberintos utilizando diferentes tecnicas de busqueda

## Requerimientos
1. Leer de un archivo de texto el laberinto generado con [Generador](https://www.vidarholen.net/cgi-bin/labyrinth)
   * Puede ser modificado para que tengan espacios abiertos
1. Leer un mapa de costo (Especificado más adelante)
   * El costo se traduce en un movimiento mas lento del agente mientras transita por esa zona.
1. Mostrar el laberinto en pantalla (Consola es válido, siempre y cuando el despliegue sea claro y ordenado, si no se puede apreciar como marca los caminos o como se mueve el agente la tarea se considera no entregada)
1. Colocar un agente de manera aleatoria o mediante una marca en el archivo del laberinto (tipo los ejercicios de hackerrank)
1. Escoger el algoritmo de búsqueda para que el agente salga del laberinto
1. El programa debe ir mostrando como el algoritmo de búsqueda recorre los diferentes caminos
1. Cuando el algoritmo de búsqueda encuentre la salida, hacer que el agente salga del laberinto
1. El ambiente puede ser totalmente observable o parcialmente observable (esto significa que los algoritmos de búsqueda puede que no puedan analizar totalmente el laberinto)

## Requerimientos técnicos
1. Utilizar FSM
1. Event Bus
1. Utilizar como base el algoritmo de busqueda visto en clase para implementar las búsquedas
1. El programa debe tener una velocidad ajustable
1. Debe tener controles que permitan:
   * cambiar los algoritmos de búsqueda
   * cambiar el tipo de ambiente escogiendo un radio máximo de visión (es opcional mostrar en pantalla la visión restringida)
   * pausar
   * cambiar la velocidad
   * cambiar la posición del agente
 1. Interface de despliegue que muestre:
   * El análisis paso a paso del algoritmo de búsqueda
   * El progreso del agente recorriendo un camino

## Mapa de Costo
El mapa de costo consiste un archivo de texto en el cual se marcan puntos de costo, estos puntos van disminuyendo de manera circular hasta llegar a 0, si 2 o más puntos se encuentran los costos se suman. Ver mapa de ejemplo
En el mapa solo se marcan los puntos iniciales, el programa debe calcular el costo total.
Estos costos deben ser considerados por los algoritmos de busqueda que puedan hacerlo

### Mapa inicial:
                                                                 
                                        2                        
            3                                                        
               3                                                
                                                                 
                                             2                   
                                                                 

#### Mapa expandido:
                                                                 
           111                         111                       
          12222111                     121                       
          12323221                     111                            
          12223321                                                
          11123221                           111                 
              1111                           121                  
                                             111                 

## Algoritmos de busqueda a implementar

1. BFS 
2. DFS 
3. A*

## Opcional
Lo mencionado sobre otros agentes en el mapa queda de manera opcional en esta primera etapa.
