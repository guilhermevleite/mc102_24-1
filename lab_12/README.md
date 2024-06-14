# Arquivos

O objetivo deste laboratório é praticar a leitura e escrita de arquivos em Python.

## Problema

No arquivo `primeiro_nome.txt` está uma lista com o primeiro nome de todos os membros de um organização, em outro arquivo, chamado `sobrenome.txt`, estão os sobrenomes desses membros, porém os sobrenomes estão na ordem invertida do arquivo `primeiro_nome.txt`. Faça um programa, chamado *`arquivos.py`*, que junte corretamente o nome e sobrenome de todos os membros, ordene os nomes em ordem alfabética e salve essa lista em um terceiro arquivo, chamado `membros.md`, usando notação Markdown para listas.

### Entrada

> primeiro_nome.txt
```
santiago
vinicius
guilherme
paulo
ieremies
```

> sobrenome.txt
```
romero
santos
leite
soares
ravelo
```

### Saída

> membros.md
```
# Organizacao
1. Membros da organizacao
    1. guilherme leite
    1. ieremies romero
    1. paulo santos
    1. santiago ravelo
    1. vinicius soares
```

Obs.: A identação é de 4 (quatro) espaços em branco.
Curiosidade: Abra o arquivo membros.md em um visualizador de [Markdown](https://markdownlivepreview.com)

## Correção

Não faça a leitura dos arquivos usando `input()`, utilize leitura e escrita aprendidos na aula de arquivos. Entregue o laboratório pelo Classroom utilizando o mesmo padrão dos anteriores, ou seja, um arquivo *zip* com seu RA no nome e *somente* o programa `arquivos.py` lá dentro, veja o exemplo:

```
210404.zip
│   arquivos.py
```

É permitido utilizar `sort()` para ordenar a lista. Em caso de dúvidas, [Discord](https://discord.gg/cWJEU95G6M) ou os horários de monitoria.

A correção será feita com os seguintes comandos:

```
python3 arquivos.py
diff --side-by-side resposta_correta.md membros.md
```

## Peso

Peso: 4