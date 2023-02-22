# Aprendendo a Sintaxe do Java

- [Resumo do môdulo](https://glysns.gitbook.io/java-basico/)
- [Arquivos desenvolvidos durante as aulas](https://github.com/Viny-Pereira/DIO-Aulas/tree/main/Sintaxe)

## Pontos base

- Nome do arquivo: O inicio de cada palavra deve ser com letra maiuscula -> NumerosPrimos.java
- Nome da classe principal deve ter o mesmo nome do arquivo -> NumerosPrimos
- Nome de variável deve iniciar com minuscula e se composta as demais maiuscula -> numeroPrimo
- Variavel que não deve ser mudada deve ser completamente maiuscula -> ESTADOS_BRASILEIROS = 27 ou usar o `final`
- Variavel pode conter: Números, \_, $ e Letras.

### Condições base Arquivo: MinhaClasse.java

```
public class MinhaClasse {
  public static void main (String [] args){
    System.out.print(s:"Hello World");
  }
}
```

### Declaração variável

- Tipo nomeVariavel = Atribuição(Nem sempre é preciso)
- Tipo: String, int, booLean(true e false)

### Identação

- Formas de hierparquisar o código por meio de tabulação
- A identação no Java não é obrigatória, porém auxilia na leitura do código.

### Organização de Arquivos

- Criação de subdiretórios para organização e controle mais adequado no desenvolvimento do projeto
- Se utiliza um prefixo anterior ao nome da empresa -> com.empresaX.projeto01
  - Comercial (com); Opensource (or); Organizacional (org)

### Java Beans

- Convenção de escrita da comunidade de desenvolvimento java

#### Convenções

- Variável deve ser clara, sem abreviações ou definições sem sentido
- Variavel deve ser no singular com excessao de array ou coleção
- Trabalhe o arquivo em um só idioma
- Metodo deve ser nomeado como verbo -> `somar(){}`, `abrirConexao(){}`

## Tipos de Variáveis

- Tipos premitivos: tipos de dados básicos usados para criação dos demais programas:

  - byte(1byte), short(2byte), int(4byte), long(8byte \_ usar L no final do número para forçar o uso do tipo) -> Normalmente utiliza-se o `int`
  - float(4bytes \_ usar F no final para forçar usar o tipo), double(8bytes) -> Normalmente utiliza-se o `double` devido a maior precisão
  - boolean (true/false)
  - char (uma única letra)

- Casting: Forçar uma variável a ser de determinado tipo de menor tamanho

```
short numeroCurto = 1;
int numeroNormal = numeroCurto;
short numeroCurto2 = (short) numeroNormal; // casting
```

## Constante

- Valores que não poderão ser modificados
- Deve estar em caixa alta
- usar palavra reservada `final`
  `final double VALOR_PI = 3.14`

## Operadores

- Simbolos especiais que tem significado para linguagem e realizam determinada operação

  - Atribuição `=`
  - Aritmético `+ - * /`
  - Unário `+(positivo) -(negativo) ++(incremento) --(decremento) !(negação)`
  - Ternario `<condição> ? <caso verdadeiro> : <caso falso>`
  - Relacionais `== != > < >= <=`
  - Logicos `&&(e) ||(ou)`

## Métodos

- São funcoes/subrotinas
- Convenções da comunidade
  - nomeado como verbo
  - Padrão camelCase
- Se o metodo não possuir uma saida deve ser precedido por `void`

## Escopo

- Ambiente onde uma variável pode ser acessada
- Parâmetros de métodos são variáveis locais primordialmente existindo apenas dentro do método;
- Variáveis de classe podem ser usadas dentro de toda a classe.

## Palavras Reservadas

- Indentificadores de uma linguagem, que não podem ser usadas para nomear variáveis, classes, métodos ou atributos.
- São 52 palavras contidas nesse [link](https://glysns.gitbook.io/java-basico/sintaxe/palavras-reservadas)

## Java Doc

- [Documentação Java SE](https://docs.oracle.com/javase/7/docs/api/java/lang/String.html)

- Tags: palavra reservada no codigo que passam alguma informação

- Comentário:

  - Uma linha `//`
  - Multiplas linhas `/* */`
  - Documentação `/** */`

- Javadoc - gerador de documentação a partir do codigo fonte.

  - Comando javadoc em HTML
    `javadoc -encoding UTF-8 -docencoding ISO-8859-1  -d ../docs  src/*.java`

## Terminal

- Muitas vezes é necessário criar um executável, para que os usuários possam utilizar o projeto de maneira simplificada.
- Excução via terminal
  - Compilar `javac NomeProjeto.java`
  - Executar`java NomeProjeto`

## Argumentos

- Podemos usar argumentos no formato de String para usar como logica na execução
  - Arquivo: meuProjeto
    `java meuProjeto <arg[1]> <args[2]> ... <args[n]>`
- class `Scanner` faz a leitura de parametros pos execução
