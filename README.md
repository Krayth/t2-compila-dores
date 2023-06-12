# Trabalho 1 - Compiladores

## Alunos e RAs

- Bruno Matos de Souza - 769754
- Eduardo Minoru Takeda - 776857
- Fernando Eiji Hieda - 769768

## Sobre

O objetivo deste projeto é escrever um analisador léxico capaz de ler programas em forma de pseudocódigos de um arquivo texto e gerar outro arquivo de saída contendo os _tokens_ de cada termo presente da entrada de acordo com as regras de gramática especificadas.
Os principais arquivos responsáveis pela conclusão do projeto são:

AlgumaLexer.g4 - contém as regras para a gramática AlgumaLexer como PALAVRA-CHAVE, IDENT, CADEIA e regras para detecção de erros, por exemplo CADEIA-NAO-FECHADA, COMENTARIO-NAO-FECHADO.

Principal.java - contém a função principal do código que lê os arquivos de entrada e gera o arquivo de saída contendo os _tokens_ de cada termo presente e de possíveis erros.

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

