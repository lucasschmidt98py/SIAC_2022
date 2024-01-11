# Um pouco sobre o código

## C++

A instrumentação do problema foi feita de duas formas. Um primeiro código escrito em C++ cria os cenários ramificativos n vezes, que por sua vez, gera n planilhas no HD do computador, librando espaço na memória. Um protótipo da versão do problema pontual está sendo desenvolvido utilizando o projeto Cuda.

O código é orientado a objeto, o que significa que cada nêutron é um objeto alocado num espaço da memória , que recebe os atributos 'tempo de nascimento' , 'tempo de morte' , 'geração' e sessão de choque. A cada iteração, números randômicos são gerados , o que determinará o número de filhos de um neutron-pai, bem como o tempo com o qual o mesmo filho morrerá. De um ponto de vista filosófico, sua existência precede sua essência.

Caso uma geração não produza novos filhos, a simulação terminará com a mensagem:

``` C++
cout << "A árvore morreu" << endl;
```

O intervalo de tempo com que o nêutron permanece vivo no meio é dado por:

$$ \delta t_i = \frac{- log(\xi)}{\Sigma}  $$



## Python

Na segunda etapa, códigos Python analisam as planilhas de modo a calcular frequência de ocorrência de eventos ao longo das simulações. Tais frequências se tornam probabilidades para grandes valores do número de simulações.

Bibliotecas usadas:

* numpy
* pandas
* matplotlib
* plotly
* numba