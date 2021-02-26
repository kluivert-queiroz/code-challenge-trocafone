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


## Desafio #1 CamelCase

O propósito é transformar uma sentença para o estilo camelCase:
```js
camelCase("one word") // resulta oneWord
camelCase("I said one word!!") // resulta iSaidOneWord
```

## Desafio #2 DeduplicateSentence

O propósito e remover palavras que são duplicadas em sequência.
Por exemplo
```js
deduplicateSentence("Hello Bob. Hello Ana.") // resulta "Hello Bob" mesmo hello repetindo na frase.
deduplicateSentence("Hello Hello Bob") // resulta "Hello Bob"
```

## Desafio #3 FindFirstBiggestWord

O propósito é encontrar a primeira maior palavra de uma sentença.

```js
findFirstBiggestWord("Hello Bob") // resulta em "Hello"
```

## Informações
Palavras são conjuntos de letras alfanuméricos. Ou seja símbolos e acentuações como `!@#...` não são considerados palavras para o desafio.

Exemplo:
```
Palavras:
Hello!!! - A palavra é Hello
@Uncle123 - A palavra é Uncle
```