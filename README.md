# Trabalho 2 - Compiladores

## Alunos e RAs

- Bruno Matos de Souza - 769754
- Eduardo Minoru Takeda - 776857
- Fernando Eiji Hieda - 769768

## Sobre

O objetivo deste projeto é escrever um analisador sintático capaz de analisar programas na linguagem LA (Linguagem Algorítmica) desenvolvida pelo prof. Jander, no âmbito do DC/UFSCar. A partir de um código fonte, o analisador detecta erros sintáticos, indicando a linha e o motivo de determinada falha sintática.

Os principais arquivos responsáveis pela conclusão do projeto são:

AlgumaLexer.g4 - contém as regras para a gramática da linguagem LA, como identificadores, constantes, operações e parâmetros, assim como a definição de início e fim de comentários, início e fim do próprio programa, e erros possíveis que podem ser encontrados, como CADEIA_NAO_FECHADA, COMENTARIO_NAO_FECHADO e SIMBOLO_NAO_IDENTIFICADO.

Principal.java - contém a função principal do código que lê os arquivos de entrada e gera os arquivos de saída contendo as mensagens de erro para cada programa analisado.

MyCustomErrorListener.java - gera a mensagem de erro ocorrido no código, indicando a linha e o motivo da falha sintática em questão, e interrompe a execução do programa.

## Pré-Requisitos

- Java 11
- ANTLR 4.11.1
- Maven 4.0.0

## Instalação de Dependências

Instalar JDK 11.0.18 de alguma fonte.

## Execução do programa

Use este comando para compilar o .jar do programa
```
mvn package
```

Para executar o programa .jar use
```
java -jar \caminho-do-diretorio\alguma-lexico\target\alguma-lexico-1.0-SNAPSHOT-jar-with-dependencies.jar \caminho_do_arquivo-de-entrada\entrada.txt \caminho_do_arquivo-de-saida\saida.txt
```

