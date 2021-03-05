# Code Challenge Trocafone

Este repositório contém os testes unitários para validação do desafio técnico realizado para admissão.

Implemente as funções necessárias para passar nos testes automatizados e envie para o recrutador.

Utilize o comando abaixo para validar as funções.
```
npm run test
```

## Como começar

 Clone o repositório e execute:
 ```
 npm install
 ```
 E você estará pronto para começar o desafio.

## Desafio #1 SortList

O objetivo é reordenar uma lista passada em ordem alfabetica crescente, ou seja:
```js
sortList([3,2,1]); // deve retornar [1,2,3]
sortList([6,4,5]); // deve retornar [4,5,6]
sortList(["c","b","a"]); // deve retornar ["a","b", "c"]
```

## Desafio #2 CamelCase

O propósito é transformar uma sentença para o estilo camelCase:
```js
camelCase("one word") // resulta oneWord
camelCase("I said one word!!") // resulta iSaidOneWord
```

## Desafio #3 DeduplicateSentence

O propósito e remover palavras que são duplicadas em sequência.
Por exemplo
```js
deduplicateSentence("Hello Bob. Hello Ana.") // resulta "Hello Bob. Hello Ana." mesmo hello repetindo na frase.
deduplicateSentence("Hello Hello Bob") // resulta "Hello Bob"
```

## Desafio #4 FindFirstBiggestWord

O propósito é encontrar a primeira maior palavra de uma sentença.
Considerando apenas [palavras](#informações).

```javascript
findFirstBiggestWord("Hello Bob") // resulta em "Hello"
findFirstBiggestWord("You're right!") // resulta em "right"
```
## Desafio #5 WordMesh (Bônus)

O propósito é receber uma matriz de com N palavras que podem ou não ser "ligadas" e retornar apenas os "conectores" entre as palavras.
Uma ligação de palavras neste desafio é quando o final de uma palavra contém as mesmas letras que o começo de outra. 

Exemplo de palavras ligáveis:
```
apply 	 -> plywood
apple 	 -> each
behemoth -> mother
...
```

Exemplo de palavras não ligáveis:
```
apply -> playground
apple -> peggy
...
```

Caso todas as palavras possam ser ligadas deve retornar apenas os "conectores" das palavras.
Exemplo:

```javascript
wordMesh(["apply", "plywood"]) // resulta em "ply", porque ply é o final de "apply" e o começo de "plywood"
wordMesh(["apple", "each"]) // resulta em "e"
wordMesh(["word", "notmesh"]) // false, porque o final de "word" não é começo de "notmesh"

```
A função deve suportar matrizes com N palavras, ou seja, de tamanho indeterminado, mas o tamanho sempre será par para o propósito do desafio.
```js
wordMesh(["apple", "each", "chainsmoker", "river"]) // echr
```
O resultado é `echr`, porque:
- `apple` e `each` ligam por `e`, 
- `each` e `chainsmoker` ligam por `ch` 
- e `chainsmoker` e `river` ligam por `r`


Se alguma das palavras não "ligar" com a próxima, a função deve retornar `false`.

## Informações
Palavras são conjuntos de letras alfanuméricos. Ou seja símbolos e acentuações como `!@#...` não são considerados palavras para o desafio.

Exemplo:
```
Palavras:
Hello!!! - A palavra é Hello
@Uncle123 - A palavra é Uncle
```
