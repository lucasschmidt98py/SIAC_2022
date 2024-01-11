# O Processo Ramificativo e o processo Markoviano

## Processo Markoviano

Um processo randômico n(t) gera um processo de Markov se a probabilidade de transição:

$$ P(n(t) = j | n(0) = i) = p_{ij}(t) $$

Se satisfaz as condições:

* $$0 \leq p_{ij}(t) $$


* $$\sum_{j = 0}^{\infty} p_{ij}(t) = 1$$


* $$p_{ij}(t) = \sum_{k = 0}^{\infty} p_{jk}(u)p_{kj}(t-u)$$ (Equação de Chapman–Kolmogorov)


* $$p_{ij} = \delta_{ij}$$

A equação de Chapman-Kolmogorov é pode ser derivado diretamente da propridade mais fundamental dos processos markovianos:

$$ E(X_{n+1}|X_{n}) = E(X_{n+1}|X_{n},X_{n-1},X_{n-2},...,X_{1}) $$

## O Processo de Ramificação

Um processo Markoviano n(t) será chamado processo Markoviano ramificativo se as probabilidades de transição forem dadas por:

$$ p_{ij}(t) = \sum_{n_1 + n_2 + ... + n_k = n} p_{n_1}(t)p_{n_2}(t)...p_{n_k}(t) $$

A probabilidade $p_{ij}$ pode ainda ser vista como uma k-convolução de uma sequência ${S_i}$ (Feller). Tal notação pode tornar mais intuitivo a estrutura de semi-grupo da função geradora como será derivado a seguir:

## Semi-Grupos de Markov

Das equações:

$$ p_n(t+u) = \sum_{k = 0}^{\infty}p_k(t)p_{kn}(u) $$

e

$$ p_{kn}(u) = \sum_{n_1 + n_2 + ... + n_k = n}\prod_{i = 1}^{k}p_{n_{i}} $$

Temos:

$$ g(z,t + u) = \sum_{k = 0}^{\infty} p_k(t) \sum_{n = 0}^{\infty}p_{kn}(u)z^n = \sum_{k = 0}^{\infty}p_k(t)[g(z,u)]^k = g( g(z,u) , t) = $$

Ou seja:

$$ g_{t+s} = g_t \circ g_s $$

O que define um semi-grupo!

O processo Markoviano de ramificativo pode ser pensado como um processo iterativo, com a geração do estado futuro como uma aplicação do funcional $g(z, \circ)$ sob o passado.  