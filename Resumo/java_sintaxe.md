# Aprendendo a Sintaxe do Java

- [Resumo do môdulo](https://glysns.gitbook.io/java-basico/)

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
