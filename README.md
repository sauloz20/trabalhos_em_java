# Trabalhos em Java

Exercícios introdutórios de Java executados no terminal: contagem de 1 a 10 e verificações de idade, nota, maior número, paridade e sinal.

## Tecnologias e requisitos

- Java e biblioteca padrão (`Scanner`).
- JDK com `javac` e `java` disponíveis no terminal.
- Git para clonar o repositório.

## Executar

Clone o projeto e entre na pasta:

```sh
git clone https://github.com/sauloz20/trabalhos_em_java.git
cd trabalhos_em_java
```

Cada exercício é independente e usa o mesmo nome de classe. Compile um por vez em uma pasta de saída separada. Por exemplo:

```sh
javac -encoding UTF-8 -d build/idade src/idade/Mavenproject1.java
java -cp build/idade com.mycompany.mavenproject1.Mavenproject1
```

Troque `idade` pelo diretório desejado. Para `maior`, a classe não tem pacote; execute com `java -cp build/maior Mavenproject1`. Informe os dados solicitados no terminal.

## Estrutura

```text
src/
  contador/   Contagem de 1 a 10
  idade/      Classificação por idade
  nota/       Classificação de nota
  maior/      Comparação de dois números
  par-impar/  Verificação de paridade
  sinal/      Verificação de sinal
```

Os exercícios preservam seu comportamento original. Em `maior`, os dois `if` são independentes; por isso, quando o primeiro número é maior, a saída também informa que são iguais.
