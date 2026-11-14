# La isla del faro

Guion para cinco integrantes. 60 minutos en total.

Cada lámina dura 1:30. Cada pareja dura 3:00. Cuatro parejas por integrante suman 12:00. Los tiempos incluyen explicación, ejecución, preguntas, respuestas y cambios de pantalla. No son doce minutos de lectura continua. Ensayar con cronómetro: la narración ocupa aproximadamente 45 segundos a ritmo conversado y la acción guiada ocupa los 45 segundos restantes. Si se termina de hablar antes, usar ese margen para señalar el código y escuchar respuestas.

No leer el código carácter por carácter. Explicar qué problema resuelve, predecir, ejecutar y comparar. Tener los 20 archivos abiertos o preparados. Cada carpeta es independiente: todos los archivos se llaman Main.java y no se compilan juntos. El código de las láminas puede ser un fragmento; ejecutar siempre el archivo completo. Los comentarios indican dónde va cada fragmento.

Para ejecutar localmente, abrir una terminal dentro de la carpeta del ejemplo y usar `javac Main.java` y `java Main`. Hace falta un JDK. También puede pegarse cada Main.java completo en un editor Java en línea. En los ejemplos 12 y 20 se usa la entrada Alex. Si el editor tiene un campo de entrada estándar, escribir Alex allí antes de ejecutar.

Código visual: coral para palabras clave y tipos, turquesa para textos, amarillo para números, gris para comentarios. El color ayuda a encontrar elementos, no cambia cómo funciona Java.


# Integrante 5 · La luz del faro

Tiempo global 48:00 a 60:00. Láminas 33 a 40.


## Lámina 33 · La lista de la expedición

Tiempo del integrante: 00:00 a 01:30. Tiempo global: 48:00 a 49:30.

### Para decir · primeros 45 segundos aproximadamente

Estamos frente al faro. Antes de subir, el guardián revisa quiénes forman parte de la expedición. Podríamos tener una variable para cada nombre, pero un arreglo nos permite reunir varios valores del mismo tipo. En este primer ejemplo guardaremos textos. Imaginen una fila de espacios numerados. En Java, el primer espacio tiene índice cero y el segundo índice uno. El índice es la posición que escribimos para acceder a un elemento. Que empiece en cero no cambia cuántas personas hay: siguen siendo dos.

### Explicación didáctica · 45 segundos

Para entenderlo mejor, imaginemos una estantería con varios casilleros. Cada casillero tiene un número que indica dónde encontrar lo que guardamos. En programación funciona de manera parecida: podemos guardar varios datos dentro de un mismo arreglo y acceder a cada uno mediante su posición.

La ventaja es que no necesitamos crear una variable diferente para cada integrante de la expedición. Además, cuando trabajamos con arreglos, podemos organizar los datos y recorrerlos más adelante.

Hay que distinguir dos conceptos: **el índice indica dónde está un elemento, mientras que el tamaño indica cuántos elementos tenemos**. En Java utilizamos `length` para conocer ese tamaño.


## Lámina 34 · Los nombres en un arreglo

Tiempo del integrante: 01:30 a 03:00. Tiempo global: 49:30 a 51:00.

### Para decir · primeros 45 segundos aproximadamente

Los corchetes junto a String indican un arreglo de textos. Las llaves contienen Luna y Sol, separados por una coma. nombres con corchetes cero devuelve Luna. Con uno devuelve Sol. length nos dice que hay dos elementos. El último índice válido es uno porque empezamos a contar posiciones en cero. Si intentáramos leer nombres dos, el programa fallaría al ejecutarse porque esa posición no existe. Hoy evitaremos ese acceso y comprobaremos las posiciones válidas. El tamaño de este arreglo queda fijado al crearlo.

### Acción guiada · 45 segundos

0-15 s: ejecutar 17. 15-30 s: añadir Alex al final del arreglo y mostrar nombres[2]. 30-45 s: comprobar que length ahora muestra 3.


Archivo: codigo/17_faro/Main.java

Salida prevista del archivo completo:

```text
Luna
Sol
2
```


## Lámina 35 · El pase de lista

Tiempo del integrante: 03:00 a 04:30. Tiempo global: 51:00 a 52:30.

### Para decir · primeros 45 segundos aproximadamente

El guardián empieza a pasar lista. Con dos nombres podríamos escribir dos instrucciones, pero si mañana llega alguien más tendríamos que añadir otra. Un recorrido permite hacer la misma tarea con cada elemento. Usaremos la forma for-each. Al hablar podemos leerla así: para cada nombre dentro de nombres, muestra que está presente. Esta forma resulta cómoda cuando queremos visitar los elementos del arreglo en orden y no necesitamos conocer su índice. Vamos a usarla primero con personas y después con los robots.

### Explicación didáctica · 45 segundos

En programación existen unas estructuras llamadas bucles, que sirven para repetir instrucciones sin tener que escribirlas muchas veces.

Podemos imaginar un bucle como una cinta transportadora: los elementos pasan uno por uno y a cada uno se le aplica la misma instrucción. Cada repetición se conoce como una **iteración**.

El `for-each` es un tipo de bucle especialmente útil para recorrer arreglos. Durante cada iteración toma un elemento y lo coloca temporalmente en una variable para que podamos trabajar con él.

Cuando termina de recorrer todos los elementos, el bucle finaliza automáticamente. Así podemos procesar listas pequeñas o grandes utilizando prácticamente las mismas instrucciones.


## Lámina 36 · Recorrer los nombres

Tiempo del integrante: 04:30 a 06:00. Tiempo global: 52:30 a 54:00.

### Para decir · primeros 45 segundos aproximadamente

La variable nombres contiene el arreglo completo. La variable nombre, en singular, recibe un texto en cada vuelta. Primero recibe Luna y después Sol. Los dos puntos separan esa variable del arreglo que recorremos. Aquí no escribimos paso más más ni una comparación, porque esta forma de for visita los elementos disponibles. Si añadimos Alex a la lista, el mismo bucle lo saludará en una vuelta adicional. Seguimos teniendo un arreglo de tamaño fijo: al editar su declaración y ejecutar otra vez, creamos un arreglo nuevo.

### Acción guiada · 45 segundos

0-15 s: ejecutar 18. 15-30 s: agregar Alex al arreglo. 30-45 s: ejecutar y contar tres saludos sin cambiar el bucle.


Archivo: codigo/18_faro/Main.java

Salida prevista del archivo completo:

```text
Presente: Luna
Presente: Sol
```


## Lámina 37 · Dos robots para el faro

Tiempo del integrante: 06:00 a 07:30. Tiempo global: 54:00 a 55:30.

### Para decir · primeros 45 segundos aproximadamente

El pase de lista termina y Lumen se coloca junto a Chispa. Ahora vamos a reunir objetos en vez de textos. La idea del arreglo sigue siendo la misma, pero su tipo será Robot. Cada elemento permite acceder a un robot con su nombre y su energía. Conservamos lo aprendido sobre clases, constructores y métodos. Para esta versión, el constructor recibirá dos datos: nombre y energía inicial. Cuatro unidades de Lumen y tres de Chispa podrían ser suficientes para encender el faro. Primero necesitamos comprobar lo que aporta cada uno.

### Explicación didáctica · 45 segundos

Recordemos que una clase es como un molde que nos permite crear objetos. Por ejemplo, la clase `Robot` define qué características y comportamientos pueden tener nuestros robots.

Con ese mismo molde podemos crear a Lumen y Chispa. Aunque pertenecen a la misma clase, cada uno es un objeto independiente, con sus propios datos.

Hasta ahora habíamos utilizado un arreglo para guardar textos, pero también podemos guardar referencias a objetos. De esta manera, un solo arreglo puede reunir a todos nuestros robots.

Esto es útil porque podemos organizar un equipo completo y utilizar un bucle para consultar las características de cada integrante sin escribir instrucciones individuales para todos.


## Lámina 38 · Un arreglo de objetos

Tiempo del integrante: 07:30 a 09:00. Tiempo global: 55:30 a 57:00.

### Para decir · primeros 45 segundos aproximadamente

Creamos dos objetos dentro del arreglo equipo. Cada new llama al constructor con su nombre y su energía. La clase completa usa el setter para revisar la energía inicial y conserva los atributos privados. Después el for-each toma un robot en cada vuelta. Le pide que se presente y consulta su energía con el getter. El punto se refiere al robot de esa vuelta. Si cambiamos solo la energía de Chispa, la de Lumen seguirá siendo cuatro. Estamos combinando piezas pequeñas que ya practicamos por separado.

### Acción guiada · 45 segundos

0-15 s: ejecutar 19. 15-30 s: cambiar la energía de Chispa a 2. 30-45 s: comprobar que Lumen conserva 4 y restaurar Chispa a 3.


Archivo: codigo/19_faro/Main.java

Salida prevista del archivo completo:

```text
Soy Lumen
4
Soy Chispa
3
```


## Lámina 39 · La luz vuelve a la isla

Tiempo del integrante: 09:00 a 10:30. Tiempo global: 57:00 a 58:30.

### Para decir · primeros 45 segundos aproximadamente

Luna y Sol llegan a la parte alta del faro. Conectan a Lumen y Chispa y observan el medidor. No vamos a adivinar si alcanza la energía: el programa la sumará y tomará la decisión. Este cierre combina variables, un método con parámetro, entrada de texto, clases, objetos, un arreglo, un recorrido y una condición. No aparece una herramienta misteriosa al final. Cada pieza viene de un capítulo anterior. El faro se encenderá con siete unidades o más, así que podremos probar tanto el éxito como la falta de energía.

### Explicación didáctica · 45 segundos

Este último desafío nos permite comprender cómo funciona un algoritmo. Un algoritmo es una secuencia ordenada de pasos que seguimos para resolver un problema.

En nuestro caso, podemos dividirlo en tres partes: **obtener los datos, procesarlos y mostrar un resultado**.

Primero obtenemos la energía de cada robot. Después utilizamos un bucle para sumar esos valores. Finalmente, una condición `if` permite que el programa decida qué mensaje mostrar.

La condición funciona como una pregunta de verdadero o falso. Si la energía alcanza el mínimo requerido, encendemos el faro; de lo contrario, mostramos que falta energía.

Así combinamos distintas herramientas de Java para resolver un único problema.


## Lámina 40 · La decisión final

Tiempo del integrante: 10:30 a 12:00. Tiempo global: 58:30 a 60:00.

### Para decir · primeros 45 segundos aproximadamente

total empieza en cero. En cada vuelta le sumamos la energía del robot actual. Después de Lumen vale cuatro y después de Chispa vale siete. El if compara ese total con el mínimo. En el programa completo, Scanner también lee nuestro nombre y saludar lo agradece usando un parámetro. La lámina muestra únicamente el cálculo final para poder leerlo con calma. Primero ejecutaremos con cuatro y tres. Después bajaremos Chispa a dos. Si obtenemos ambos mensajes según los datos, tendremos una comprobación útil del comportamiento y la historia habrá llegado al faro.

### Acción guiada · 45 segundos

0-15 s: ejecutar 20 con Alex. 15-30 s: cambiar Chispa a 2 y ejecutar otra vez. 30-40 s: comprobar Falta energia. 40-45 s: cerrar: hoy ustedes guiaron la aventura.


Archivo: codigo/20_faro/Main.java

Salida prevista del archivo completo:

```text
Tu nombre:
Gracias, Alex
Energia total: 7
Faro encendido
```
