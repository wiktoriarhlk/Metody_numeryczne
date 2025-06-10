# Metody numeryczne – biblioteka obliczeniowa

Projekt biblioteki numerycznej realizowany w ramach zajęć z metod numerycznych. Zawiera implementacje i testy podstawowych metod obliczeniowych wykorzystywanych w analizie numerycznej.

# 📁 Struktura projektu

```
Metody_numeryczne-main/
├── include/               # Pliki nagłówkowe (*.h)
├── src/                   # Implementacje funkcji (*.cpp)
├── tests/                 # Testy jednostkowe
├── examples/              # Przykłady użycia funkcji bibliotecznych
├── CMakeLists.txt         # Konfiguracja budowania CMake
└── README.md              # Niniejszy plik
```

# Metody numeryczne – projekt biblioteki obliczeniowej

Projekt zrealizowany w ramach zajęć z metod numerycznych. Celem było utworzenie biblioteki implementującej wybrane algorytmy numeryczne wraz z testami jednostkowymi i przykładami użycia.


----------------------------------------------------------------------------

## 📚 Zakres funkcjonalny

Biblioteka obejmuje metody numeryczne w następujących kategoriach:

### 🔹 Układy równań liniowych
- Eliminacja Gaussa bez wyboru
- Eliminacja Gaussa z częściowym wyborem

### 🔹 Interpolacja
- Interpolacja wielomianowa (Lagrange’a)
- Obliczanie wartości wielomianu interpolacyjnego

### 🔹 Aproksymacja
- Metoda najmniejszych kwadratów (regresja liniowa)

### 🔹 Całkowanie numeryczne
- Metoda trapezów
- Metoda Simpsona
- Kwadratura Gaussa-Legendre’a (dla n = 2, 3, 4, 5)

### 🔹 Równania różniczkowe zwyczajne (ODE)
- Metoda Eulera
- Metoda Heuna (Euler poprawiony)
- Metoda punktu środkowego
- Metoda Rungego-Kutty czwartego rzędu (RK4)

### 🔹 Równania nieliniowe
- Metoda Newtona
- Metoda siecznych

-----------------------------------------------------------------------------------------

## 🛠️ Kompilacja projektu

### ✅ Wymagania

- Kompilator zgodny z C++17 (np. g++, clang++, MSVC)
- CMake w wersji 3.10 lub wyższej

### 💻 Budowanie w terminalu (Linux / Mac / WSL / MinGW)

```bash
mkdir build
cd build
cmake ..
make
```

### Budowanie (Visual Studio)
- Otwórz folder jako projekt CMake
- Wybierz „element startowy” (np. test_approximation.exe)
- Naciśnij ▶ aby uruchomić

## ▶️ Uruchamianie

Testy:
```bash
./test_approximation
./test_linear_system_solver
./test_linear_solver
./test_integration
./test_nonlinear_solver
./test_ode_solver
```

Przykłady:
```bash
./example_approximation
./example_system_solver
./example_interpolation
./example_integration
./example_ode_solver
./example_nonlinear_solver
```

## ✅ Testowanie

Każda funkcja posiada testy jednostkowe (`tests/`) sprawdzające poprawność działania oraz przypadki brzegowe.


## 👨‍💻 Autor

Projekt został opracowany przez Joannę Polak i Wiktorię Rychlak w ramach ćwiczeń z przedmiotu Metody numeryczne.
