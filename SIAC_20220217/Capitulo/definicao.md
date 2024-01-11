# Definições

Seja $\tau$ o intervalo de tempo entre a aparição do nêutron no meio , $t_0$ e sua interação. Iremos supor que $\tau$ segue uma distribuição de Poisson:


$$ P(\tau > t-t_0|t_0) = exp(-Q(t-t_0)) $$

Em que Q é a intensidade da reação e se relaciona com a Sessão de Choque da seguinte forma:

Uma reação ocorre se e somente se:

$$ P(\chi > x-x_0|x_0) = P(\tau > t-t_0|t_0) $$

Assim , tomando a inversa:

$$ ln(\xi) = -Q \delta t = -\Sigma \delta x $$

$$ Q = \Sigma v $$

Ainda, o número $\nu$ representa o número de novas particulas na reação. Assim, seja

$$ P(\nu = k) = f_k $$

a probabilidade de que dado uma interação , $k$ novos nêutrons são gerados no meio. 

As grandezas $Q$ e $f_k$ irão determinar o estado do meio multiplicativo. 

Seja:

$$ P(n(t) = n | n(0) = 1) = p_n(t) $$

a probabilidade de transição do estado inicial que possui um nêutron, para o estado com n nêutrons no instante t.
O processo é chamado homogêneo quando a probabilidade de transição depende apenas do intervalo de tempo $t-t_0$

Seja a função geradora:


$$g(z,t) = E(Z^{n(t)}|n(0) = 1) = \sum_{n = 0}^{\infty} p_n(t)z^n$$


Além disso, seja a função geradora básica:

$$ q(z) = E(z^\nu) = \sum_{k = 0}^{\infty} f_k z^k $$

Como propriedade básica da função geradora, temos:

$$ E(n) = [ \frac{\partial g(z,t)}{\partial z} ]_{z = 1} $$
