# Voo

Neste lab você está ajudando a planejar uma viagem e precisa descobrir qual voo é o mais adequado para suas férias. Para isso, utilize *classes* e seu conhecimento acumulado para resolver este problema.

---

Jairzinho sente que no futuro próximo precisará passar um tempo fora do país, mas apesar de 4 anos "juntando" dinheiro, a grana está curta. Por isso, ele deve economizar para sua viagem. Enquanto isso, ele acompanha os valores e planeja sua ~fuga~ férias. O destino não importa, desde que ele consiga voltar na data definida.

Construa um programa para Jairzinho registrar as ofertas de voos que ele encontra e escolha a data de ida e volta ideal. Dentre todas as ofertas, ele deve comprar as passagens mais baratas de ida e volta cujas datas estejam pelo menos quatro dias dentro do seu período de "férias". Enquanto ele sonha com suas férias, muitas coisas podem acontecer, novas ofertas podem aparecer, os preços podem mudar, ou um voo pode ser cancelado. Para onde ele vai viajar?

## Entrada

A entrada contém várias operações. Cada uma consiste em uma linha com o nome da operação, que talvez é seguida de uma ou mais linhas com os parâmetros.

* **`registrar`**: registra um novo voo com os parâmetros: número do voo, código de três letras do aeroporto de origem, código de três letras do aeroporto de destino, data do voo no formato dd/mm/aaaa e valor em reais.

* **`alterar`**: altera o valor de um voo já registrado com parâmetros número do voo e novo valor em reais.

* **`cancelar`**: cancela um voo já registrado com parâmetro número do voo.

* **`planejar`**: informa os dados de Jairzinho e termina o programa com parâmetros: código do aeroporto de saída e datas do primeiro e do último dias de férias.

*Obs.: Você pode supor que todos os voos ocorrem nos anos de 2021 ou 2022.*

### Exemplo de entrada

```
registrar
488
XAP CGR
05/08/2021
29.87

registrar
907
CGR XAP
01/08/2021
300.43

registrar
767
CGR XAP
01/08/2021
335.37

alterar
767 324.68

cancelar
907

planejar
CGR
29/07/2021 06/08/2021
```

## Saída

A saída deve informar toda vez que o valor de um voo foi alterado com a frase `X valor alterado de Y para Z`, onde X é o código do voo, Y é o valor anterior e Z é o novo valor. O final da saída deve conter duas linhas, uma com o código de origem e outra com o código do destino.

### Exemplo de saída

```
767 valor alterado de 335.37 para 324.68
767
488
```


## Critérios

É obrigatório que você crie *classes* para os **voos** e para as **datas**. Complete o arquivo [passagem.py](./passagem.py), definindo as variáveis e funções necessárias. Por exemplo, um função para dizer se dois A e B voos são possíveis. Lembre-se de testar o código com o arquivo [entrada.in](./entrada.in).

#### Peso: 3
