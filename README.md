# C++ – Funkcja szablonowa `wypisz()`

## 📌 Opis projektu

Projekt przedstawia wykorzystanie **szablonów funkcji (Templates)** w języku C++.

Program zawiera uniwersalną funkcję `wypisz()`, która pozwala wyświetlać różne typy danych za pomocą tej samej nazwy funkcji.

## 🛠️ Obsługiwane typy danych

Program obsługuje:

- `int` – liczby całkowite
- `float` – liczby zmiennoprzecinkowe
- `string` – tekst
- `vector` – wektory
- `queue<int>` – kolejki liczb całkowitych
- `queue<string>` – kolejki napisów

## 💻 Technologie

- C++
- Templates (szablony funkcji)
- STL (Standard Template Library)

## ⚙️ Jak działa program?

W programie wykorzystano trzy przeciążenia funkcji `wypisz()`:

1. **Uniwersalna funkcja szablonowa** – wypisuje pojedyncze wartości, np. `int`, `float` i `string`.
2. **Funkcja dla vectora** – przechodzi przez wszystkie elementy wektora i wyświetla je na ekranie.
3. **Funkcja dla kolejki** – wyświetla elementy kolejki za pomocą `front()` i `pop()`.

Kolejka jest przekazywana przez kopię, dzięki czemu oryginalna kolejka nie zostaje zmieniona.

## ▶️ Przykład użycia

```cpp
int a = 5;
string s = "Ala";
float f = 5.5;

vector<int> v = {1, 2, 3, 4};

queue<int> q;
q.push(10);
q.push(20);
q.push(30);

wypisz(a);
wypisz(s);
wypisz(f);
wypisz(v);
wypisz(q);
```

## 📤 Przykładowy wynik

```text
5
Ala
5.5
1 2 3 4
10 20 30
```

## 🎯 Cel projektu

Celem projektu jest nauka:
- tworzenia szablonów funkcji (`template`)
- przeciążania funkcji
- korzystania z kontenerów STL
- obsługi `vector` i `queue`
- przekazywania argumentów do funkcji

---

**Projekt edukacyjny – C++ Templates & STL**
