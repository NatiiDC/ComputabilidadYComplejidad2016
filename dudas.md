# Dudas

## 1

> A es incontable, B es contable. ¿`A ∩ B` es infinito incontable?

B es contable, por lo tanto cualquier subconjunto de B es contable, por lo tanto `A ∩ B` es contable.

## 2

> Siendo F = {f / f : N -> N}. ¿|F| ≤ |N²|?

G es el conjunto de las funciones que, para cada N' en ρ(ℕ) dicen si un n pertenece a N'. Como ρ(ℕ) es infinito incontable, y ∃ un g para cada ρ(ℕ), G es infinito incontable. Como G es sólo un subconjunto de F, F es infinito incontable. Como N² es infinito contable, |N²| ≤ |F|. Por lo tanto, la proposición es falsa.

## 3

> Existe una reducción L1 α_p L2 para:
>
> * L1 = {0ⁿ1 | n ≥ 0} y L2 = L_D

Sí! M_f consistiría en ejecutar M1, para cada qA generar algun `<M>` / `<M> ∉ L(M)`, y para cada qR escribir algún código inválido de MT.

> * L1 = L_u y L2 = {0ⁿ / n > 10}

No! Dado un (<M>, w), cuando M rechaza a w loopeando, L_u no termina, por lo que no podríamos construir una máquina M_f que emule L_u para que cuando rechace construya un w' ∈ L2. Por otro lado, la reducción de un L1 a un L2 implica que L1 no es más complejo que L2. En este caso L_u es claramente más complejo que L2.

## 4

> Dada M una MT DIS, ¿siempre se puede construir una M' equivalente que comienza con el cabezal apuntando a cualquier lugar de la cinta? ¿Y si comienza siempre a la derecha (alejada un número desconocido de celdas)?

En general se puede. Pero no siempre: para aquellos lenguajes que incluyen a λ, la MT no podría saber cuándo encontró el "comienzo" de la cinta.

## 5

Antes que nada, un poco de repaso sobre notación. `f👎🏽 ∈ O(g(n))` sii `f(n') ≤ c * g(n')` siendo `c` una constante cualquiera y `n'` un número mayor que un cierto `n` fijo.

> * tA1(n) ∈ O(n²)
> * tA2(n) ∈ O(n³)
> * n1, n2 ∈ N
> * n1 < n2
>
> Es posible que:
>
> *a*. ¿tA1(n2) > tA2(n1)?

Sí. `tA1(x) = 100 * x^2`, `tA2(x) = x^3`, `n1 = 2`, `n2 = 3`

> *b*. ¿∀n ∈ [n1,n2], tA1(n) > tA2(n)?

Sí. `tA1(x) = 100 * x^2`, `tA2(x) = x^3`, `n1 = 2`, `n2 = 3`

> *c*. ¿∀n ∈ N, tA1(n) > tA2(n)?

No. Seguramente va contra la definición de O👎🏽.

## 6

> ¿∃ L_d α L_u?

## 7

> ∃ HP α L1. ¿L1 ∉ RE?

No necesariamente. Que exista una reducción de L1 a L2 significa que L1 no es más complejo que L2. En este caso, HP no es más complejo que L1. Como HP ∈ RE, L1 puede ser igual de complejo y pertenecer a RE, o bien puede ser más complejo y no pertenecer a RE. Un contraejemplo es L1 = L_d.

## 8

> HP ∈ R. ¿L_d también? ¿Y L_u?

Sí. Ver que se puede construir una M / L(M) ∈ R.

## 9

> ¿(L1 ∪ L2 ∈ R) -> (L1 ∈ R) y (L2 ∈ R)?

No. Contraejemplo: `L1 = Σ*`, `L2 = L_d`.

## 10

> TSP ∈ NPC. P ≠ NP. ¿∃ algoritmo que resuelve eficientemente TSP?

No.
