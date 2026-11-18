# Trabalhos em Java

![Java](https://img.shields.io/badge/linguagem-Java-blue)

Exercícios introdutórios de Java para terminal: contagem, idade, nota, comparação de números, paridade e sinal. Cada arquivo contém um exercício independente.

## Tecnologias e requisitos

Java, biblioteca padrão e um JDK com `javac` e `java`. Os arquivos originais não têm extensão e reutilizam o nome de classe `Mavenproject1`.

## Executar

Clone o repositório e, no PowerShell, prepare uma cópia de um exercício por vez:

```powershell
git clone https://github.com/sauloz20/trabalhos_em_java.git
cd trabalhos_em_java
Copy-Item 'verificação de idade' Mavenproject1.java
javac -encoding UTF-8 -d build/idade Mavenproject1.java
java -cp build/idade com.mycompany.mavenproject1.Mavenproject1
```

Para testar outro exercício, substitua o arquivo copiado pelo exercício desejado e compile em outra pasta de saída. O exercício `verificação de numero maior` não declara pacote: nesse caso, execute `java -cp build/maior Mavenproject1`. Como todos usam a mesma classe pública, compile-os separadamente.

## Estrutura

Os seis arquivos de exercícios estão na raiz: contador, idade, nota, maior número, paridade e sinal. O [PR de organização](https://github.com/sauloz20/trabalhos_em_java/pull/1) propõe organizá-los em `src/`.

## Limitação conhecida

No exercício de comparação, os dois `if` são independentes: quando o primeiro número é maior, o programa também exibe a mensagem de igualdade. Este README descreve o comportamento existente.
