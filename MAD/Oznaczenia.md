#Math
# Suma i iloczyn
## [[Notacja matematyczna w markdown (latex)#^040b17|Suma]]
$j, k \in \mathbb{Z} , j \leq k$

$$\sum_{i = j}^{k}x_{i}= x_{j} + x_{j+1} + \ldots + x_k$$
w $x_i$ przechodź po kolei po liczbach zaczynając od $i$ kończąc (**WŁĄCZNIE**) na $k$

*np:*
$$\sum_{i=0}^{3} i = 0 + 1 + 2 + 3 = 6$$
## [[Notacja matematyczna w markdown (latex)#^86005b|Iloczyn]]
$j, k \in \mathbb{Z}, j \leq k$
$$\prod_{i=j}^{k}x = x_{j} \times x_{j+1}\times \ldots \times x_{k}$$
*np:*
$$\prod_{i = 1}^{4}i = 1\times2\times3\times4 = 4! = 24$$
# Zbiory

## Różnica symetryczna (Suma zbiorów minus ich część wspólna)
$$A \oplus B = (A\setminus B)\cup(B\setminus A) $$
np:
Dla $A = \{1, 2, 3\}$ oraz $B = \{2, 4\}$
$$A \oplus B = \{1, 3, 4\}$$
`Dla 3 lub więcej zbiorów trzeba najpierw zrobić różnice dwóch a potem wynik z trzecim i tak dalej`

## Iloczyn Kartezjański (Wynikiem jest zbiór par liczb)
$$A \times B = \{(x, y):x\in A, y\in B\} $$

np:
Dla $A = \{1, 2, 3\}$ oraz $B = \{2, 4\}$
$$A \times B = \{(1, 2), (1, 4), (2, 2), (2,4), (3, 2), (3, 4)\}$$
## Dopełnienie zbioru
$U - \text{Uniwersum, przestrzeń}$
Dopełnienie zbioru $A\quad \text{to}\quad U \setminus A \text{ oznaczane jako }, \bar{A}$
np:
$U = \mathbb{N},\quad A = \{1, 2, 3, 4\}$
$$\bar{A} = \{5,\ldots\} \text{ lub inaczej } \mathbb{N} \setminus \{1, 2, 3, 4\}$$
# Działania na zbiorach
## Suma
$$\bigcup_{1\leq i \leq k}A_{i}= \{x:x\in A_{i} \text{ dla pewnego } 1\leq i \leq k\}$$
## Iloczyn (przekrój)
$$\bigcap_{1\leq i \leq k} A_{i} = \{x:x \in A_{i} \text{ dla każdego } 1 \leq i \leq k\}$$
## Różnica symetryczna:
$$\bigoplus_{1 \leq i \leq k} A_{i} = \begin{cases}A_{1} \oplus A_{2} & \text{jeśli k = 2}\\ \bigoplus_{1 \leq i \leq k-1} A_{i}\oplus A_{k}&\text{w przeciwnym wypadku }\end{cases}$$

### Przykłady
rodzina zbiorów $\mathcal{A}=\{A_{1}, A_{2}, \ldots, A_{k}\}$
zbiór indeksów $I = \{1, 2, 3, 4, 5\}$
dla każdego $i \in I$ określamy zbiór $A_{i} = \{x \in \mathbb{N} : i \leq x \leq 2i\}$

$$\bigcup_{i\in I} A_{i} = \{1, 2\}\cup\{2, 3, 4\}\cup\{3, 4, 5, 6\}\cup\{4, 5, 6, 7, 8\}\cup\{5, 6, 7, 8, 9, 10\} = \{1, \ldots , 10\}$$
$$\bigcap_{i\in I}A_{i} = \{1, 2\}\cap \{2, 3, 4\}\cap\{3, 4, 5, 6\}\cap\{4, 5, 6, 7, 8\}\cap\{5, 6, 7, 8, 9, 10\} = \emptyset$$

