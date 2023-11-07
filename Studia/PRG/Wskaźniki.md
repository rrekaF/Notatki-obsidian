## Wskaźnik typu void:
pasuje do każdego typu zmiennej
```cpp
int *wi1, *wi2;
float *wf1;
wi1 = wi2; // OK
wi1 = wf1 // NIE OK

void *wv;
wv = wi1; // OK
wi1 = (int*) wv // Trzeba castować przy wyciąganiu 
```
## Wskaźnik do tablicy
Mając pierwszy element i znając rozmiar elementów możemy poznać wartość reszty elementów.
```cpp
int *w
int tab[20]

//Zapisy równoważne
w = &tab[i]
w = tab

tab + 4;
&tab[4];

tab[5]
*(tab+5)
```

## Rezerwowanie pamięci
Mocno rekomendowanie jest zwalnianie pamięci aby uniknąć wycieków pamięci .
```cpp
char wchar*;
wchar = new char;
delete wchar;

float w*;
w = new float[10];
delete []w;
```
 - Programiasta decyduje o czasie życia tych obiektów
 - Nie mają nazwy, tylko wskaźnikami się nimi operuje
 - Tylko operatory statyczne mają defaultowo 0 przy *new* będą to przypadkowe wartości
 
## Dynamiczna alokacja pamięci tablicy

```cpp
int w_tab*
w_tab = new int[rozmiar]

w_tab* = 50;
t_tab[0] = 50;

(w_tab + 4)* = 100
w_tab[4] = 100

delete []w_tab
```

## Stałe wskaźniki
```cpp
int dworzer;
int *const wi = &dworzec;
```
Albo stały możę być wskaźnik czyli pokazuje cał czas na to samo miejsce w pamięci, albo wartość może być stała i wskaźnik wskazywać na różne stałe zmienne.

stały wskaźnik i stała zmienna:
```cpp
const float *const wf = &a;
```

```cpp
w = tab; // Adres 1 elementu tablicy

w = func(); // Adres zmiennej

float *wf;
wf = new float; // Adres nowej zmiennej(alokowanie pamięci)
```

## Zalety wskaźników
- zwiększają efektywność pracy z tablicami
- dynamiczna alokacja pamięci 
- przekazywanie funkcjom oryginalne zmienne a nie jej kopie
- współpraca z urządzeniem zewnętrznym ( np miernikiem )
