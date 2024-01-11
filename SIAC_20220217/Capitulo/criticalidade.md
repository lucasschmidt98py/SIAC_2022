# Número Esperado de Nêutrons

Relembrando:

$$ E(n) = [ \frac{\partial g(z,t)}{\partial z} ]_{z = 1} = m_1(t) $$

$$ E(\nu) = [ \frac{dq(z) }{dz} ]_{z = 1} = q_1 $$


Da BKE, tomando a derivada parcial e avaliznado g em 1, encontramos:

$$ m_1(t) = Qq_1 \int_{0}^{t} exp(-Q(t-u))m_1(u)du + exp(-Qt) $$

Resolvendo em termos da transformada de Laplace:

$$ \mathcal{L}(m_1(t)) = \int_{0}^{\infty} m_1(t)dt exp(-st)dt  $$

Encontramos:

$$ \mathcal{L}(m_1(t)) = \frac{1}{s + Q(1-q_1)} $$

e assim:

$$ m_1(t) = \mathcal{L}^{-1}(m_1(t)) = exp(\kappa t) $$

em que 

$$ \kappa = Q(q_1 - 1) $$

Se $\kappa < 0$ , o processo é dito subcrítico. Se $\kappa = 0$ , o processo é dito crítico. Se $\kappa > 0$ , o processo é dito supercrítico.

Para o Urânio-235 , $q_1 \approx 2 $

## Probabilidade de Extinção

A probabilidade de extinção $p_0(t)$ é a probabilidade de que a população neutrônica venha a morrer para um valor assintótico t:

Temos simplesmente que:

$$ g(0,t) = p_0(t) $$

Além disso, no intervalo $0 < s < 1$ , a função g(z,t) é crescente. Assim:

$$ g( g(0,1) , t) = g( 0 , t + 1) \geq g(0,t) $$

Ou seja:

$$ p_0(t+1) \geq p_0(t) $$

## Formulação por Gerações

Consideremos agora $P(s) = \sum p_k s^k$ a função geradora da variável $X_1$ em que $X_n$ representa o tamanho da n-geração. E seja:

$$x_n = P(X_n = 0) = P_n(0)$$

Pelos mesmos argumentos anteriores , temos:

$$x_{n+1} = P(x_n) \geq P(x_{n-1}) = x_n $$

em que chegamos na equação de ponto-fixo:

$$\eta = P(\eta) $$

Pode-se demonstrar que se $E(\nu) \leq 1$ ,então a probablidade de que haja a extinção da população em algum momento, tende para 1. Se $1 \leq E(\nu)$ , então existe uma raiz $\eta$ que é o limite da probabilidade de extinção da população.