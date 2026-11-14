# La isla del faro

Guion para cinco integrantes. 60 minutos en total.

Cada lámina dura 1:30. Cada pareja dura 3:00. Cuatro parejas por integrante suman 12:00. Los tiempos incluyen explicación, ejecución, preguntas, respuestas y cambios de pantalla. No son doce minutos de lectura continua. Ensayar con cronómetro: la narración ocupa aproximadamente 45 segundos a ritmo conversado y la acción guiada ocupa los 45 segundos restantes. Si se termina de hablar antes, usar ese margen para señalar el código y escuchar respuestas.

No leer el código carácter por carácter. Explicar qué problema resuelve, predecir, ejecutar y comparar. Tener los 20 archivos abiertos o preparados. Cada carpeta es independiente: todos los archivos se llaman Main.java y no se compilan juntos. El código de las láminas puede ser un fragmento; ejecutar siempre el archivo completo. Los comentarios indican dónde va cada fragmento.

Para ejecutar localmente, abrir una terminal dentro de la carpeta del ejemplo y usar `javac Main.java` y `java Main`. Hace falta un JDK. También puede pegarse cada Main.java completo en un editor Java en línea. En los ejemplos 12 y 20 se usa la entrada Alex. Si el editor tiene un campo de entrada estándar, escribir Alex allí antes de ejecutar.

Código visual: coral para palabras clave y tipos, turquesa para textos, amarillo para números, gris para comentarios. El color ayuda a encontrar elementos, no cambia cómo funciona Java.


# Integrante 3 · La radio del guardián

Tiempo global 24:00 a 36:00. Láminas 17 a 24.


## Lámina 17 · La radio del guardián

Tiempo del integrante: 00:00 a 01:30. Tiempo global: 24:00 a 25:30.

### Para decir · primeros 45 segundos aproximadamente

Después de cruzar la escalera, Sol encuentra una radio. El guardián del faro podría escucharlos, pero la señal necesita un mensaje claro. Lumen prepara una acción llamada pedirAyuda. Un método es un bloque de instrucciones con nombre. Nos permite guardar una acción para usarla desde distintos lugares del programa. Definir el método se parece a escribir una receta. Llamarlo se parece a preparar esa receta. La receta no se cocina sola por estar escrita. Del mismo modo, el mensaje solo aparecerá cuando el programa llame al método.

### Acción guiada · 45 segundos

0-15 s: proponer un mensaje corto para la radio. 15-30 s: separar preparar de ejecutar. 30-45 s: predecir cuántas líneas saldrán.


## Lámina 18 · Crear y llamar un método

Tiempo del integrante: 01:30 a 03:00. Tiempo global: 25:30 a 27:00.

### Para decir · primeros 45 segundos aproximadamente

Aquí definimos pedirAyuda fuera de main, pero dentro de Main. Después, dentro de main, lo llamamos dos veces. Por eso el mismo mensaje aparecerá dos veces. void indica que el método no devuelve un resultado. En este ejemplo realiza una acción visible: imprimir. static permite llamar a este método desde main sin crear un objeto de Main. Por ahora conservaremos esa forma para estos métodos auxiliares. Los comentarios de la lámina indican dónde va cada fragmento. El archivo completo ya tiene todo en su lugar.

### Acción guiada · 45 segundos

0-15 s: ejecutar 09 completo. 15-30 s: quitar una llamada, sin borrar la definición. 30-45 s: ejecutar y comparar las dos salidas.


Archivo: codigo/09_radio/Main.java

Salida prevista del archivo completo:

```text
Equipo en camino
Equipo en camino
```


## Lámina 19 · Un mensaje para cada explorador

Tiempo del integrante: 03:00 a 04:30. Tiempo global: 27:00 a 28:30.

### Para decir · primeros 45 segundos aproximadamente

El guardián responde por la radio: ¿quién está hablando? Luna y Sol necesitan presentarse por separado. En lugar de crear un método distinto para cada persona, podemos darle un dato al mismo método. Ese espacio para recibir un dato se llama parámetro. Imaginen una tarjeta con un hueco para escribir el nombre de quien llama. Las palabras del saludo siguen siendo las mismas, pero el nombre cambia. Esto nos permite reutilizar una acción sin que todos los mensajes tengan que ser idénticos.

### Acción guiada · 45 segundos

0-15 s: pedir dos nombres para la radio. 15-30 s: señalar el hueco nombre. 30-45 s: anticipar las dos respuestas.


## Lámina 20 · Un método con parámetro

Tiempo del integrante: 04:30 a 06:00. Tiempo global: 28:30 a 30:00.

### Para decir · primeros 45 segundos aproximadamente

El método saludar recibe un String llamado nombre. Cuando escribimos saludar con Luna entre paréntesis, enviamos Luna como argumento. En esa llamada, nombre vale Luna. Cuando llamamos con Sol, nombre vale Sol. El tipo que recibe el método debe corresponder al dato que enviamos. Aquí queremos texto. Si intentamos llamar a saludar sin ningún dato, Java nos avisará que falta el argumento. Primero observemos las dos llamadas correctas. Después cambiaremos uno de los nombres para escuchar al público en nuestra radio.

### Acción guiada · 45 segundos

0-15 s: ejecutar 10. 15-30 s: sustituir Sol por el nombre elegido. 30-45 s: ejecutar y señalar parámetro en la definición y argumento en la llamada.


Archivo: codigo/10_radio/Main.java

Salida prevista del archivo completo:

```text
Adelante, Luna
Adelante, Sol
```


## Lámina 21 · El cálculo del guardián

Tiempo del integrante: 06:00 a 07:30. Tiempo global: 30:00 a 31:30.

### Para decir · primeros 45 segundos aproximadamente

El guardián pregunta cuánta energía trae el equipo. Luna tiene cuatro unidades y Sol tiene tres. Hasta ahora nuestros métodos mostraban mensajes. Ahora queremos uno que calcule un dato y nos lo entregue para usarlo después. Piensen en una calculadora: escribimos dos números y recibimos un resultado. Ese resultado puede guardarse, compararse o mostrarse. En Java, return entrega el resultado de un método a la parte del programa que lo llamó. Así podremos usar un mismo cálculo sin obligarlo a imprimir siempre un mensaje.

### Acción guiada · 45 segundos

0-15 s: sumar cuatro y tres mentalmente. 15-30 s: preguntar dónde guardarían el resultado. 30-45 s: distinguir entregar un dato de decirlo en voz alta.


## Lámina 22 · Un método que devuelve un número

Tiempo del integrante: 07:30 a 09:00. Tiempo global: 31:30 a 33:00.

### Para decir · primeros 45 segundos aproximadamente

En la definición cambiamos void por int porque devolveremos un entero. Los parámetros a y b reciben cuatro y tres. return calcula la suma y entrega siete. Después guardamos ese siete en total. La última línea lo muestra en consola. Si quitáramos println, el cálculo todavía se haría, pero no veríamos el mensaje. Esa diferencia es importante: devolver un dato no significa mostrarlo. Vamos a cambiar los números y a predecir el resultado antes de ejecutar. Más adelante usaremos un resultado para decidir si encendemos el faro.

### Acción guiada · 45 segundos

0-15 s: ejecutar 11. 15-30 s: cambiar a sumar(2, 5). 30-45 s: ejecutar y comentar por qué sigue dando 7.


Archivo: codigo/11_radio/Main.java

Salida prevista del archivo completo:

```text
Total: 7
```


## Lámina 23 · Tu nombre entra en la aventura

Tiempo del integrante: 09:00 a 10:30. Tiempo global: 33:00 a 34:30.

### Para decir · primeros 45 segundos aproximadamente

La voz de la radio se escucha con claridad. Ahora el guardián quiere conocer a quien nos está ayudando desde el público. Hasta este momento todos los datos estaban escritos dentro del programa. Scanner permite leer información que una persona introduce al ejecutarlo. Eso vuelve la conversación interactiva. Nuestro ejemplo pedirá un nombre y lo usará en una bienvenida. En un editor con entrada preparada, escribiremos el nombre en el campo de entrada antes de ejecutar. En una terminal, lo escribiremos cuando aparezca la pregunta.

### Acción guiada · 45 segundos

0-15 s: elegir un nombre del público. 15-30 s: localizar dónde se escribe la entrada en el editor. 30-45 s: anticipar el saludo completo.


## Lámina 24 · Leer una línea de texto

Tiempo del integrante: 10:30 a 12:00. Tiempo global: 34:30 a 36:00.

### Para decir · primeros 45 segundos aproximadamente

El archivo completo empieza importando Scanner para poder usarlo. Creamos entrada conectada a System.in, que representa la entrada estándar. Después mostramos una pregunta. nextLine lee una línea completa y guarda ese texto en nombre. Finalmente lo unimos al saludo y cerramos el lector al terminar. Para la primera prueba usaremos Alex, por eso esa es la salida prevista. Con otro nombre, el saludo cambiará. Solo leeremos texto para mantener este primer ejemplo sencillo. Ya podemos enviar datos, recibirlos y organizar acciones con métodos.

### Acción guiada · 45 segundos

0-15 s: ejecutar 12 con Alex como entrada. 15-30 s: repetir con el nombre elegido. 30-45 s: señalar el cambio y pasar al integrante 4, que construirá robots.


Archivo: codigo/12_radio/Main.java

Salida prevista del archivo completo:

```text
Tu nombre:
Bienvenido, Alex
```

