# Sección 2 — Condicionales (`if` / `else if` / `else`)

**Operadores de comparación** (devuelven verdadero o falso):

| Símbolo | Significado |
|---|---|
| `>` | mayor que |
| `<` | menor que |
| `>=` | mayor o igual que |
| `<=` | menor o igual que |
| `==` | igual a (¡son **dos** signos!) |
| `!=` | distinto de |

---

## Bloque 1 — `if` y `if`–`else` básico

### Ejercicio 1
Lee un número entero. Si el número es mayor que 100, imprime `Mayor a 100`. Si no lo es, no imprimas nada.

Entrada: `150` → Salida: `Mayor a 100`
Entrada: `50` → Salida: *(no imprime nada)*

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n > 100) {
        cout << "Mayor a 100" << endl;
    }
    return 0;
}
```

---

### Ejercicio 2
Lee un número entero. Si es positivo (mayor que 0), imprime `Positivo`; en caso contrario, imprime `No positivo`.

Entrada: `5` → Salida: `Positivo`
Entrada: `-3` → Salida: `No positivo`
Entrada: `0` → Salida: `No positivo`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n > 0) {
        cout << "Positivo" << endl;
    } else {
        cout << "No positivo" << endl;
    }
    return 0;
}
```

---

### Ejercicio 3
Lee la edad de una persona (un número entero). Si tiene 18 años o más, imprime `Mayor de edad`; si no, imprime `Menor de edad`.

Entrada: `20` → Salida: `Mayor de edad`
Entrada: `18` → Salida: `Mayor de edad`
Entrada: `15` → Salida: `Menor de edad`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int edad;
    cin >> edad;
    if (edad >= 18) {
        cout << "Mayor de edad" << endl;
    } else {
        cout << "Menor de edad" << endl;
    }
    return 0;
}
```

---

### Ejercicio 4
Lee una temperatura (un número entero). Si es menor que 0, imprime `Bajo cero`; en caso contrario, imprime `Cero o sobre cero`.

Entrada: `-5` → Salida: `Bajo cero`
Entrada: `0` → Salida: `Cero o sobre cero`
Entrada: `8` → Salida: `Cero o sobre cero`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int t;
    cin >> t;
    if (t < 0) {
        cout << "Bajo cero" << endl;
    } else {
        cout << "Cero o sobre cero" << endl;
    }
    return 0;
}
```

---

### Ejercicio 5
Lee un número entero. Si es igual a 0, imprime `Es cero`; si no, imprime `No es cero`.

Entrada: `0` → Salida: `Es cero`
Entrada: `7` → Salida: `No es cero`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n == 0) {
        cout << "Es cero" << endl;
    } else {
        cout << "No es cero" << endl;
    }
    return 0;
}
```

---

### Ejercicio 6
Lee dos números enteros. Si son distintos, imprime `Distintos`; si no, imprime `Iguales`.

Entrada: `5 7` → Salida: `Distintos`
Entrada: `4 4` → Salida: `Iguales`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    if (a != b) {
        cout << "Distintos" << endl;
    } else {
        cout << "Iguales" << endl;
    }
    return 0;
}
```

---

### Ejercicio 7
Lee un número entero. Si es par, imprime `Par`; si no, imprime `Impar`. (Un número es par cuando el residuo de dividirlo por 2 es 0.)

Entrada: `4` → Salida: `Par`
Entrada: `7` → Salida: `Impar`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n % 2 == 0) {
        cout << "Par" << endl;
    } else {
        cout << "Impar" << endl;
    }
    return 0;
}
```

---

### Ejercicio 8
Lee dos números enteros e imprime el **mayor** de los dos. Si son iguales, imprime ese mismo número.

Entrada: `8 3` → Salida: `8`
Entrada: `2 9` → Salida: `9`
Entrada: `5 5` → Salida: `5`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    if (a > b) {
        cout << a << endl;
    } else {
        cout << b << endl;
    }
    return 0;
}
```

---

### Ejercicio 9
Lee dos números enteros e imprime el **menor** de los dos. Si son iguales, imprime ese mismo número.

Entrada: `8 3` → Salida: `3`
Entrada: `2 9` → Salida: `2`
Entrada: `5 5` → Salida: `5`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    if (a < b) {
        cout << a << endl;
    } else {
        cout << b << endl;
    }
    return 0;
}
```

---

### Ejercicio 10
Lee un número entero. Si es negativo, imprímelo sin el signo (su valor absoluto); si no, imprímelo tal cual.

Entrada: `-7` → Salida: `7`
Entrada: `4` → Salida: `4`
Entrada: `0` → Salida: `0`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n < 0) {
        cout << -n << endl;
    } else {
        cout << n << endl;
    }
    return 0;
}
```

---

## Bloque 2 — `if` / `else if` / `else`

### Ejercicio 11
Lee un número entero. Si es positivo (mayor que 0), imprime `Positivo`; si es negativo (menor que 0), imprime `Negativo`; si no, imprime `Cero`.

Entrada: `5` → Salida: `Positivo`
Entrada: `-3` → Salida: `Negativo`
Entrada: `0` → Salida: `Cero`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n > 0) {
        cout << "Positivo" << endl;
    } else if (n < 0) {
        cout << "Negativo" << endl;
    } else {
        cout << "Cero" << endl;
    }
    return 0;
}
```

---

### Ejercicio 12
Lee dos números enteros. Si el primero es mayor que el segundo, imprime `El primero es mayor`; si el primero es menor, imprime `El segundo es mayor`; si son iguales, imprime `Son iguales`.

Entrada: `5 3` → Salida: `El primero es mayor`
Entrada: `3 5` → Salida: `El segundo es mayor`
Entrada: `4 4` → Salida: `Son iguales`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    if (a > b) {
        cout << "El primero es mayor" << endl;
    } else if (a < b) {
        cout << "El segundo es mayor" << endl;
    } else {
        cout << "Son iguales" << endl;
    }
    return 0;
}
```

---

### Ejercicio 13
Lee la edad de una persona (un número entero). Si es menor que 13, imprime `Niño`; si tiene entre 13 y 17 años, imprime `Adolescente`; si tiene 18 o más, imprime `Adulto`.

Entrada: `10` → Salida: `Niño`
Entrada: `15` → Salida: `Adolescente`
Entrada: `30` → Salida: `Adulto`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int edad;
    cin >> edad;
    if (edad < 13) {
        cout << "Niño" << endl;
    } else if (edad < 18) {
        cout << "Adolescente" << endl;
    } else {
        cout << "Adulto" << endl;
    }
    return 0;
}
```

---

### Ejercicio 14
Lee el puntaje de una prueba (un número entero de 0 a 100) y conviértelo a una letra según esta tabla: 90 o más → `A`; entre 80 y 89 → `B`; entre 70 y 79 → `C`; entre 60 y 69 → `D`; menos de 60 → `F`. Imprime la letra.

Entrada: `95` → Salida: `A`
Entrada: `85` → Salida: `B`
Entrada: `72` → Salida: `C`
Entrada: `61` → Salida: `D`
Entrada: `40` → Salida: `F`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int p;
    cin >> p;
    if (p >= 90) {
        cout << "A" << endl;
    } else if (p >= 80) {
        cout << "B" << endl;
    } else if (p >= 70) {
        cout << "C" << endl;
    } else if (p >= 60) {
        cout << "D" << endl;
    } else {
        cout << "F" << endl;
    }
    return 0;
}
```

> Nota docente: el orden de las condiciones importa. Como cada `else if` solo se evalúa si las anteriores fueron falsas, basta con comparar el límite inferior de cada rango de mayor a menor.

---

### Ejercicio 15
Lee un número entero positivo. Si es menor que 10, imprime `Pequeño`; si está entre 10 y 99, imprime `Mediano`; si es 100 o más, imprime `Grande`.

Entrada: `5` → Salida: `Pequeño`
Entrada: `50` → Salida: `Mediano`
Entrada: `500` → Salida: `Grande`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n < 10) {
        cout << "Pequeño" << endl;
    } else if (n < 100) {
        cout << "Mediano" << endl;
    } else {
        cout << "Grande" << endl;
    }
    return 0;
}
```

---

### Ejercicio 16
Lee la temperatura del agua en grados Celsius (un número entero) e imprime su estado: si es 0 o menos, `Sólido (hielo)`; si está entre 1 y 99, `Líquido (agua)`; si es 100 o más, `Gaseoso (vapor)`.

Entrada: `-5` → Salida: `Sólido (hielo)`
Entrada: `50` → Salida: `Líquido (agua)`
Entrada: `150` → Salida: `Gaseoso (vapor)`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int t;
    cin >> t;
    if (t <= 0) {
        cout << "Sólido (hielo)" << endl;
    } else if (t < 100) {
        cout << "Líquido (agua)" << endl;
    } else {
        cout << "Gaseoso (vapor)" << endl;
    }
    return 0;
}
```

---

### Ejercicio 17
Lee el número de un mes (un número entero del 1 al 12; siempre será un valor válido) e imprime el trimestre al que pertenece: meses 1 a 3 → `Primer trimestre`; 4 a 6 → `Segundo trimestre`; 7 a 9 → `Tercer trimestre`; 10 a 12 → `Cuarto trimestre`.

Entrada: `2` → Salida: `Primer trimestre`
Entrada: `5` → Salida: `Segundo trimestre`
Entrada: `8` → Salida: `Tercer trimestre`
Entrada: `11` → Salida: `Cuarto trimestre`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int mes;
    cin >> mes;
    if (mes <= 3) {
        cout << "Primer trimestre" << endl;
    } else if (mes <= 6) {
        cout << "Segundo trimestre" << endl;
    } else if (mes <= 9) {
        cout << "Tercer trimestre" << endl;
    } else {
        cout << "Cuarto trimestre" << endl;
    }
    return 0;
}
```

---

### Ejercicio 18
Lee el número de un día de la semana (un número entero del 1 al 7; siempre será un valor válido) e imprime su nombre: 1 → `Lunes`, 2 → `Martes`, 3 → `Miércoles`, 4 → `Jueves`, 5 → `Viernes`, 6 → `Sábado`, 7 → `Domingo`.

Entrada: `1` → Salida: `Lunes`
Entrada: `4` → Salida: `Jueves`
Entrada: `7` → Salida: `Domingo`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int dia;
    cin >> dia;
    if (dia == 1) {
        cout << "Lunes" << endl;
    } else if (dia == 2) {
        cout << "Martes" << endl;
    } else if (dia == 3) {
        cout << "Miércoles" << endl;
    } else if (dia == 4) {
        cout << "Jueves" << endl;
    } else if (dia == 5) {
        cout << "Viernes" << endl;
    } else if (dia == 6) {
        cout << "Sábado" << endl;
    } else {
        cout << "Domingo" << endl;
    }
    return 0;
}
```

---

### Ejercicio 19
Lee el monto de una compra en pesos (un número entero) e imprime el descuento que le corresponde: 100000 o más → `30% de descuento`; entre 50000 y 99999 → `15% de descuento`; entre 20000 y 49999 → `5% de descuento`; menos de 20000 → `Sin descuento`.

Entrada: `120000` → Salida: `30% de descuento`
Entrada: `60000` → Salida: `15% de descuento`
Entrada: `30000` → Salida: `5% de descuento`
Entrada: `10000` → Salida: `Sin descuento`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int monto;
    cin >> monto;
    if (monto >= 100000) {
        cout << "30% de descuento" << endl;
    } else if (monto >= 50000) {
        cout << "15% de descuento" << endl;
    } else if (monto >= 20000) {
        cout << "5% de descuento" << endl;
    } else {
        cout << "Sin descuento" << endl;
    }
    return 0;
}
```

---

### Ejercicio 20
Lee dos números enteros y, a continuación, un código de operación (un número entero). Según el código, imprime el resultado de la operación entre los dos números: `1` → suma, `2` → resta (primero menos segundo), `3` → multiplicación, `4` → división entera (primero dividido por el segundo). Si el código no es ninguno de esos, imprime `Operación inválida`. Para la división, el segundo número nunca será 0.

Entrada: `6 2 1` → Salida: `8`
Entrada: `6 2 2` → Salida: `4`
Entrada: `6 2 3` → Salida: `12`
Entrada: `6 2 4` → Salida: `3`
Entrada: `6 2 9` → Salida: `Operación inválida`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b, op;
    cin >> a >> b >> op;
    if (op == 1) {
        cout << a + b << endl;
    } else if (op == 2) {
        cout << a - b << endl;
    } else if (op == 3) {
        cout << a * b << endl;
    } else if (op == 4) {
        cout << a / b << endl;
    } else {
        cout << "Operación inválida" << endl;
    }
    return 0;
}
```

---

## Bloque 3 — `if` anidados

Un `if` anidado es un `if` que está **dentro** de otro. Sirve para tomar una decisión solo después de que otra ya se cumplió: primero se revisa la condición de afuera y, dependiendo del resultado, recién se revisa la de adentro.

### Ejercicio 21
Lee dos números enteros. Imprime `Ambos positivos` **únicamente** si el primero es positivo (mayor que 0) y el segundo también lo es. En cualquier otro caso, no imprimas nada.

Entrada: `5 3` → Salida: `Ambos positivos`
Entrada: `5 -1` → Salida: *(no imprime nada)*
Entrada: `-2 4` → Salida: *(no imprime nada)*

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    if (a > 0) {
        if (b > 0) {
            cout << "Ambos positivos" << endl;
        }
    }
    return 0;
}
```

---

### Ejercicio 22
Lee dos números enteros. Si el primero es positivo: cuando el segundo también sea positivo imprime `Ambos positivos`, y si no, imprime `Solo el primero es positivo`. Si el primero **no** es positivo, imprime `El primero no es positivo`.

Entrada: `5 3` → Salida: `Ambos positivos`
Entrada: `5 -1` → Salida: `Solo el primero es positivo`
Entrada: `-2 4` → Salida: `El primero no es positivo`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    if (a > 0) {
        if (b > 0) {
            cout << "Ambos positivos" << endl;
        } else {
            cout << "Solo el primero es positivo" << endl;
        }
    } else {
        cout << "El primero no es positivo" << endl;
    }
    return 0;
}
```

---

### Ejercicio 23
Lee la edad de una persona y luego un número que indica si tiene licencia de conducir (`1` si tiene, `0` si no tiene). Si la edad es 18 o más: cuando tenga licencia imprime `Puede conducir`, y si no la tiene imprime `Necesita licencia`. Si la edad es menor que 18, imprime `Muy joven para conducir`.

Entrada: `20 1` → Salida: `Puede conducir`
Entrada: `20 0` → Salida: `Necesita licencia`
Entrada: `15 1` → Salida: `Muy joven para conducir`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int edad, licencia;
    cin >> edad >> licencia;
    if (edad >= 18) {
        if (licencia == 1) {
            cout << "Puede conducir" << endl;
        } else {
            cout << "Necesita licencia" << endl;
        }
    } else {
        cout << "Muy joven para conducir" << endl;
    }
    return 0;
}
```

---

### Ejercicio 24
Lee un número entero. Imprime `En el rango` si el número está entre 10 y 20 (incluyendo el 10 y el 20). En cualquier otro caso imprime `Fuera del rango`. Resuélvelo anidando dos `if`: primero revisa si es 10 o más y, dentro, si es 20 o menos.

Entrada: `15` → Salida: `En el rango`
Entrada: `25` → Salida: `Fuera del rango`
Entrada: `5` → Salida: `Fuera del rango`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n >= 10) {
        if (n <= 20) {
            cout << "En el rango" << endl;
        } else {
            cout << "Fuera del rango" << endl;
        }
    } else {
        cout << "Fuera del rango" << endl;
    }
    return 0;
}
```

---

### Ejercicio 25
Lee dos números enteros, `x` e `y`, que representan un punto en el plano (ninguno de los dos será 0). Imprime en qué cuadrante está: si `x` es positivo e `y` es positivo → `Cuadrante I`; si `x` es negativo e `y` es positivo → `Cuadrante II`; si `x` es negativo e `y` es negativo → `Cuadrante III`; si `x` es positivo e `y` es negativo → `Cuadrante IV`.

Entrada: `3 5` → Salida: `Cuadrante I`
Entrada: `-3 5` → Salida: `Cuadrante II`
Entrada: `-3 -5` → Salida: `Cuadrante III`
Entrada: `3 -5` → Salida: `Cuadrante IV`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int x, y;
    cin >> x >> y;
    if (x > 0) {
        if (y > 0) {
            cout << "Cuadrante I" << endl;
        } else {
            cout << "Cuadrante IV" << endl;
        }
    } else {
        if (y > 0) {
            cout << "Cuadrante II" << endl;
        } else {
            cout << "Cuadrante III" << endl;
        }
    }
    return 0;
}
```

---

### Ejercicio 26
Lee tres números enteros e imprime el **mayor** de los tres. Si hay empate, imprime ese valor. Resuélvelo anidando `if` (sin usar funciones).

Entrada: `3 7 5` → Salida: `7`
Entrada: `9 2 4` → Salida: `9`
Entrada: `1 1 8` → Salida: `8`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b, c;
    cin >> a >> b >> c;
    if (a >= b) {
        if (a >= c) {
            cout << a << endl;
        } else {
            cout << c << endl;
        }
    } else {
        if (b >= c) {
            cout << b << endl;
        } else {
            cout << c << endl;
        }
    }
    return 0;
}
```

---

### Ejercicio 27
Lee un número entero y clasifícalo así: si es positivo, cuando sea mayor que 100 imprime `Positivo grande`, y si no `Positivo pequeño`. Si es negativo, cuando sea menor que -100 imprime `Negativo grande`, y si no `Negativo pequeño`. Si es 0, imprime `Cero`.

Entrada: `150` → Salida: `Positivo grande`
Entrada: `50` → Salida: `Positivo pequeño`
Entrada: `-150` → Salida: `Negativo grande`
Entrada: `-50` → Salida: `Negativo pequeño`
Entrada: `0` → Salida: `Cero`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n > 0) {
        if (n > 100) {
            cout << "Positivo grande" << endl;
        } else {
            cout << "Positivo pequeño" << endl;
        }
    } else {
        if (n < 0) {
            if (n < -100) {
                cout << "Negativo grande" << endl;
            } else {
                cout << "Negativo pequeño" << endl;
            }
        } else {
            cout << "Cero" << endl;
        }
    }
    return 0;
}
```

---

### Ejercicio 28
Lee un año (un número entero) e indica si es bisiesto. Un año es bisiesto si es divisible por 4, **salvo** que sea divisible por 100, en cuyo caso solo es bisiesto si además es divisible por 400. Imprime `Bisiesto` o `No bisiesto`.

Entrada: `2000` → Salida: `Bisiesto`
Entrada: `1900` → Salida: `No bisiesto`
Entrada: `2024` → Salida: `Bisiesto`
Entrada: `2023` → Salida: `No bisiesto`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int anio;
    cin >> anio;
    if (anio % 4 == 0) {
        if (anio % 100 == 0) {
            if (anio % 400 == 0) {
                cout << "Bisiesto" << endl;
            } else {
                cout << "No bisiesto" << endl;
            }
        } else {
            cout << "Bisiesto" << endl;
        }
    } else {
        cout << "No bisiesto" << endl;
    }
    return 0;
}
```

---

### Ejercicio 29
Una entrada de cine cuesta según la edad y si la persona es estudiante. Lee la edad y luego un número que indica si es estudiante (`1` si lo es, `0` si no). El precio es: si la edad es menor que 12, `3000` (sin importar lo demás). En caso contrario: si es estudiante, `4000`; si no es estudiante, `6000`. Imprime el precio.

Entrada: `8 0` → Salida: `3000`
Entrada: `20 1` → Salida: `4000`
Entrada: `20 0` → Salida: `6000`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int edad, estudiante;
    cin >> edad >> estudiante;
    int precio;
    if (edad < 12) {
        precio = 3000;
    } else {
        if (estudiante == 1) {
            precio = 4000;
        } else {
            precio = 6000;
        }
    }
    cout << precio << endl;
    return 0;
}
```

---

### Ejercicio 30
Para aprobar un curso se necesita asistencia suficiente **y** una buena nota. Lee la nota (un número entero de 0 a 100) y luego la asistencia (un número entero de 0 a 100). Si la asistencia es menor que 50, imprime `Reprobado por asistencia` (sin importar la nota). En caso contrario: si la nota es 60 o más, imprime `Aprobado`; si no, imprime `Reprobado por nota`.

Entrada: `90 40` → Salida: `Reprobado por asistencia`
Entrada: `90 80` → Salida: `Aprobado`
Entrada: `40 80` → Salida: `Reprobado por nota`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int nota, asistencia;
    cin >> nota >> asistencia;
    if (asistencia < 50) {
        cout << "Reprobado por asistencia" << endl;
    } else {
        if (nota >= 60) {
            cout << "Aprobado" << endl;
        } else {
            cout << "Reprobado por nota" << endl;
        }
    }
    return 0;
}
```

---

## Bloque 4 — Final

### Ejercicio 31 
Escribe un programa que decida el resultado final de un estudiante combinando todo lo aprendido sobre condicionales.

El programa lee, **en este orden exacto**:
1. `nombre` — el nombre del estudiante (una palabra).
2. `n1`, `n2` — los puntajes de dos pruebas (dos enteros de 0 a 100).
3. `asistencia` — el porcentaje de asistencia (un entero de 0 a 100).

El programa calcula el promedio de las dos pruebas con decimales (`(n1 + n2) / 2.0`) y luego decide el resultado así:
- Si la asistencia es menor que 70, el resultado es `Reprobado por inasistencia` (sin importar el promedio).
- En caso contrario, según el promedio: si es 90 o más, `Aprobado con distinción`; si está entre 60 y 89, `Aprobado`; si es menor que 60, `Reprobado`.

Finalmente imprime **exactamente** estas tres líneas:
1. `Estudiante: ` seguido del nombre.
2. `Promedio: ` seguido del promedio calculado.
3. `Resultado: ` seguido del resultado.

**Ejemplo — Entrada:**
```
Diego
70
85
80
```

**Salida:**
```
Estudiante: Diego
Promedio: 77.5
Resultado: Aprobado
```

**Solución:**
```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string nombre;
    int n1, n2, asistencia;
    cin >> nombre >> n1 >> n2 >> asistencia;

    double promedio = (n1 + n2) / 2.0;

    string resultado;
    if (asistencia < 70) {
        resultado = "Reprobado por inasistencia";
    } else {
        if (promedio >= 90) {
            resultado = "Aprobado con distinción";
        } else if (promedio >= 60) {
            resultado = "Aprobado";
        } else {
            resultado = "Reprobado";
        }
    }

    cout << "Estudiante: " << nombre << endl;
    cout << "Promedio: " << promedio << endl;
    cout << "Resultado: " << resultado << endl;
    return 0;
}
```

# Operadores lógicos `&&`, `||` y `!`


| Operador | Nombre | Es verdadero cuando… |
|---|---|---|
| `&&` | Y (AND) | **ambas** condiciones son verdaderas |
| `\|\|` | O (OR) | **al menos una** condición es verdadera |
| `!` | NO (NOT) | invierte el resultado: es verdadero cuando la condición es **falsa** |


---

### Ejercicio 32
Lee dos números enteros. Si **ambos** son positivos (mayores que 0), imprime `Ambos positivos`; en caso contrario, imprime `No ambos`. Resuélvelo con `&&` en una sola condición.

Entrada: `5 3` → Salida: `Ambos positivos`
Entrada: `5 -1` → Salida: `No ambos`
Entrada: `-2 4` → Salida: `No ambos`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b;
    cin >> a >> b;
    if (a > 0 && b > 0) {
        cout << "Ambos positivos" << endl;
    } else {
        cout << "No ambos" << endl;
    }
    return 0;
}
```

---

### Ejercicio 33
Lee un número entero. Imprime `En el rango` si está entre 10 y 20 (incluyendo ambos extremos); si no, imprime `Fuera del rango`. Usa `&&` para revisar las dos cotas en una sola condición.

Entrada: `15` → Salida: `En el rango`
Entrada: `25` → Salida: `Fuera del rango`
Entrada: `5` → Salida: `Fuera del rango`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n >= 10 && n <= 20) {
        cout << "En el rango" << endl;
    } else {
        cout << "Fuera del rango" << endl;
    }
    return 0;
}
```

---

### Ejercicio 34
Lee el número de un día de la semana (un entero del 1 al 7, donde 6 es sábado y 7 es domingo). Si es sábado **o** domingo, imprime `Fin de semana`; si no, imprime `Día de semana`. Usa `||`.

Entrada: `6` → Salida: `Fin de semana`
Entrada: `7` → Salida: `Fin de semana`
Entrada: `3` → Salida: `Día de semana`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int dia;
    cin >> dia;
    if (dia == 6 || dia == 7) {
        cout << "Fin de semana" << endl;
    } else {
        cout << "Día de semana" << endl;
    }
    return 0;
}
```

---

### Ejercicio 35
Lee un número entero. Si es divisible por 3 **o** por 5, imprime `Divisible por 3 o por 5`; en caso contrario, imprime `No divisible`. Combina `||` con el operador `%`.

Entrada: `9` → Salida: `Divisible por 3 o por 5`
Entrada: `10` → Salida: `Divisible por 3 o por 5`
Entrada: `15` → Salida: `Divisible por 3 o por 5`
Entrada: `7` → Salida: `No divisible`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n % 3 == 0 || n % 5 == 0) {
        cout << "Divisible por 3 o por 5" << endl;
    } else {
        cout << "No divisible" << endl;
    }
    return 0;
}
```

---

### Ejercicio 36
Lee un número entero. Si es **par y además** mayor que 10, imprime `Par y mayor que 10`; en cualquier otro caso, imprime `No cumple`. Combina `&&` con el operador `%`. (Recuerda: un número es par cuando `n % 2 == 0`.)

Entrada: `12` → Salida: `Par y mayor que 10`
Entrada: `8` → Salida: `No cumple`
Entrada: `11` → Salida: `No cumple`
Entrada: `14` → Salida: `Par y mayor que 10`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n % 2 == 0 && n > 10) {
        cout << "Par y mayor que 10" << endl;
    } else {
        cout << "No cumple" << endl;
    }
    return 0;
}
```

---

### Ejercicio 37
Lee un número entero y aplica esta regla: si es divisible por 3 **y** por 5, imprime `FizzBuzz`; si solo es divisible por 3, imprime `Fizz`; si solo es divisible por 5, imprime `Buzz`; si no es divisible por ninguno, imprime el número tal cual.

Entrada: `15` → Salida: `FizzBuzz`
Entrada: `9` → Salida: `Fizz`
Entrada: `10` → Salida: `Buzz`
Entrada: `7` → Salida: `7`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (n % 3 == 0 && n % 5 == 0) {
        cout << "FizzBuzz" << endl;
    } else if (n % 3 == 0) {
        cout << "Fizz" << endl;
    } else if (n % 5 == 0) {
        cout << "Buzz" << endl;
    } else {
        cout << n << endl;
    }
    return 0;
}
```

---

### Ejercicio 38
Lee un año (un número entero) e indica si es bisiesto, **usando una sola condición** con `&&` y `||`. La regla es: un año es bisiesto si es divisible por 4 y **no** por 100, **o bien** si es divisible por 400. Imprime `Bisiesto` o `No bisiesto`.

Entrada: `2000` → Salida: `Bisiesto`
Entrada: `1900` → Salida: `No bisiesto`
Entrada: `2024` → Salida: `Bisiesto`
Entrada: `2023` → Salida: `No bisiesto`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int anio;
    cin >> anio;
    if ((anio % 4 == 0 && anio % 100 != 0) || anio % 400 == 0) {
        cout << "Bisiesto" << endl;
    } else {
        cout << "No bisiesto" << endl;
    }
    return 0;
}
```


---

### Ejercicio 39
Lee tres números enteros positivos que representan las longitudes de los lados de un posible triángulo. Tres lados forman un triángulo solo si cada lado es menor que la suma de los otros dos; es decir, deben cumplirse las tres condiciones a la vez. Imprime `Sí forma un triángulo` o `No forma un triángulo`.

Entrada: `3 4 5` → Salida: `Sí forma un triángulo`
Entrada: `1 2 10` → Salida: `No forma un triángulo`
Entrada: `5 5 5` → Salida: `Sí forma un triángulo`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int a, b, c;
    cin >> a >> b >> c;
    if (a + b > c && b + c > a && a + c > b) {
        cout << "Sí forma un triángulo" << endl;
    } else {
        cout << "No forma un triángulo" << endl;
    }
    return 0;
}
```


---

### Ejercicio 40
Para subir a un juego mecánico hay que medir al menos 140 cm **y** tener al menos 12 años. Pero quien venga acompañado de un adulto puede subir aunque no cumpla alguno de esos requisitos. Lee la estatura en centímetros, la edad y un número que indica si viene acompañado (`1` si viene acompañado, `0` si no). Imprime `Puede subir al juego` o `No puede subir al juego`.

Entrada: `150 14 0` → Salida: `Puede subir al juego`
Entrada: `130 10 0` → Salida: `No puede subir al juego`
Entrada: `130 10 1` → Salida: `Puede subir al juego`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int estatura, edad, acompanado;
    cin >> estatura >> edad >> acompanado;
    if ((estatura >= 140 && edad >= 12) || acompanado == 1) {
        cout << "Puede subir al juego" << endl;
    } else {
        cout << "No puede subir al juego" << endl;
    }
    return 0;
}
```


---

### Ejercicio 41
Lee dos números enteros: la clave que ingresó un usuario y la clave correcta. Si la clave ingresada es **distinta** de la correcta, imprime `Clave incorrecta`; si son iguales, imprime `Acceso concedido`. Usa el operador `!=`.

Entrada: `1234 5678` → Salida: `Clave incorrecta`
Entrada: `1234 1234` → Salida: `Acceso concedido`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int ingresada, correcta;
    cin >> ingresada >> correcta;
    if (ingresada != correcta) {
        cout << "Clave incorrecta" << endl;
    } else {
        cout << "Acceso concedido" << endl;
    }
    return 0;
}
```


---

### Ejercicio 42
Lee un número entero. Si **no** está entre 10 y 20 (ambos inclusive), imprime `Fuera del rango`; si está dentro, imprime `Dentro del rango`. Resuélvelo escribiendo la condición de rango completa y **negándola** con `!`.

Entrada: `5` → Salida: `Fuera del rango`
Entrada: `15` → Salida: `Dentro del rango`
Entrada: `25` → Salida: `Fuera del rango`

**Solución:**
```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;
    if (!(n >= 10 && n <= 20)) {
        cout << "Fuera del rango" << endl;
    } else {
        cout << "Dentro del rango" << endl;
    }
    return 0;
}
```
