# Enunciados

### 1. El despertar de Chip
La mascota del taller, un pequeño robot llamado **Chip**, se enciende por primera vez. Lo primero que quiere hacer es saludar al mundo entero.

**Entrada:** no hay.

**Salida:** una línea con el saludo de Chip.

**Ejemplo**

*Salida:*
```
¡Hola, mundo!
```

---

### 2. La primera escalera
Animado, Chip aprende a dibujar con asteriscos. Su primer dibujo es una escalera de tres escalones, cada uno un asterisco más alto que el anterior.

**Entrada:** no hay.

**Salida:** tres líneas formando la escalera.

**Ejemplo**

*Salida:*
```
*
**
***
```

---

### 3. La cuenta regresiva
En la línea de partida de una carrera de robots, el juez grita la cuenta regresiva antes de la largada: tres, dos, uno… ¡ya! Imprime los tres números en una sola línea, separados por un espacio.

**Entrada:** no hay.

**Salida:** una línea con `3 2 1`.

**Ejemplo**

*Salida:*
```
3 2 1
```

---

### 4. El casillero
En el gimnasio hay un casillero inteligente: le dices un número y él lo muestra en su pantallita para que no lo olvides.

**Entrada:** un entero `n` (`0 ≤ n ≤ 1000`).

**Salida:** la línea `El número guardado es n`.

**Ejemplo**

*Entrada:*
```
25
```
*Salida:*
```
El número guardado es 25
```

---

### 5. El truco del mago
El mago Zoltán recibe dos cartas con números. Para su truco, siempre las muestra **al revés**: primero la segunda y luego la primera.

**Entrada:** dos enteros `a` y `b`.

**Salida:** los dos números en orden inverso, separados por un espacio.

**Ejemplo**

*Entrada:*
```
8
3
```
*Salida:*
```
3 8
```

---

### 6. Dos cofres
Un pirata encuentra dos cofres de monedas. Quiere saber cuántas monedas tiene en total.

**Entrada:** dos enteros `a` y `b`, las monedas de cada cofre.

**Salida:** el total de monedas.

**Ejemplo**

*Entrada:*
```
4
5
```
*Salida:*
```
9
```

---

### 7. Las galletas que quedan
Tenías un frasco con `a` galletas y te comiste `b`. ¿Cuántas quedan en el frasco?

**Entrada:** dos enteros `a` y `b` (`a ≥ b`).

**Salida:** las galletas restantes (`a - b`).

**Ejemplo**

*Entrada:*
```
10
3
```
*Salida:*
```
7
```

---

### 8. La caja de chocolates
Una caja acomoda los chocolates en `f` filas y `c` columnas. ¿Cuántos chocolates entran en total?

**Entrada:** dos enteros `f` y `c`.

**Salida:** la cantidad total de chocolates.

**Ejemplo**

*Entrada:*
```
6
7
```
*Salida:*
```
42
```

---

### 9. El reparto justo
Tienes `n` caramelos y quieres repartirlos en partes **iguales** entre `k` amigos. Los que sobren quedan en la bolsa. ¿Cuántos caramelos recibe cada amigo?

**Entrada:** dos enteros `n` y `k` (`k ≥ 1`).

**Salida:** los caramelos que recibe cada amigo (división entera `n / k`).

**Ejemplo**

*Entrada:*
```
7
2
```
*Salida:*
```
3
```

---

### 10. Lo que sobra
Misma bolsa del problema anterior: repartes `n` caramelos en partes iguales entre `k` amigos. Ahora la pregunta es: ¿cuántos caramelos **sobran** en la bolsa?

**Entrada:** dos enteros `n` y `k` (`k ≥ 1`).

**Salida:** los caramelos que sobran (residuo `n % k`).

**Ejemplo**

*Entrada:*
```
7
2
```
*Salida:*
```
1
```

---

### 11. El patio cuadrado
Quieres embaldosar un patio **cuadrado** de `n` metros de lado, usando baldosas de 1 metro por 1 metro. ¿Cuántas baldosas necesitas?

**Entrada:** un entero `n`.

**Salida:** la cantidad de baldosas (`n × n`).

**Ejemplo**

*Entrada:*
```
5
```
*Salida:*
```
25
```

---

### 12. El marco de la foto
Quieres ponerle un marco a una foto rectangular de `l` cm de largo y `a` cm de ancho. La cinta del marco debe rodear toda la foto. ¿Cuántos centímetros de cinta necesitas?

**Entrada:** dos enteros `l` y `a`.

**Salida:** el perímetro `2 * (l + a)`.

**Ejemplo**

*Entrada:*
```
5
3
```
*Salida:*
```
16
```

---

### 13. Empalmando cintas
En el taller hay dos trozos de cinta que miden `a` y `b` metros (pueden tener decimales). Si los unes, ¿cuánto mide la cinta resultante?

**Entrada:** dos números decimales `a` y `b`.

**Salida:** la suma `a + b`.

**Ejemplo**

*Entrada:*
```
2.5
1.75
```
*Salida:*
```
4.25
```

---

### 14. Mitad y mitad
Dos amigos juntan sus puntajes `a` y `b` (enteros) en un videojuego y quieren saber el **promedio** exacto, aunque dé con decimales.

**Entrada:** dos enteros `a` y `b`.

**Salida:** el promedio `(a + b) / 2.0` (conservando decimales).

**Ejemplo**

*Entrada:*
```
5
2
```
*Salida:*
```
3.5
```

---

### 15. El cronómetro
Un cronómetro marcó `S` segundos en total. Quieres expresarlo como minutos completos y segundos sobrantes.

**Entrada:** un entero `S` (`0 ≤ S ≤ 10000`).

**Salida:** dos líneas: primero los minutos completos (`S / 60`) y luego los segundos sobrantes (`S % 60`).

**Ejemplo**

*Entrada:*
```
130
```
*Salida:*
```
2
10
```

---

### 16. La pizza gigante
Una pizzería ofrece una pizza circular de radio `r`. Para cobrarla necesitan su área. Usa `3.14` como valor de pi: `área = 3.14 * r * r`.

**Entrada:** un entero `r`.

**Salida:** el área de la pizza.

**Ejemplo**

*Entrada:*
```
2
```
*Salida:*
```
12.56
```

---

### 17. El kiosco
En el kiosco compras `cantidad` unidades de un producto que cuesta `precio` cada una, y pagas con un billete de `pago` pesos (siempre alcanza). El kiosquero quiere imprimir el total de la compra y tu vuelto.

**Entrada:** tres enteros: `cantidad`, `precio` y `pago`.

**Salida:** dos líneas: el total (`cantidad * precio`) y el vuelto (`pago - total`).

**Ejemplo**

*Entrada:*
```
3
500
2000
```
*Salida:*
```
1500
500
```

---

### 18. Ficha de jugador
Un videojuego arma la ficha de un personaje. Lee su `nombre` (una palabra) y sus tres atributos: `ataque`, `defensa` y `velocidad`. Su **poder total** es la suma de los tres.

**Entrada:** una palabra `nombre` y tres enteros `ataque`, `defensa`, `velocidad`.

**Salida:** dos líneas: `Jugador: nombre` y `Poder total: suma`.

**Ejemplo**

*Entrada:*
```
Aria
30
20
10
```
*Salida:*
```
Jugador: Aria
Poder total: 60
```

---

### 19. Reporte de fin de temporada (final)
Al cerrar la temporada, el juego genera el reporte de un explorador. Lee, **en este orden exacto**:

1. `nombre` — el nombre del explorador (una palabra).
2. `mapas` — cuántos mapas completó (entero).
3. `totales` — cuántos mapas tiene el juego (entero, `totales ≥ mapas`).
4. `p1`, `p2`, `p3` — los puntajes de tres desafíos (tres enteros).
5. `bonus` — un puntaje extra que puede tener decimales (decimal).
6. `minutos` — el total de minutos jugados (entero).

Luego imprime **exactamente** estas ocho líneas:

1. `Explorador: ` y el nombre.
2. `Mapas: ` los completados, ` de `, el total, ` mapas`.
3. `Faltan: ` los que faltan (`totales - mapas`) y ` mapas`.
4. `Puntos por mapas: ` los completados por 10.
5. `Suma de desafios: ` la suma de los tres puntajes.
6. `Bonus: ` el puntaje extra.
7. `Promedio (3 desafios y bonus): ` el promedio de los cuatro valores `(suma + bonus) / 4.0` (con decimales).
8. `Tiempo de juego: ` las horas completas (`minutos / 60`), ` h y `, los minutos sobrantes (`minutos % 60`) y ` min`.

**Entrada:** los datos en el orden indicado arriba.

**Salida:** las ocho líneas del reporte.

**Ejemplo**

*Entrada:*
```
Nico
42
50
60
70
50
78.5
145
```
*Salida:*
```
Explorador: Nico
Mapas: 42 de 50 mapas
Faltan: 8 mapas
Puntos por mapas: 420
Suma de desafios: 180
Bonus: 78.5
Promedio (3 desafios y bonus): 64.625
Tiempo de juego: 2 h y 25 min
```