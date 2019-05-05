# API Estructura de Datos

Programación en python de las estructuras basicas de datos, algoritmos de ordenamiento y grafos(pendiente).

## Estructuras basicas de datos

### _Listas simplemente enlazadas_

#### __Metodos__
___agreagar___
Este método dentro de la clase LSE se encarga de agregar un nuevo nodo dentro de la lista haciendo uso de un dato u objeto que entre como parámetro.

- __Parámetros:__
  * __nuevo_dato:__ Es el dato que contendrá el nodo que se está creando.
- __Retornos:__
  * __True:__ El método retornará True si el nodo pudo ser creado.
  * __False:__ El método retornará False si el nodo no pudo ser creado.

___remover___
Este método dentro de la clase LSE se encarga de remover un nodo dentro de la lista sea uno o varios a la vez.

_ __Parámetros:__
  * __item:__ Este parámetro actúa de dos maneras bien sea actuando como dato para eliminar todos los nodos que lo contengan a eliminar un nodo siendo este su posición.
  * __por_pos:__ Se lo inicializa por defecto en True haciendo que "item" sea una posición. Si se lo cambia a falso, "item" es el dato que se contiene en los nodos a eliminar.
_ __Retornos:__
  * __True:__ El método retornará True si el nodo, o nodos, pudo ser removido
  * __False:__ El método retornará False si el nodo, o nodos, no pudo ser removido.

___posicionar___
Este método dentro de la clase LSE se encarga de agregar un nodo con el dato que llegue como parámetro en una posición específica de la lista.

_ __Parámetros:__
  * __pos:__ Se lo toma como la posición donde se desea agregar el nuevo nodo
  * __nuevo_dato:__ Es el dato que contendrá el nuevo nodo.
_ __Retornos:__
  * __True:__ El método retornará True si el nodo pudo ser agregado.
  * __False:__ El método retornará False si el nodo no pudo ser agregado.

___encontrar___
Este método dentro de la clase LSE se encarga de encontrar un nodo dentro de la lista.

- __Parámetros:__
  * __dato_buscado:__ Este parámetro es el dato que se utilizará para encontrar el nodo que lo contiene.
- __Retornos:__
    * nodo_actual: El método retornará el nodo que corresponda al dato
    buscado.
    * None: El método retornará Nodo si el nodo no pudo ser encontrado o
    no existe.

___len___
Este método dentro de la clase LSE se encarga de retornar la cantidad de nodos que se encuentren actualmente en la lista.

- __Parámetros:__
  Sin parámetros.
- __Retornos:__
  * __cont:__ El método retornará cont con la cantidad de nodos en la lista si la lista no está vacía.
  * __0:__ El método retornará 0 si la lista está vacía.

___srt___
Este método dentro de la clase LSE se encarga de retornar una cadena con todos los datos contenidos en los nodos uno detrás de otro o con un separador si en el constructor se envió uno.

_ __Parámetros:__
    Sin parámetros

- __Retornos:__
  * __cad:__ El método retornará la cadena "cad" con los datos dentro de los nodos de la lista.
  * : El método retornará un mensaje informando que no se encuentran datos en la lista si esta lista está vacía.

___iter___
 Se encarga de convertir a la lista en una lista iterable por un ciclo for.


### _Listas circulares simplemente enlazadas_

#### __Metodos__
___agregar:___
Este método dentro de la clase LCSE se encarga de agregar un nuevo nodo dentro de la lista haciendo uso de un dato u objeto que entre como parámetro.

- __Parámetros:__
    * __nuevo_dato:__ Es el dato que contendrá el nodo que se está creando.
- __Retornos:__
   * __True:__ El método retornará True si el nodo pudo ser creado.
   * __False:__ El método retornará False si el nodo no pudo ser creado.

___posicionar:___
Este método dentro de la clase LCSE se encarga de agregar un nodo con el dato que llegue como parámetro en una posición relativa específica dentro de la lista. Esta posición se determinará recorriendo la lista en círculos hasta encontrar la posición.

- __Parámetros:__
  * __pos_rel:__ Se lo toma como la posición relativa donde se desea agregar
  el nuevo nodo.
  * __nuevo_dato:__ Es el dato que contendrá el nuevo nodo.
- __Retornos:__
  * __True:__ El método retornará True si el nodo pudo ser agregado.
  * __False:__ El método retornará False si el nodo no pudo ser agregado.

___remover:___
Este método dentro de la clase LSE se encarga de remover un nodo dentro de la lista sea uno o varios a la vez.

- __Parámetros:__
  * __item:__ Este parámetro actúa de dos maneras bien sea actuando como dato para eliminar uno o todos los nodos que lo contengan, también eliminar un nodo siendo este su posición.
  * __por_pos:__ Se lo inicializa por defecto en False. Si este se vuelve True, "item" sea comporta como posición.
  * __all:__ Este parámetro actúa cuando por_pos es False. Se lo inicializa por defecto en   __False__. Si este es false, item es un dato y borra un solo nodo que lo contenga. Si este es __True__, se eliminarán todos los nodos que tengan el dato item.
- __Retornos:__
  * __True:__ El método retornará True si el nodo, o nodos, pudo ser removido
  * __False:__ El método retornará False si el nodo, o nodos, no pudo ser removido.

___Encontrar:___
Este método dentro de la clase LCSE se encarga de encontrar un nodo dentro de la lista.

- __Parámetros:__
  * __dato:__ Este parámetro es el dato que se utilizará para encontrar el nodo que lo contiene.
- __Retornos:__
  * __nodo_actual:__ El método retornará el nodo que corresponda al dato buscado.
  * __None:__ El método retornará None si el nodo no pudo ser encontrado o no existe.

___Ruleta:___
Este método dentro de la clase LCSE se encarga de encontrar un dato contenido en un nodo dentro de la lista.

- __Parámetros:__
  * __pos_rel:__ Este parámetro es la posición relativa del nodo que contenga el dato.
- __Retornos:__
  * __nodo_actual.dato:__ El método retornará el dato que corresponda al nodo buscado.
  * __None:__ El método retornará None si el nodo no pudo ser encontrado o no existe.

___Recorrer:___
Este método dentro de la clase LCSE se encarga de recorrer e imprimir los datos que se encuentren en los nodos dentro la lista.

- __Parámetros:__
    * __sep:__ Este parámetro es el separador para los datos, se inicializa por
    defecto como una cadena vacía("").
- __Retornos:__
  * __cad:__ El método retornará la cadena con los datos en ella.
  * __None:__ El método retornará None si la lista está vacía.

___len___:
Este método dentro de la clase LCSE se encarga de retornar la cantidad de nodos que se encuentren actualmente en la lista.

- __Parámetros:__
    Sin parámetros.
- __Retornos:__
  * __con:__ El método retornará cont con la cantidad de nodos en la lista si la lista no está vacía.
  * __0:__ El método retornará 0 si la lista está vacía.

___iter___:
Este método dentro de la clase LCSE se encarga de convertir a la lista en una lista iterable por un ciclo for.

- __Parámetros:__
  Sin parámetros.
- __Retornos:__
  * __IteradorLista:__ Devuelve el iterador de la lista.
