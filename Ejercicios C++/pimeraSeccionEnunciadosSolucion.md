# Enunciados progcomp C++


---

### 1. El despertar de Chip
```cpp
#include <iostream>
using namespace std;
int main() {
    cout << "¡Hola, mundo!" << endl;
    return 0;
}
```

---

### 2. La primera escalera
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

### 3. La cuenta regresiva
```cpp
#include <iostream>
using namespace std;
int main() {
    cout << 3 << " " << 2 << " " << 1 << endl;
    return 0;
}
```

---

### 4. El casillero
```cpp
#include <iostream>
using namespace std;
int main() {
    int n;
    cin >> n;
    cout << "El número guardado es " << n << endl;
    return 0;
}
```

---

### 5. El truco del mago
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

### 6. Dos cofres
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

### 7. Las galletas que quedan
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

### 8. La caja de chocolates
```cpp
#include <iostream>
using namespace std;
int main() {
    int f, c;
    cin >> f >> c;
    cout << f * c << endl;
    return 0;
}
```

---

### 9. El reparto justo
```cpp
#include <iostream>
using namespace std;
int main() {
    int n, k;
    cin >> n >> k;
    cout << n / k << endl;
    return 0;
}
```

---

### 10. Lo que sobra
```cpp
#include <iostream>
using namespace std;
int main() {
    int n, k;
    cin >> n >> k;
    cout << n % k << endl;
    return 0;
}
```

---

### 11. El patio cuadrado
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

### 12. El marco de la foto
```cpp
#include <iostream>
using namespace std;
int main() {
    int l, a;
    cin >> l >> a;
    cout << 2 * (l + a) << endl;
    return 0;
}
```

---

### 13. Empalmando cintas
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

### 14. Mitad y mitad
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

### 15. El cronómetro
```cpp
#include <iostream>
using namespace std;
int main() {
    int S;
    cin >> S;
    cout << S / 60 << endl;
    cout << S % 60 << endl;
    return 0;
}
```

---

### 16. La pizza gigante
```cpp
#include <iostream>
using namespace std;
int main() {
    int r;
    cin >> r;
    cout << 3.14 * r * r << endl;
    return 0;
}
```

---

### 17. El kiosco
```cpp
#include <iostream>
using namespace std;
int main() {
    int cantidad, precio, pago;
    cin >> cantidad >> precio >> pago;
    int total = cantidad * precio;
    cout << total << endl;
    cout << pago - total << endl;
    return 0;
}
```

---

### 18. Ficha de jugador
```cpp
#include <iostream>
#include <string>
using namespace std;
int main() {
    string nombre;
    int ataque, defensa, velocidad;
    cin >> nombre >> ataque >> defensa >> velocidad;
    cout << "Jugador: " << nombre << endl;
    cout << "Poder total: " << ataque + defensa + velocidad << endl;
    return 0;
}
```

---

### 19. Reporte de fin de temporada (final)
```cpp
#include <iostream>
#include <string>
using namespace std;
int main() {
    string nombre;
    int mapas, totales;
    int p1, p2, p3;
    double bonus;
    int minutos;

    cin >> nombre >> mapas >> totales >> p1 >> p2 >> p3 >> bonus >> minutos;

    int suma = p1 + p2 + p3;

    cout << "Explorador: " << nombre << endl;
    cout << "Mapas: " << mapas << " de " << totales << " mapas" << endl;
    cout << "Faltan: " << totales - mapas << " mapas" << endl;
    cout << "Puntos por mapas: " << mapas * 10 << endl;
    cout << "Suma de desafios: " << suma << endl;
    cout << "Bonus: " << bonus << endl;
    cout << "Promedio (3 desafios y bonus): " << (suma + bonus) / 4.0 << endl;
    cout << "Tiempo de juego: " << minutos / 60 << " h y " << minutos % 60 << " min" << endl;
    return 0;
}
```
