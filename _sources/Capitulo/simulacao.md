# Yule-Furry process

O processo de Yule-Furry , tem-se que $f_0 = f_1 = 0$ e $f_2 = 1$

Da equação $BKE$ , tem-se

$$\frac{dg(z,t)}{g(z,t)(g(z,t) - 1)} = Qdt$$

$$ Cexp(-Qt) = \frac{g(z,t)}{g(z,t) - 1} $$

em que aplicando a condição inicial $g(z,0) = z$:

$$ C = \frac{z}{z-1} $$

e assim:

$$ g(z,t) = \frac{zexp(-Qt)}{1 - z(1 - exp(-Qt))} $$

![](../fig/geradora_analitica.png)

É conhecido da Teoria das Equações Diferenciais, que toda solução da BKE é solução se e somente se é solução da FKE

## Simulação Mostrando a convergência dos valores

![](../fig/geradora_branching_analitic.png)

## População e Distribuição de Probabilidade no Reator

### Crítico
![regime crítico](../fig/critico_populacao.png)
![regime critico](../fig/probabilidade_cr.png)

### Subcrítico
![regime subritico](../fig/subcritico_populacao.png)
![regime subcritico](../fig/probabilidade_subcr.png)

### Supercrítico
![regime supercritico](../fig/populacao_supercritico.png)
![regime supercritico](../fig/probabilidade_supercr.png)
