# La isla del faro

Guion para cinco integrantes. 60 minutos en total.

Cada lámina dura 1:30. Cada pareja dura 3:00. Cuatro parejas por integrante suman 12:00. Los tiempos incluyen explicación, ejecución, preguntas, respuestas y cambios de pantalla. No son doce minutos de lectura continua. Ensayar con cronómetro: la narración ocupa aproximadamente 45 segundos a ritmo conversado y la acción guiada ocupa los 45 segundos restantes. Si se termina de hablar antes, usar ese margen para señalar el código y escuchar respuestas.

No leer el código carácter por carácter. Explicar qué problema resuelve, predecir, ejecutar y comparar. Tener los 20 archivos abiertos o preparados. Cada carpeta es independiente: todos los archivos se llaman Main.java y no se compilan juntos. El código de las láminas puede ser un fragmento; ejecutar siempre el archivo completo. Los comentarios indican dónde va cada fragmento.

Para ejecutar localmente, abrir una terminal dentro de la carpeta del ejemplo y usar `javac Main.java` y `java Main`. Hace falta un JDK. También puede pegarse cada Main.java completo en un editor Java en línea. En los ejemplos 12 y 20 se usa la entrada Alex. Si el editor tiene un campo de entrada estándar, escribir Alex allí antes de ejecutar.

Código visual: coral para palabras clave y tipos, turquesa para textos, amarillo para números, gris para comentarios. El color ayuda a encontrar elementos, no cambia cómo funciona Java.


# Integrante 2 · La puerta de piedra

Tiempo global 12:00 a 24:00. Láminas 9 a 16.


## Lámina 09 · El precio del camino

Tiempo del integrante: 00:00 a 01:30. Tiempo global: 12:00 a 13:30.

### Para decir · primeros 45 segundos aproximadamente

El equipo llega a un puente vigilado por una máquina antigua. Lumen reúne cinco cristales y Sol encuentra tres más. Son ocho en total. Cruzar cuesta dos, así que quedarán seis. Las variables nos ayudaron a recordar cantidades y ahora los operadores nos permiten calcular con ellas. Son símbolos que conocen de matemáticas, aunque la multiplicación se escribe con un asterisco y la división con una barra. Vamos a revisar la cuenta antes de entregar nada. Una predicción nos ayudará a reconocer si el programa funciona como esperamos.

### Acción guiada · 45 segundos

0-15 s: hacer la suma en voz alta. 15-30 s: pedir el resultado después del pago. 30-45 s: pedir una predicción del reparto.


## Lámina 10 · Cuentas del viaje

Tiempo del integrante: 01:30 a 03:00. Tiempo global: 13:30 a 15:00.

### Para decir · primeros 45 segundos aproximadamente

Primero sumamos cinco más tres y guardamos ocho. Después restamos el precio del puente y guardamos seis en quedan. Multiplicar ese seis por dos muestra doce, y dividirlo entre dos muestra tres. Esas dos últimas líneas solo muestran cálculos: no cambian la variable quedan. Hay un detalle con los enteros: cinco dividido entre dos produce dos, porque Java descarta la parte decimal cuando ambos operandos son enteros. Para nuestro reparto de seis no hay sobrante. Probemos primero la cuenta exacta y después el caso de cinco.

### Acción guiada · 45 segundos

0-15 s: ejecutar 05. 15-30 s: cambiar la última cuenta a 5 / 2. 30-45 s: comparar 2 con 2.5 y restaurar el ejemplo.


Archivo: codigo/05_puerta/Main.java

Salida prevista del archivo completo:

```text
6
12
3
```


## Lámina 11 · La puerta de los seis cristales

Tiempo del integrante: 03:00 a 04:30. Tiempo global: 15:00 a 16:30.

### Para decir · primeros 45 segundos aproximadamente

Al otro lado del puente hay una puerta de piedra. Su letrero pide seis cristales. Luna pregunta si pueden pasar y Lumen revisa la mochila. La respuesta depende de una condición: la cantidad debe ser mayor o igual que seis. Si se cumple, la puerta se abre. Si no se cumple, el equipo tendrá que buscar más. En el programa esta elección se expresa con if y else. La computadora no inventa una decisión: sigue la condición y las instrucciones que nosotros escribimos para cada caso.

### Acción guiada · 45 segundos

0-15 s: votar si seis alcanza. 15-30 s: votar si cinco alcanza. 30-45 s: explicar por qué el igual de >= importa.


## Lámina 12 · Una decisión con if y else

Tiempo del integrante: 04:30 a 06:00. Tiempo global: 16:30 a 18:00.

### Para decir · primeros 45 segundos aproximadamente

Los paréntesis contienen la condición cristales mayor o igual que seis. Esa comparación produce true o false. Las llaves agrupan lo que ocurre en cada camino. Con seis cristales entraremos en el primer bloque. Con cinco ejecutaremos el bloque de else. También existen mayor, menor, menor o igual, doble igual para comparar igualdad y signo de admiración seguido de igual para comparar diferencia. Un solo igual asigna un valor. Dos iguales comparan. Vamos a probar los dos lados de la puerta cambiando solo el dato inicial.

### Acción guiada · 45 segundos

0-15 s: ejecutar 06 con 6. 15-30 s: ejecutar con 5. 30-45 s: ejecutar con 7 y confirmar que el límite es al menos seis.


Archivo: codigo/06_puerta/Main.java

Salida prevista del archivo completo:

```text
Puerta abierta
```


## Lámina 13 · Los tres escalones

Tiempo del integrante: 06:00 a 07:30. Tiempo global: 18:00 a 19:30.

### Para decir · primeros 45 segundos aproximadamente

La puerta se mueve y aparece una escalera de tres peldaños. Para cruzarla, Lumen debe enviar una señal en cada escalón. Podríamos copiar la misma instrucción tres veces, pero un bucle expresa mejor que estamos repitiendo una tarea. Usaremos for porque sabemos cuántas señales necesitamos. Piensen en un contador que avanza después de cada señal. La historia sigue siendo la misma, solo que ahora Java nos ayuda a repetir sin escribir una línea nueva para cada peldaño. Antes de ejecutar, vamos a recorrer el contador con las manos.

### Acción guiada · 45 segundos

0-15 s: contar los peldaños de la imagen. 15-30 s: representar 1, 2, 3 con los dedos. 30-45 s: preguntar si se imprimirá el 4.


## Lámina 14 · Contar con for

Tiempo del integrante: 07:30 a 09:00. Tiempo global: 19:30 a 21:00.

### Para decir · primeros 45 segundos aproximadamente

Dentro de los paréntesis hay tres partes. La primera crea paso con valor uno. La segunda pregunta si paso sigue siendo menor o igual que tres. Si la respuesta es verdadera, Java ejecuta el mensaje. La tercera, paso más más, aumenta el contador en uno. Luego vuelve a comprobar la condición. Cuando paso llega a cuatro, la condición falla y el bucle termina. Los puntos y coma separan esas tres partes. Vamos a cambiar el límite a cuatro y comprobar si aparece exactamente una señal adicional.

### Acción guiada · 45 segundos

0-15 s: ejecutar 07. 15-30 s: cambiar <= 3 por <= 4. 30-45 s: ejecutar, contar las líneas y explicar por qué termina.


Archivo: codigo/07_puerta/Main.java

Salida prevista del archivo completo:

```text
Escalon 1
Escalon 2
Escalon 3
```


## Lámina 15 · La batería de emergencia

Tiempo del integrante: 09:00 a 10:30. Tiempo global: 21:00 a 22:30.

### Para decir · primeros 45 segundos aproximadamente

Dentro de la escalera está oscuro. Lumen enciende su luz de emergencia, pero le quedan tres cargas de batería. Cada destello consume una. Aquí nos interesa repetir mientras quede energía. El bucle while comprueba esa condición antes de cada vuelta. Se parece a decir: mientras todavía haya batería, emite un destello. Este caso también podría resolverse con for, pero nos sirve para conocer otra manera de expresar una repetición. La diferencia práctica está en cómo organizamos el contador y la condición al escribir el código.

### Acción guiada · 45 segundos

0-15 s: representar las tres cargas con dedos. 15-30 s: bajar una por destello. 30-45 s: identificar el momento en que debe detenerse.


## Lámina 16 · La cuenta regresiva

Tiempo del integrante: 10:30 a 12:00. Tiempo global: 22:30 a 24:00.

### Para decir · primeros 45 segundos aproximadamente

Creamos batería con tres y preguntamos si es mayor que cero. Mostramos el valor y lo reducimos con dos signos menos. Así aparecen tres, dos y uno. Al llegar a cero, Java sale del bucle y muestra el mensaje final. Si olvidáramos la resta, batería seguiría valiendo tres y la condición nunca cambiaría: tendríamos un bucle infinito. No hace falta provocarlo durante la exposición. Podemos explicarlo siguiendo el valor en papel. El equipo ya superó la puerta y ahora necesita comunicarse con el faro.

### Acción guiada · 45 segundos

0-15 s: ejecutar 08. 15-30 s: cambiar la batería inicial a 1. 30-45 s: comprobar una sola vuelta y pasar al integrante 3 con la radio.


Archivo: codigo/08_puerta/Main.java

Salida prevista del archivo completo:

```text
Bateria: 3
Bateria: 2
Bateria: 1
Fin de la senal
```

