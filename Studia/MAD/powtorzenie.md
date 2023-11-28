# Powtórka na kolokwium MAD

## Logika

### __Implikacja:__
| $\alpha$   | $\beta$    | $\alpha \implies \beta$|
|---------------- |--------------- | --------------- |
|  0   | 0    |  1  |
|  0   | 1    |  1  |
|  1   | 0    |  0  |
|  1   | 1    |  1  |

### __Reguły dowodzenia:__
- Reguła odrywania: Jeżeli prawdziwe są wszystkie formuły nad kreską (przesłanki) to prawdziwa jest także reguła pod kreską(wniosek) np. $\dfrac{\alpha, \alpha \implies \beta}{\beta}$

| $\alpha$    | $\alpha \implies \beta$| $\beta$|
|---------------- | --------------- | --------------- |
| Item1.1    | Item2.1    | Item3.1    |
| Item1.2    | Item2.2    | Item3.2    |
| Item1.3   | Item2.3   | Item3.3   |
| Item1.4   | Item2.4   | Item3.4   |

### __Prawa de Morgana:__
- $\neg (\forall_x \phi(x)) \iff \exists_x \neg \phi(x)$
np. $\exists_{n \in N} 2|n \to \forall_{n\in N} \neg(2|n)$
- $\neg (\exists_x \phi(x)) \iff \forall_x \neg \phi(x)$

## Zbiory 
- Wszystkich podzbiorów zbioru $A$ jest $2^{|A|}$
- Rodzinę podzbiorów zbioru $A$ oznaczamy $\mathcal{P}(A) \text{ lub } 2^A$

### Relacje
__Przykłady:__

### $X = \{A, B, C\}, Y = \{ a, b \}$ ile jest relacji w zbiorze $X \times Y$? 

Odp.

$X \times Y = \{(A,a), (A,b),(B,a), (B,b), (C,a), (C,b)\}$

$|X \times Y| = 6$

(Relacja = dowolny podzbiór $X\times Y$)

$2^{|X\times Y|} = 2^6 = 32$

### Czy relacja $R = \{(A,a), (A,b), (B,a)\}$ jest funkcją?
Odp.

Nie ponieważ jednocześnie istnieje (A,a) oraz (A,b) i nie ma wartości dla C

### Relacja równoważności
Relację $R \subseteq X \times X$ nazywamy relacją równoważności $\iff$ jest ona(dla dowonlych $x,y \in X$):
1. zwrotna ($xRx$)
2. symetryczna ($xRy \implies yRx$)
3. przechodnia ($(xRy \land yRz) \implies xRz$)

Przykłady:
### $X = \{a,b,c\}, R = \{(x,y)\in X^2 | x \neq y\}$ 
$R = \{(a,b), (a,c), (b,a),(b,c), (c,a), (c,b)\}$

- zwrotna? Nie ($(a,a)$)
- symetryczna? Tak ($(a,b), (b,a)$)
- przechodnia? TODO
## Arytmetyka
W systemie o podstawie b liczba x ma $\lfloor \log_{b}{x}\rfloor + 1$

### system $u_2$:

$-50_2$ w ośmiu bitach to:

ABS:$|-50| = 50$

Zmiana na binarny: $50 = (110010)_2$

Zmiana z 6 na 8 bitów: $(00110010)_2$

Negacja: $(11001101)_2$

Dodawanie 1: $(11001101)_2 + 1 = (11001110)_2$

### zamiana spowrotem na 10:
$(0 * 2^0) + (1 * 2^1) + (1 * 2^2) + (1 * 2^3) + (0 * 2^4) + (0 * 2^5) + (1 * 2^6) - (-1 * 2^7) = 2 + 4 + 8 + 64 -128 = -50$

### Stało i zmiennopozycyjne liczby: 
| 4837.92 | 4.83792E3 |
|--------------- | --------------- |
| 0.034 | 3.4E-2|
| -12.0   | -1.2E1  |


### Algorytm szukania pierwiastka
$n = 256; \alpha = 2$

$k_d = 1; k_g = n$

to co wyjdzie to pierwistek naturalny stopnia $\alpha$ z n


| $k_d$    | $k_g$| $k_g - k_d \leq 1 ?$| $j = \lfloor \dfrac{k_d + k_g}{2}\rfloor$ | $j^\alpha = n ?$ | ?(>, <, =) |
|---------------- | --------------- | --------------- | --------------- | --------------- | ---|
|  1   | 256    |  $256-1 \leq $    | Item4.1    | Item5.1|  |  
| Item1.2   | Item2.2   | Item3.2   | Item4.2   | Item5.2   |   | 
| Item1.3   | Item2.3   | Item3.3   | Item4.3   | Item5.3   |   | 
| Item1.4   | Item2.4   | Item3.4   | Item4.4   | Item5.4   |   | 

jeżeli kg − kd ¬ 1, to
koniec, n nie jest potęgą;
w przeciwnym wypadku:
k +k
. j := b d 2 g c;
. jeżeli j α = n , to koniec, n jest potęgą j,
. jeżeli j α > n , to kg := j,
. jeżeli j α < n , to kd := j.


### $(1+x)^n = \sum_{k=0}^n {n \choose k} x^k$

np.

$(1+t)^8 = \sum_{k=0}^8 {n \choose k}t^k = {8 \choose 0}t^0 + {8 \choose 1}t^1 + \dots + {8 \choose 8} t^8$



