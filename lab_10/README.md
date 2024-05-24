# Recursão

Você já aprendeu que algoritmos recursivos para um certo problema são procedimentos que incluem instruções para resolver instâncias menores para o mesmo problema. Por esse motivo, é importante entender claramente qual é o conjunto de entradas (ou instâncias) do problema e qual é o conjunto de soluções (ou saídas) do problema. Quando tentamos resolver um problema de maneira recursiva, temos que considerar um ou mais casos básico, que são exemplos de instâncias resolvidas diretamente, e os demais casos, quando uma solução é obtida a partir de uma solução de uma ou mais instâncias menores do problema.

O objetivo desta tarefa é começarmos a pensar recursivamente. Assim, é obrigatório resolver cada um dos problemas seguintes utilizando recursão, mesmo que você conheça um algoritmo iterativo mais eficiente. Uma das vantagens de recursão é que as funções recursivas são normalmente muito simples e elegantes. Se seu programa para alguma das questões abaixo parecer muito complicado, então pare e repense seu algoritmo. E não deixe de tirar as dúvidas que aparecerem no canal do [Discord](https://discord.gg/cWJEU95G6M), ou com os PED/PADS.

## 1. Máximo

Dada uma lista de elementos, faça um programa `maximo.py` que encontra o maior elemento.

### Entrada

Uma sequência de números separados por espaço.

`19 21 24 23 10 29 24 8 23 29 8 6`

### Saída

O maior element da sequência.

`29`

## 2. Busca em um vetor ordenado

Dado um vetor de inteiros em ordem crescente e um número, faça um programa `busca_binaria.py` que realize uma busca binária e retorne o índice da posição desse número no vetor ou -1 se esse número não estiver no vetor.

### Entrada

Uma sequência de números separados por espaço e um número *i*.

```
0 4 5 6 7 10 10 15 20 23 24 25 26 29 29
29
```

### Saída

A posição de *i* na sequência ou -1.

`13`

## 3. Formiga de Langton

Um tabuleiro retangular tem diversos quadrados dispostos em uma grade de tamanho *m* x *n*, onde *m* e *n* são o número de linhas e o número de colunas, respectivamente. Cada um desses quadrados tem uma cor, que pode ser branco ou preto. Sobre esse tabuleiro, há uma formiga que se move de acordo com as seguintes regras:

* estando em um quadrado branco, ela vira 90° para a direita, muda a cor do quadrado para preto e avança uma unidade;
* estando em um quadrado preto, ela vira 90° para a esquerda, muda a cor do quadrado para branco e avança uma unidade.

Essa é uma [formiga de Langton](https://pt.wikipedia.org/wiki/Formiga_de_Langton). Crie um programa `langton.py` que mostre o estado do tabuleiro após iterações. Suponha que a formiga inicia no quadrado central do tabuleiro virada para baixo e que ela não sairá do tabuleiro em nenhuma das entradas de teste.

### Entrada

A primeira linha contém os inteiros *t*, *m* e *n*. É garantido que *m* e *n* são ímpares. As demais linhas correspondem às linhas do tabuleiro, de forma que um ponto `.` representa um quadrado branco e um caractere `#` representa um quadrado preto.

```
4 9 9
....#....
....#....
....#....
....#....
#########
....#....
....#....
....#....
....#....
```

### Saída

O estado final do tabuleiro.

```
....#....
....#....
....#....
....###..
####..###
....#....
....#....
....#....
....#....
```

## 4. Quick-sort

Faça um programa `quick_sort.py` que, ao receber uma lista de elementos, retorna essa lista em ordem crescente. Para isso, implemente o algoritmo de ordenação quick-sort.

### Entrada

Uma sequência de números separados por espaço.

`8 10 13 17 14 16 2 19 7 2 18 16`

### Saída

A sequência em ordem crescente.

`2 2 7 8 10 13 14 16 16 17 18 19`

## 5. Quase palíndromo

Uma string é um *k*-quase palíndromo se, ao compará-la com o seu inverso, tiver no máximo *k* caracteres diferentes. Por exemplo, `arara` é um *0*-quase palíndromo e `araro` é um *2*-quase palíndromo.

Crie um programa `quase_palindromo.py` que verfique se uma palavra é um *k*-quase palíndromo.

### Entrada

A primeira linha contém um número *k* e a segunda linha contém uma string.

```
2
araro
```

### Saída

Um linha contendo `sim` ou `nao`, dependendo se a string é um *k*-quase palíndromo.

`sim`

## 6. Todas as somas que levam a *n*

Dado um número *n*, encontre todas as combinações de somas de números positivos que resultam em *n*. Seu programa `soma_n.py` deverá imprimir todas as somas cujos termos estão em ordem crescente. As diferentes somas devem ser apresentadas em ordem lexicográfica, sem repetições.

### Entrada

O número *n*.

`5`

### Saída

Todas as combinações em ordem crescente.

```
1+1+1+1+1=5
1+1+1+2=5
1+1+3=5
1+2+2=5
1+4=5
2+3=5
5=5
```

## 7. Um caminho para escapar do labirinto

Faça um programa `caminho.py` que encontra um caminho (não necessariamente com comprimento mínimo) para atravessar um labirinto. O labirinto é representado por uma matriz sendo que as paredes são indicadas por `#`. A entrada e saída são indicadas por `E` e `S` respectivamente. É possível se mover em *4* direções: cima, baixo, esquerda e direita.

### Entrada

Um labirinto.

```
###E####
#      #
# #  # #
# ## # #
#  #   #
#####S##
```

### Saída

Um caminho na forma de uma sequência de coordenadas de matriz.

```
0 3
1 3
2 3
2 4
3 4
4 4
4 5
5 5
```

## Correção

Você pode discutir o lab e pedir ajuda no [Discord](https://discord.gg/cWJEU95G6M)

Pontos:
|Lab|Pontos|
|---|------|
|maximo.py|1|
|busca_binaria.py|1|
|langton.py|1|
|quick_sort.py|2|
|quase_palindromo.py|1|
|soma_n.py|2|
|caminho.py|2|

É obrigatório resolver todos os exercícios usando recursão, caso contrário a nota será *0* zero. Os exercícios serão corrigidos de forma automática usando o comando:

`python3 arquivo.py < entrada.in`

Se seu código der erro nesse comando a nota não vai ser computada. Entregue somente um arquivo *zip* com os arquivos `.py` e nada mais, por exemplo:

```
210404.zip
│   busca_binaria.py
│   maximo.py
│   ...
│   caminho.py
```

#### Peso 4

# [IMPORTANTE] Não plagiar!

![plagio](spotted.png)