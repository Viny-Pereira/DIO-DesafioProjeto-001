# Estruturas de dados em java

- [João Ricardo Côre Dutra](https://www.linkedin.com/in/jo%C3%A3o-dutra-400a9330/)
- [Slides](https://github.com/jrdutra/estruturaDeDadosJavaDio/tree/main/apresentacoes)
- [Repositório](https://github.com/jrdutra/estruturaDeDadosJavaDio)

## 1. Introdução

- Memória primária(ROM - HD) / Memória secundária(RAM)
- Atribuição de objetos fazem referencia ao local da memória dessa forma mudanças nos objetos variáveis tem efeito em cascata.

### Nó

- Armazena o dado e a referência de outro nó
- Encadeamento: os nós são refrenciados aos próximos e o ultimo referencia `null`

### Generrics

- Determina o tipo de dados que o objeto recebe.

```
Lista<String> minhaLista = new Lista<>()

public class Lista<T>{
    private T t;
}
```

- Unknown Wildcard: Genérioco

```
public void imprimeLista(List<?>lista){
    for(Object obj : lista){
        Syste,.out.println(obj);
    }
}

List<Aluno>minhaLista = new List<Aluno>();
imprimeLista(minhaLista);
```

- UpperBounded Wildcard: Aceita qualquer filho do objeto pessoa

```
public void imprimeLista(List<? extends Pessoa>listaPessoas){
    for(Pessoa p : listaPessoas){
        Syste,.out.println(p);
    }
}

List<Aluno>minhaLista = new List<Aluno>();
imprimeLista(minhaLista);
```

- LowerBounded Wildcard: Só aceita objetos pais a pessoa

```
public void imprimeLista(List<? super Pessoa>listaPessoas){
    for(Pessoa p : listaPessoas){
        Syste,.out.println(p);
    }
}

List<Aluno>minhaLista = new List<Aluno>();
imprimeLista(minhaLista);
```

#### Convenções

- **K** -> Key
- **V** -> Value
- **E** -> Element
- **T** -> Type
- **?** -> Generic

## 2. Pilhas

- Last In First Out (LIFO) - O primeiro a entrar é o ultimo a sair
- Metódo Top (Verifica a informação do superior) `.top`
- Método Pop (Receber o dado e tirar o nó) `.pop`
- Metodo push (inserir o nó)
- `isEmpty()`

## 3. Filas

- First In Firt Out (FIFO) - Primeiro entrar primeiro a sair
- A informação do nó é um objeto

- `enqueue()` adiciona um nó no final da fila
- `dequeue()` elimina o primeiro elemento da fila
- `isEmpty()`

## 4. Listas encadeadas

- `add(n)` adiciona um nó na posição n da fila
- `remove(n)` elimina o elemento n da fila
- `get(n)` pega a informação do nó n
- `isEmpty()`

## 5. Listas Duplamente Encadeadas

## 6. Listas Circulares

## 7. Arvores

## 8. Principais implementações das estruturas de dados do Java
