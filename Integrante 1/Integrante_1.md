# La isla del faro

Guion para cinco integrantes. 60 minutos en total.

Cada lámina dura 1:30. Cada pareja dura 3:00. Cuatro parejas por integrante suman 12:00. Los tiempos incluyen explicación, ejecución, preguntas, respuestas y cambios de pantalla. No son doce minutos de lectura continua. Ensayar con cronómetro: la narración ocupa aproximadamente 45 segundos a ritmo conversado y la acción guiada ocupa los 45 segundos restantes. Si se termina de hablar antes, usar ese margen para señalar el código y escuchar respuestas.

No leer el código carácter por carácter. Explicar qué problema resuelve, predecir, ejecutar y comparar. Tener los 20 archivos abiertos o preparados. Cada carpeta es independiente: todos los archivos se llaman Main.java y no se compilan juntos. El código de las láminas puede ser un fragmento; ejecutar siempre el archivo completo. Los comentarios indican dónde va cada fragmento.

Para ejecutar localmente, abrir una terminal dentro de la carpeta del ejemplo y usar `javac Main.java` y `java Main`. Hace falta un JDK. También puede pegarse cada Main.java completo en un editor Java en línea. En los ejemplos 12 y 20 se usa la entrada Alex. Si el editor tiene un campo de entrada estándar, escribir Alex allí antes de ejecutar.

Código visual: coral para palabras clave y tipos, turquesa para textos, amarillo para números, gris para comentarios. El color ayuda a encontrar elementos, no cambia cómo funciona Java.


# Integrante 1 · La llegada a la isla

Tiempo global 00:00 a 12:00. Láminas 1 a 8.


## Lámina 01 · La isla quedó a oscuras

Tiempo del integrante: 00:00 a 01:30. Tiempo global: 00:00 a 01:30.

### Para decir · primeros 45 segundos aproximadamente

Imaginen que llegan en una barca a una isla. Debería haber un faro para guiarlos, pero está apagado. En la playa encuentran a Lumen, un pequeño robot amarillo. Luna le dice: ayúdanos. Lumen no se mueve. Necesita instrucciones concretas. Nosotros seremos quienes se las escriban usando Java, un lenguaje de programación. En esta aventura no vamos a dibujar un videojuego, sino a construir su lógica y ver los resultados en la consola. Nuestra primera tarea es conseguir que el robot pueda avisarnos qué ocurre en la isla.

### Acción guiada · 45 segundos

0-15 s: observar la imagen. 15-30 s: escuchar dos propuestas de saludo. 30-45 s: elegir un mensaje concreto y anunciar que se probará.


## Lámina 02 · El primer mensaje

Tiempo del integrante: 01:30 a 03:00. Tiempo global: 01:30 a 03:00.

### Para decir · primeros 45 segundos aproximadamente

Este es nuestro primer diálogo con Lumen. println muestra un mensaje y después pasa a la siguiente línea. El texto está entre comillas para que Java sepa dónde empieza y dónde termina. El punto y coma cierra cada instrucción. Primero veremos Soy Lumen y luego el aviso del faro, porque estas instrucciones se ejecutan en ese orden. El archivo completo también incluye una clase Main y un método main. Por ahora usamos esa estructura como punto de inicio. Más adelante entenderemos qué son las clases y los métodos.

### Acción guiada · 45 segundos

0-15 s: ejecutar 01. 15-30 s: cambiar el primer mensaje por el saludo elegido. 30-45 s: ejecutar de nuevo y comparar el orden.


Archivo: codigo/01_llegada/Main.java

Salida prevista del archivo completo:

```text
Soy Lumen
El faro necesita ayuda
```


## Lámina 03 · La ficha de Luna

Tiempo del integrante: 03:00 a 04:30. Tiempo global: 03:00 a 04:30.

### Para decir · primeros 45 segundos aproximadamente

Lumen ya puede hablar, pero todavía no conoce a sus visitantes. Luna se presenta y cuenta que lleva dos cristales de energía en su mochila. El robot necesita recordar ambos datos. Para eso usaremos variables. Piensen en una etiqueta que nos permite encontrar un dato por su nombre. Una variable llamada nombre guardará Luna y otra llamada cristales guardará dos. El nombre de la variable lo elegimos nosotros. Conviene que explique qué contiene, porque después será mucho más fácil seguir la historia y entender el programa.

### Acción guiada · 45 segundos

0-15 s: pedir un dato del personaje. 15-30 s: decidir si es texto o número. 30-45 s: predecir qué pasa si cambia el nombre.


## Lámina 04 · Nombre y cristales

Tiempo del integrante: 04:30 a 06:00. Tiempo global: 04:30 a 06:00.

### Para decir · primeros 45 segundos aproximadamente

Aquí String indica que guardaremos texto. Su inicial es mayúscula. int indica un número entero, sin parte decimal. El signo igual asigna el valor de la derecha a la variable de la izquierda. No está haciendo una pregunta. Cuando escribimos nombre sin comillas, Java busca el valor guardado. Si lo escribimos entre comillas, mostraría literalmente la palabra nombre. Vamos a cambiar Luna por Sol y a comprobar la diferencia. El programa seguirá teniendo las mismas instrucciones, pero trabajará con otro dato.

### Acción guiada · 45 segundos

0-15 s: ejecutar 02. 15-30 s: sustituir Luna por Sol. 30-45 s: mostrar nombre entre comillas y sin comillas, y explicar la diferencia.


Archivo: codigo/02_llegada/Main.java

Salida prevista del archivo completo:

```text
Luna
2
```


## Lámina 05 · La mochila de Lumen

Tiempo del integrante: 06:00 a 07:30. Tiempo global: 06:00 a 07:30.

### Para decir · primeros 45 segundos aproximadamente

Lumen revisa su mochila antes de salir. Tiene dos cristales y sabe que el faro está a un kilómetro y medio. También revisa si lleva una llave. Estas cosas no se cuentan de la misma manera. El nombre es texto, los cristales se cuentan con enteros y la distancia puede tener decimales. La llave plantea una pregunta con dos resultados posibles: la tiene o no la tiene. Java llama boolean a ese tipo de dato. Su valor será true para verdadero o false para falso.

### Acción guiada · 45 segundos

0-15 s: nombrar los cuatro datos de la mochila. 15-30 s: pedir el tipo de cada uno. 30-45 s: preguntar qué significa false para la llave.


## Lámina 06 · Cuatro datos sencillos

Tiempo del integrante: 07:30 a 09:00. Tiempo global: 07:30 a 09:00.

### Para decir · primeros 45 segundos aproximadamente

Leamos estos datos como una ficha de viaje. String acompaña a Lumen, int a los cristales, double a la distancia y boolean a tieneLlave. En el código escribimos uno punto cinco, aunque al hablar digamos uno coma cinco. true y false no llevan comillas porque son valores booleanos. Tampoco int ni double llevan mayúscula. Hoy no necesitamos aprender todos los tipos de Java. Con estos cuatro podemos contar buena parte de nuestra aventura. Vamos a cambiar únicamente la llave para comprobar qué muestra la consola.

### Acción guiada · 45 segundos

0-15 s: ejecutar 03. 15-30 s: cambiar false por true. 30-45 s: pedir que un compañero explique qué cambió y qué datos siguen iguales.


Archivo: codigo/03_llegada/Main.java

Salida prevista del archivo completo:

```text
Lumen
2
1.5
false
```


## Lámina 07 · Un cristal en la arena

Tiempo del integrante: 09:00 a 10:30. Tiempo global: 09:00 a 10:30.

### Para decir · primeros 45 segundos aproximadamente

Antes de dejar la playa, Luna ve un brillo bajo la arena. Es otro cristal. La ficha del robot decía que tenían dos, pero ahora deben registrar tres. Aquí aparece una idea que usaremos hasta el final: los datos cambian mientras el programa avanza. Una variable no queda congelada después de crearla. Podemos leer su valor, hacer un cálculo y guardar el resultado. También podemos dejar comentarios para explicar una intención. Esos comentarios ayudan a las personas que leen el código y no producen mensajes en pantalla.

### Acción guiada · 45 segundos

0-15 s: recordar cuántos cristales había. 15-30 s: simular el hallazgo con los dedos. 30-45 s: predecir el valor y pasar al código.


## Lámina 08 · Actualizar la mochila

Tiempo del integrante: 10:30 a 12:00. Tiempo global: 10:30 a 12:00.

### Para decir · primeros 45 segundos aproximadamente

La línea cristales igual cristales más uno se entiende de derecha a izquierda: toma el dos guardado, súmale uno y guarda tres. No volvemos a escribir int porque la variable ya existe. En la última línea, el signo más une el texto con el valor para formar un mensaje. El comentario empieza con dos barras y Java lo ignora al ejecutar. Si quitáramos un punto y coma, aparecería un error de compilación. Revisar comillas, llaves y puntos y coma será parte normal de nuestras pruebas.

### Acción guiada · 45 segundos

0-15 s: ejecutar 04. 15-30 s: cambiar el aumento a 2 y predecir 4. 30-45 s: comprobar y dar paso al integrante 2: la puerta espera.


Archivo: codigo/04_llegada/Main.java

Salida prevista del archivo completo:

```text
Cristales: 3
```

