# La isla del faro

Guion para cinco integrantes. 60 minutos en total.

Cada lámina dura 1:30. Cada pareja dura 3:00. Cuatro parejas por integrante suman 12:00. Los tiempos incluyen explicación, ejecución, preguntas, respuestas y cambios de pantalla. No son doce minutos de lectura continua. Ensayar con cronómetro: la narración ocupa aproximadamente 45 segundos a ritmo conversado y la acción guiada ocupa los 45 segundos restantes. Si se termina de hablar antes, usar ese margen para señalar el código y escuchar respuestas.

No leer el código carácter por carácter. Explicar qué problema resuelve, predecir, ejecutar y comparar. Tener los 20 archivos abiertos o preparados. Cada carpeta es independiente: todos los archivos se llaman Main.java y no se compilan juntos. El código de las láminas puede ser un fragmento; ejecutar siempre el archivo completo. Los comentarios indican dónde va cada fragmento.

Para ejecutar localmente, abrir una terminal dentro de la carpeta del ejemplo y usar `javac Main.java` y `java Main`. Hace falta un JDK. También puede pegarse cada Main.java completo en un editor Java en línea. En los ejemplos 12 y 20 se usa la entrada Alex. Si el editor tiene un campo de entrada estándar, escribir Alex allí antes de ejecutar.

Código visual: coral para palabras clave y tipos, turquesa para textos, amarillo para números, gris para comentarios. El color ayuda a encontrar elementos, no cambia cómo funciona Java.


# Integrante 4 · El taller de robots

Tiempo global 36:00 a 48:00. Láminas 25 a 32.


## Lámina 25 · El taller de robots

Tiempo del integrante: 00:00 a 01:30. Tiempo global: 36:00 a 37:30.

### Para decir · primeros 45 segundos aproximadamente

La radio funciona, pero el faro tiene dos controles muy separados. Lumen no puede estar en ambos a la vez. El guardián nos lleva a un taller para construir otro robot. Aquí aprenderemos a describir objetos con clases. La clase Robot reúne los datos y las acciones que tendrán nuestros robots. Podemos imaginarla como un plano de construcción. Un objeto será un robot concreto creado con ese plano. El plano puede servir muchas veces, mientras que cada robot guarda sus propios datos durante la ejecución.

### Acción guiada · 45 segundos

0-15 s: señalar el robot de la imagen. 15-30 s: pedir un dato y una acción posibles. 30-45 s: distinguir el plano del robot construido.


## Lámina 26 · La clase y su constructor

Tiempo del integrante: 01:30 a 03:00. Tiempo global: 37:30 a 39:00.

### Para decir · primeros 45 segundos aproximadamente

La palabra class inicia la descripción. Dentro aparece nombre, que ahora es un atributo: un dato que pertenece a cada objeto. Robot, escrito igual que la clase y sin tipo de retorno, es el constructor. Recibe un nombre en n y lo guarda en el atributo. El constructor se ejecuta al crear el objeto. Esta lámina muestra la clase que necesitamos entender. En el archivo completo, main crea a Lumen y muestra su nombre. En la siguiente pareja veremos con más detalle esa creación y construiremos dos robots.

### Acción guiada · 45 segundos

0-15 s: abrir 13 y localizar class Robot. 15-30 s: ejecutar el archivo completo. 30-45 s: seguir el texto Lumen desde el constructor hasta nombre.


Archivo: codigo/13_robots/Main.java

Salida prevista del archivo completo:

```text
Lumen
```


## Lámina 27 · Lumen conoce a Chispa

Tiempo del integrante: 03:00 a 04:30. Tiempo global: 39:00 a 40:30.

### Para decir · primeros 45 segundos aproximadamente

El segundo robot sale del taller y decide llamarse Chispa. Los dos comparten la clase Robot, pero cada uno guarda un nombre diferente. Eso es lo útil de los objetos: podemos representar varias cosas del mismo tipo sin confundir sus datos. También pueden tener acciones. La acción presentarse usará el nombre del robot que la ejecuta. Si Lumen se presenta, escucharemos Lumen. Si lo hace Chispa, escucharemos Chispa. El método tiene las mismas instrucciones, pero trabaja con los datos del objeto correspondiente.

### Acción guiada · 45 segundos

0-15 s: asignar un nombre a cada robot de la imagen. 15-30 s: pedir dos voluntarios que se presenten. 30-45 s: explicar qué comparten y qué es distinto.


## Lámina 28 · Dos objetos y una acción

Tiempo del integrante: 04:30 a 06:00. Tiempo global: 40:30 a 42:00.

### Para decir · primeros 45 segundos aproximadamente

new crea un objeto y llama a su constructor. Guardamos la referencia al primero en uno y al segundo en dos. El punto permite pedirle una acción a un objeto: uno punto presentarse llama al método del primer robot. Aquí no escribimos static en presentarse, porque la acción usa el nombre propio de cada robot. Los comentarios separan los lugares del fragmento. No hay que pegar esas piezas juntas dentro de main: el archivo completo ya organiza la clase Robot y la clase Main correctamente.

### Acción guiada · 45 segundos

0-15 s: ejecutar 14. 15-30 s: cambiar Chispa por Brisa. 30-45 s: ejecutar y confirmar que el primer nombre permanece igual.


Archivo: codigo/14_robots/Main.java

Salida prevista del archivo completo:

```text
Soy Lumen
Soy Chispa
```


## Lámina 29 · La energía bajo cuidado

Tiempo del integrante: 06:00 a 07:30. Tiempo global: 42:00 a 43:30.

### Para decir · primeros 45 segundos aproximadamente

Lumen y Chispa ya pueden presentarse. Ahora revisaremos su energía. Si cualquier parte del programa pudiera cambiarla sin cuidado, podríamos terminar con valores absurdos. Vamos a guardar ese dato dentro de Robot y a limitar su acceso directo con private. Esta es una primera idea de encapsulación: el objeto reúne sus datos con las operaciones que permiten usarlos. Piensen en un medidor de batería. Pueden consultar el nivel, pero la lectura no exige abrir el robot y tocar sus componentes internos.

### Acción guiada · 45 segundos

0-15 s: imaginar el medidor de batería. 15-30 s: preguntar si consultar implica modificar. 30-45 s: localizar qué elemento debe permanecer bajo control.


## Lámina 30 · Consultar con un getter

Tiempo del integrante: 07:30 a 09:00. Tiempo global: 43:30 a 45:00.

### Para decir · primeros 45 segundos aproximadamente

El atributo energía empieza en tres y es private. Main no puede leerlo directamente con robot punto energía. En cambio, puede llamar a getEnergia, un método que devuelve el valor. A este tipo de método de consulta lo llamamos getter por convención. No es una palabra especial de Java. En este ejemplo no escribimos constructor, así que Java proporciona uno sin argumentos. Usamos new Robot con paréntesis vacíos. private controla el acceso desde el código de otras clases. No significa cifrar el dato ni crear una contraseña.

### Acción guiada · 45 segundos

0-15 s: ejecutar 15. 15-30 s: cambiar la energía inicial a 5 dentro de Robot. 30-45 s: ejecutar y comprobar que el getter devuelve 5.


Archivo: codigo/15_robots/Main.java

Salida prevista del archivo completo:

```text
3
```


## Lámina 31 · Una recarga con reglas

Tiempo del integrante: 09:00 a 10:30. Tiempo global: 45:00 a 46:30.

### Para decir · primeros 45 segundos aproximadamente

El guardián conecta el cargador de Lumen. La batería admite valores desde cero hasta cien. Queremos permitir una recarga, pero con una regla que impida guardar energía negativa o superior al límite. Para eso crearemos un método que recibe el nuevo valor y decide si lo acepta. A esta clase de método de cambio la solemos llamar setter. La validación es una decisión de nuestro diseño: Java no la añade automáticamente por ponerle ese nombre. Vamos a construirla con el if que ya conocemos.

### Acción guiada · 45 segundos

0-15 s: votar si 8 está permitido. 15-30 s: votar si -2 está permitido. 30-45 s: predecir el valor después de ambos intentos.


## Lámina 32 · Cambiar con una validación

Tiempo del integrante: 10:30 a 12:00. Tiempo global: 46:30 a 48:00.

### Para decir · primeros 45 segundos aproximadamente

setEnergia recibe nueva. La condición pregunta si nueva es mayor o igual que cero y también menor o igual que cien. Los dos símbolos de ampersand significan que ambas comparaciones deben cumplirse. Si el dato es válido, lo guardamos. Si es inválido, el método termina sin cambiar la energía. Primero asignamos ocho. Después intentamos menos dos. Al consultar, seguiremos viendo ocho. El getter permite observar el resultado de la regla. En el último capítulo reuniremos varios robots y usaremos su energía para decidir si el faro puede encenderse.

### Acción guiada · 45 segundos

0-15 s: ejecutar 16. 15-30 s: reemplazar -2 por 101 y comprobar que sigue en 8. 30-45 s: restaurar y pasar al integrante 5 con los robots listos.


Archivo: codigo/16_robots/Main.java

Salida prevista del archivo completo:

```text
8
```
