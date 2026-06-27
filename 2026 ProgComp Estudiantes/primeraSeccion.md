Orden de aprendizaje:
- **Bloque 1 (4–6):** imprimir por pantalla.
- **Bloque 2 (7–12):** leer por pantalla.
- **Bloque 3 (13–28):** una sola operación (suma, resta, multiplicación, división entera, residuo).
- **Bloque 4 (29–50):** varias lecturas, varias operaciones y varias impresiones.

## Bloque 1 — Impresión por pantalla
---
### Ejercicio 1

Diseña un programa en C++ que imprima por pantalla “¡Hola, mundo!”.

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "¡Hola, mundo!" << endl;
    return 0;
}
```
---
### Ejercicio 2

Diseña un programa en C++ que imprima por pantalla lo siguiente:

> 1
2
3
> 

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "1" << endl;
    cout << "2" << endl;
		cout << "3" << endl;
    return 0;
}
```
---
### Ejercicio 3

Diseña un programa en C++ que lea tu nombre y salude, con esta estructura de ejemplo: “¡Hola, María!

```cpp
#include <iostream>
using namespace std;

int main() {
    char nombre[30]; 
    cin >> nombre;
    cout << "¡Hola, " << nombre << "!" << endl;
    
    return 0;
}
```

```cpp
#include <iostream>
#include <string> 
using namespace std;

int main() {
    string nombre; 
    cin >> nombre;
    cout << "¡Hola, " << nombre << "!" << endl;
    
    return 0;
}
```

### Ejercicio 4
Imprime los números 1, 2 y 3 en una sola línea, separados por un espacio.

**Entrada:** (no hay)

**Salida:**
```
1 2 3
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    cout << 1 << " " << 2 << " " << 3 << endl;
    return 0;
}
```

---

### Ejercicio 5
Imprime exactamente el siguiente dibujo, formado por tres líneas:
```
*
**
***
```

**Entrada:** (no hay)

**Salida:**
```
*
**
***
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "*" << endl;
    cout << "**" << endl;
    cout << "***" << endl;
    return 0;
}
```

---

### Ejercicio 6
Imprime una tarjeta de presentación con exactamente estas tres líneas:
```
Nombre: Ana
Edad: 14
Ciudad: Valparaíso
```

**Entrada:** (no hay)

**Salida:**
```
Nombre: Ana
Edad: 14
Ciudad: Valparaíso
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Nombre: Ana" << endl;
    cout << "Edad: 14" << endl;
    cout << "Ciudad: Valparaíso" << endl;
    return 0;
}
```

---

## Bloque 2 — Lectura por pantalla

### Ejercicio 7
Lee un número entero y vuelve a imprimirlo en pantalla.

**Entrada:**
```
7
```

**Salida:**
```
7
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    cout << n << endl;
    return 0;
}
```

---

### Ejercicio 8
Lee un número entero e imprímelo con el mensaje `El número ingresado es X`, donde `X` es el número leído.

**Entrada:**
```
25
```

**Salida:**
```
El número ingresado es 25
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    cout << "El número ingresado es " << n << endl;
    return 0;
}
```

---

### Ejercicio 9
Lee dos números enteros e imprímelos, cada uno en su propia línea.

**Entrada:**
```
8
3
```

**Salida:**
```
8
3
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    cout << a << endl;
    cout << b << endl;
    return 0;
}
```

---

### Ejercicio 10
Lee dos números enteros e imprímelos en orden inverso (primero el segundo que ingresaste, luego el primero), en una sola línea separados por un espacio.

**Entrada:**
```
8
3
```

**Salida:**
```
3 8
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    cout << b << " " << a << endl;
    return 0;
}
```

---

### Ejercicio 11
Lee un número decimal y vuelve a imprimirlo.

**Entrada:**
```
3.5
```

**Salida:**
```
3.5
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    double x;
    cin >> x;
    cout << x << endl;
    return 0;
}
```

---

### Ejercicio 12
Lee tu nombre y tu apellido (dos palabras separadas) e imprime `Hola, Nombre Apellido`.

**Entrada:**
```
Ana
Soto
```

**Salida:**
```
Hola, Ana Soto
```

**Solución:**
```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string nombre, apellido;
    cin >> nombre >> apellido;
    cout << "Hola, " << nombre << " " << apellido << endl;
    return 0;
}
```

---

## Bloque 3 — Operaciones aritméticas

### Ejercicio 13
Lee dos números enteros e imprime su suma.

**Entrada:**
```
4
5
```

**Salida:**
```
9
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    cout << a + b << endl;
    return 0;
}
```

---

### Ejercicio 14
Lee dos números enteros e imprime su resta: el primero menos el segundo.

**Entrada:**
```
10
3
```

**Salida:**
```
7
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    cout << a - b << endl;
    return 0;
}
```

---

### Ejercicio 15
Lee dos números enteros e imprime su multiplicación.

**Entrada:**
```
6
7
```

**Salida:**
```
42
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    cout << a * b << endl;
    return 0;
}
```

---

### Ejercicio 16
Lee dos números enteros e imprime el resultado de la división entera: el primero dividido por el segundo. Recuerda que al dividir dos enteros, C++ descarta los decimales; por ejemplo, `7 / 2` da `3`.

**Entrada:**
```
7
2
```

**Salida:**
```
3
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    cout << a / b << endl;
    return 0;
}
```

---

### Ejercicio 17
Lee dos números enteros e imprime el residuo (lo que sobra) de dividir el primero por el segundo. Por ejemplo, el residuo de `7` entre `2` es `1`. En C++ el residuo se obtiene con el símbolo `%`.

**Entrada:**
```
7
2
```

**Salida:**
```
1
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    cout << a % b << endl;
    return 0;
}
```

---

### Ejercicio 18
Lee un número entero e imprime su doble (el número multiplicado por 2).

**Entrada:**
```
8
```

**Salida:**
```
16
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    cout << n * 2 << endl;
    return 0;
}
```

---

### Ejercicio 19
Lee un número entero e imprime su cuadrado (el número multiplicado por sí mismo).

**Entrada:**
```
5
```

**Salida:**
```
25
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    cout << n * n << endl;
    return 0;
}
```

---

### Ejercicio 20
Lee un número entero e imprime el número que viene justo después (el número más 1).

**Entrada:**
```
9
```

**Salida:**
```
10
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    cout << n + 1 << endl;
    return 0;
}
```

---

### Ejercicio 21
Lee un número entero e imprime el número que viene justo antes (el número menos 1).

**Entrada:**
```
9
```

**Salida:**
```
8
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    cout << n - 1 << endl;
    return 0;
}
```

---

### Ejercicio 22
Lee tres números enteros e imprime su suma.

**Entrada:**
```
2
3
4
```

**Salida:**
```
9
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b, c;
    cin >> a >> b >> c;
    cout << a + b + c << endl;
    return 0;
}
```

---

### Ejercicio 23
Lee dos números decimales e imprime su suma.

**Entrada:**
```
1.5
2.25
```

**Salida:**
```
3.75
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    double a, b;
    cin >> a >> b;
    cout << a + b << endl;
    return 0;
}
```

---

### Ejercicio 24
Lee un número decimal e imprime su mitad (el número dividido por 2).

**Entrada:**
```
5
```

**Salida:**
```
2.5
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    double x;
    cin >> x;
    cout << x / 2 << endl;
    return 0;
}
```

---

### Ejercicio 25
Lee dos números enteros e imprime, en este orden y separados por un espacio, su suma y su resta (primero menos segundo).

**Entrada:**
```
10
4
```

**Salida:**
```
14 6
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    cout << a + b << " " << a - b << endl;
    return 0;
}
```

---

### Ejercicio 26
Lee dos números enteros e imprime, en líneas separadas y en este orden, su suma, su resta (primero menos segundo) y su multiplicación.

**Entrada:**
```
6
2
```

**Salida:**
```
8
4
12
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    cout << a + b << endl;
    cout << a - b << endl;
    cout << a * b << endl;
    return 0;
}
```

---

### Ejercicio 27
Lee dos números enteros e imprime el resultado de sumarlos y luego multiplicar esa suma por 2; es decir, `(a + b) * 2`.

**Entrada:**
```
3
4
```

**Salida:**
```
14
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    cout << (a + b) * 2 << endl;
    return 0;
}
```

---

### Ejercicio 28
Lee tres números enteros e imprime su multiplicación.

**Entrada:**
```
2
3
4
```

**Salida:**
```
24
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b, c;
    cin >> a >> b >> c;
    cout << a * b * c << endl;
    return 0;
}
```

---

## Bloque 4 — Múltiples operaciones, lecturas e impresiones

### Ejercicio 29
Lee el largo y el ancho de un rectángulo (dos números enteros) e imprime su área (largo × ancho).

**Entrada:**
```
5
3
```

**Salida:**
```
15
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int largo, ancho;
    cin >> largo >> ancho;
    cout << largo * ancho << endl;
    return 0;
}
```

---

### Ejercicio 30
Lee el largo y el ancho de un rectángulo (dos números enteros) e imprime su perímetro. El perímetro se calcula como `2 * (largo + ancho)`.

**Entrada:**
```
5
3
```

**Salida:**
```
16
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int largo, ancho;
    cin >> largo >> ancho;
    cout << 2 * (largo + ancho) << endl;
    return 0;
}
```

---

### Ejercicio 31
Lee el largo y el ancho de un rectángulo (dos números enteros) e imprime, en líneas separadas, primero su área y luego su perímetro.

**Entrada:**
```
5
3
```

**Salida:**
```
15
16
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int largo, ancho;
    cin >> largo >> ancho;
    int area = largo * ancho;
    int perimetro = 2 * (largo + ancho);
    cout << area << endl;
    cout << perimetro << endl;
    return 0;
}
```

---

### Ejercicio 32
Lee el lado de un cuadrado (un número entero) e imprime su área (lado × lado).

**Entrada:**
```
4
```

**Salida:**
```
16
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int lado;
    cin >> lado;
    cout << lado * lado << endl;
    return 0;
}
```

---

### Ejercicio 33
Lee el lado de un cuadrado (un número entero) e imprime, en líneas separadas, su área (lado × lado) y su perímetro (4 × lado).

**Entrada:**
```
5
```

**Salida:**
```
25
20
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int lado;
    cin >> lado;
    cout << lado * lado << endl;
    cout << 4 * lado << endl;
    return 0;
}
```

---

### Ejercicio 34
Lee la base y la altura de un triángulo (dos números enteros) e imprime su área. El área de un triángulo es `(base * altura) / 2`. Para este ejercicio, la entrada siempre dará un resultado exacto (sin decimales).

**Entrada:**
```
6
4
```

**Salida:**
```
12
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int base, altura;
    cin >> base >> altura;
    cout << (base * altura) / 2 << endl;
    return 0;
}
```

---

### Ejercicio 35
Lee el precio de un producto y la cantidad de unidades compradas (dos números enteros). Imprime el total a pagar (precio × cantidad).

**Entrada:**
```
500
3
```

**Salida:**
```
1500
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int precio, cantidad;
    cin >> precio >> cantidad;
    cout << precio * cantidad << endl;
    return 0;
}
```

---

### Ejercicio 36
Una persona paga una compra con dinero en efectivo. Lee el total de la compra y con cuánto dinero paga (dos números enteros; el pago siempre es mayor o igual al total). Imprime el vuelto (lo que paga menos el total).

**Entrada:**
```
1500
2000
```

**Salida:**
```
500
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int total, pago;
    cin >> total >> pago;
    cout << pago - total << endl;
    return 0;
}
```

---

### Ejercicio 37
Lee tres números enteros que representan las tres notas de un estudiante. Imprime la suma de las tres notas.

**Entrada:**
```
60
70
80
```

**Salida:**
```
210
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n1, n2, n3;
    cin >> n1 >> n2 >> n3;
    cout << n1 + n2 + n3 << endl;
    return 0;
}
```

---

### Ejercicio 38
Lee tres números enteros (las tres notas de un estudiante) e imprime su promedio. Para este ejercicio, las tres notas siempre sumarán un total divisible por 3, así que usa la división entera.

**Entrada:**
```
60
70
80
```

**Salida:**
```
70
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n1, n2, n3;
    cin >> n1 >> n2 >> n3;
    cout << (n1 + n2 + n3) / 3 << endl;
    return 0;
}
```

---

### Ejercicio 39
Lee dos números enteros e imprime su promedio como número decimal. Usa la fórmula `(a + b) / 2.0`. Escribir `2.0` (en lugar de `2`) hace que el resultado conserve los decimales.

**Entrada:**
```
5
2
```

**Salida:**
```
3.5
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    cout << (a + b) / 2.0 << endl;
    return 0;
}
```

---

### Ejercicio 40
Lee una cantidad de minutos (un número entero) e imprime a cuántos segundos equivale (minutos × 60).

**Entrada:**
```
3
```

**Salida:**
```
180
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int minutos;
    cin >> minutos;
    cout << minutos * 60 << endl;
    return 0;
}
```

---

### Ejercicio 41
Lee una cantidad de segundos (un número entero) e imprime, en líneas separadas, cuántos minutos completos hay y cuántos segundos sobran. Usa la división entera para los minutos y el residuo para los segundos sobrantes.

**Entrada:**
```
130
```

**Salida:**
```
2
10
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int s;
    cin >> s;
    cout << s / 60 << endl;
    cout << s % 60 << endl;
    return 0;
}
```

---

### Ejercicio 42
Lee una temperatura en grados Celsius (puede tener decimales) e imprime su equivalente en grados Fahrenheit. La fórmula es `F = C * 9 / 5 + 32`. Para que no se pierdan los decimales, escribe el `9` como `9.0` en tu fórmula.

**Entrada:**
```
37
```

**Salida:**
```
98.6
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    double c;
    cin >> c;
    cout << c * 9.0 / 5 + 32 << endl;
    return 0;
}
```

---

### Ejercicio 43
Lee la velocidad de un auto en kilómetros por hora y la cantidad de horas que viaja (dos números enteros). Imprime la distancia recorrida (velocidad × horas).

**Entrada:**
```
80
3
```

**Salida:**
```
240
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int velocidad, horas;
    cin >> velocidad >> horas;
    cout << velocidad * horas << endl;
    return 0;
}
```

---

### Ejercicio 44
Lee cuatro números enteros e imprime su multiplicación.

**Entrada:**
```
3
5
9
7
```

**Salida:**
```
945
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b, c, d;
    cin >> a >> b >> c >> d;
    cout << a * b * c * d << endl;
    return 0;
}
```

---

### Ejercicio 45
Lee dos números enteros, `a` y `b`. Imprime, en líneas separadas y en este orden: su suma, su resta (`a - b`), su multiplicación y su división entera (`a / b`).

**Entrada:**
```
12
4
```

**Salida:**
```
16
8
48
3
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    cout << a + b << endl;
    cout << a - b << endl;
    cout << a * b << endl;
    cout << a / b << endl;
    return 0;
}
```

---

### Ejercicio 46
Lee el radio de un círculo (un número entero) e imprime su área aproximada. Usa `3.14` como valor de pi. La fórmula es `área = 3.14 * radio * radio`.

**Entrada:**
```
2
```

**Salida:**
```
12.56
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int radio;
    cin >> radio;
    cout << 3.14 * radio * radio << endl;
    return 0;
}
```

---

### Ejercicio 47
Lee el ancho, el largo y la altura de una caja (tres números enteros) e imprime su volumen (ancho × largo × altura).

**Entrada:**
```
2
3
4
```

**Salida:**
```
24
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int ancho, largo, altura;
    cin >> ancho >> largo >> altura;
    cout << ancho * largo * altura << endl;
    return 0;
}
```

---

### Ejercicio 48
Lee dos números enteros: una cantidad de horas y una cantidad de minutos. Imprime a cuántos minutos equivale todo en total. La fórmula es `horas * 60 + minutos`.

**Entrada:**
```
2
30
```

**Salida:**
```
150
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int horas, minutos;
    cin >> horas >> minutos;
    cout << horas * 60 + minutos << endl;
    return 0;
}
```

---

### Ejercicio 49
Lee la cantidad de productos comprados y el precio de cada uno (dos números enteros). Luego lee cuánto dinero entrega el cliente (otro número entero; siempre es suficiente). Imprime, en líneas separadas: el total de la compra (cantidad × precio) y el vuelto (lo entregado menos el total).

**Entrada:**
```
3
500
2000
```

**Salida:**
```
1500
500
```

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int cantidad, precio, entregado;
    cin >> cantidad >> precio >> entregado;
    int total = cantidad * precio;
    cout << total << endl;
    cout << entregado - total << endl;
    return 0;
}
```

---

### Ejercicio 50
Lee el nombre de un estudiante (una palabra) y luego sus tres notas (tres números enteros). Imprime tres líneas: la primera con `Estudiante: Nombre`, la segunda con `Total: ` seguido de la suma de las tres notas, y la tercera con `Promedio: ` seguido del promedio. Para este ejercicio, las tres notas siempre sumarán un total divisible por 3 (usa la división entera para el promedio).

**Entrada:**
```
Ana
60
70
80
```

**Salida:**
```
Estudiante: Ana
Total: 210
Promedio: 70
```

**Solución:**
```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string nombre;
    int n1, n2, n3;
    cin >> nombre >> n1 >> n2 >> n3;
    int total = n1 + n2 + n3;
    cout << "Estudiante: " << nombre << endl;
    cout << "Total: " << total << endl;
    cout << "Promedio: " << total / 3 << endl;
    return 0;
}
```

---

# Ejercicio Final (Difícil)

---

### Enunciado

Escribe un programa que arme el reporte de fin de curso de un estudiante en un curso de programación. Las notas y el proyecto se miden en una escala de **puntos de 0 a 100**.

El programa lee, **en este orden exacto**, los siguientes datos:

1. `nombre` — el nombre del estudiante (una palabra).
2. `resueltos` — cuántos ejercicios resolvió (entero).
3. `totales` — cuántos ejercicios tiene el curso en total (entero; siempre mayor o igual que `resueltos`).
4. `n1`, `n2`, `n3` — los puntajes de las tres pruebas (tres enteros).
5. `proyecto` — el puntaje del proyecto, que puede tener decimales (número decimal).
6. `minutos` — el total de minutos que estudió (entero).

Luego imprime **exactamente** estas ocho líneas, en este orden:

1. `Estudiante: ` seguido del nombre.
2. `Avance: ` seguido de los ejercicios resueltos, ` de `, el total, y ` ejercicios`.
3. `Te faltan: ` seguido de los ejercicios que faltan (`totales - resueltos`) y ` ejercicios`.
4. `Puntos por ejercicios: ` seguido de los ejercicios resueltos multiplicados por 10.
5. `Suma de las tres pruebas: ` seguido de la suma de los tres puntajes.
6. `Nota del proyecto: ` seguido del puntaje del proyecto.
7. `Promedio general (tres pruebas y proyecto): ` seguido del promedio de los cuatro puntajes (las tres pruebas más el proyecto, dividido por `4.0`). Como uno de los valores tiene decimales y divides por `4.0`, el resultado debe conservar los decimales.
8. `Tiempo de estudio: ` seguido de cuántas horas completas estudió (`minutos / 60`), ` h y `, cuántos minutos sobran (`minutos % 60`), y ` min`.

---

### Ejemplo

**Entrada:**
```
Camila
42
50
60
70
50
78.5
145
```

**Salida:**
```
Estudiante: Camila
Avance: 42 de 50 ejercicios
Te faltan: 8 ejercicios
Puntos por ejercicios: 420
Suma de las tres pruebas: 180
Nota del proyecto: 78.5
Promedio general (tres pruebas y proyecto): 64.625
Tiempo de estudio: 2 h y 25 min
```

---

### Solución

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string nombre;
    int resueltos, totales;
    int n1, n2, n3;
    double proyecto;
    int minutos;

    cin >> nombre >> resueltos >> totales >> n1 >> n2 >> n3 >> proyecto >> minutos;

    int suma = n1 + n2 + n3;

    cout << "Estudiante: " << nombre << endl;
    cout << "Avance: " << resueltos << " de " << totales << " ejercicios" << endl;
    cout << "Te faltan: " << totales - resueltos << " ejercicios" << endl;
    cout << "Puntos por ejercicios: " << resueltos * 10 << endl;
    cout << "Suma de las tres pruebas: " << suma << endl;
    cout << "Nota del proyecto: " << proyecto << endl;
    cout << "Promedio general (tres pruebas y proyecto): " << (suma + proyecto) / 4.0 << endl;
    cout << "Tiempo de estudio: " << minutos / 60 << " h y " << minutos % 60 << " min" << endl;
    return 0;
}
```

---
