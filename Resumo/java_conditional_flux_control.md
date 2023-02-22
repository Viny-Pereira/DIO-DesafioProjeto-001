# Lógica Condiciona e Controle de Fluxo em Java

- [Thiago Leite e Carvalho](https://www.linkedin.com/in/thiago-leite-e-carvalho-1b337b127/)

## Operadores Relacionais

- Simbolos especiais que realizam comparação e retornam um resultado.

- No mínimo 2 operandos

- Similaridade: `== !=` (Igualdade e diferença)
- Tamanho: `> < >= <= ` (maior, menor, maior ou igual, menor ou igual)

- Comparações de similidade são possiveis para todos os tipos.
- Numéricos podem ser comparados por tamanho e similaridade com outros numéricos.
- **boolean** só podem ser comparados por similaridade entre eles
- **Strigs** não podem ser comparadas por tamanho
- **char** podem ser comparados por tamanho

## Operadores lógicos

- Simbolos especiais que realizam comparações lógicas e retorna um resultado
- `&&` (Conjunção) -> Verdade V e V
- `||` (Disjunção) -> Falso F e F
- `^` (Dijunção exclusiva (xor)) -> Verdade quando o resultado das expresões são opostos: V e F ou F e V
- `!` (Negação)

## Controle de fluxo

- São estruturas capazes de direcionar o fluxo de execução do código

- Decisão

```
if(condicao){
    opcao1;
}else if (condicao2){
    opcao2;
}else if (condicao3){
    opcao3;
}else{
    ultimaopcao;
}
```

- Ternário
  `condicao ? <se true> : <se false>`

- Switch

```
switch(variavel){
    case1:
        break;
    case2:
        break;
    default:
        break;
}
```

### Boas práticas

- Se só uma variável usar `switch`
- Usar o default para indicar erros
- Evitar muitos if aninhados
- Usar variáveis intermediárias

## Blocos

- Um conjunto de códigos que trabalham em conjunto para executar um operação.
- Bloco são delimitados por `{}`
