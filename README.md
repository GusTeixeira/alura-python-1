# RESUMO PYTHON: AULA BASICA

## Tipos de dados:

### Tipos Numéricos
- **int**: Inteiros, por exemplo, `5`, `-10`, `100`.
- **float**: Números de ponto flutuante, por exemplo, `3.14`, `-0.001`, `2.0`.

### Sequências
- **str**: Sequência de caracteres, por exemplo, `"hello"`, `'Python'`, `"123"`.
- **list**: Sequência mutável de itens, por exemplo, `[1, 2, 3]`, `['a', 'b', 'c']`.
- **tuple**: Sequência imutável de itens, por exemplo, `(1, 2, 3)`, `('a', 'b', 'c')`.

### Conjuntos
- **set**: Coleção não ordenada e mutável de itens únicos, por exemplo, `{1, 2, 3}`, `{'a', 'b', 'c'}`.
- **frozenset**: Conjunto imutável, por exemplo, `frozenset({1, 2, 3})`, `frozenset({'a', 'b', 'c'})`.

### Mapeamentos
- **dict**: Coleção mutável e indexada de pares chave-valor, por exemplo, `{'a': 1, 'b': 2, 'c': 3}`.

### Booleanos
- **bool**: Valores `True` (verdadeiro) ou `False` (falso).

### Tipos de Sequência Binária
- **bytes**: Sequência imutável de bytes, por exemplo, `b'hello'`.
- **bytearray**: Sequência mutável de bytes, por exemplo, `bytearray(b'hello')`.

### Tipos None
- **NoneType**: Tipo de dado especial que representa a ausência de valor, por exemplo, `None`.


# Listas de Dicionários em Python

As listas de dicionários em Python são estruturas de dados que permitem armazenar uma coleção ordenada de elementos, onde cada elemento é um dicionário.

## Estrutura

`
restaurantes = [
    {'nome': 'Praça', 'categoria': 'Japonesa', 'ativo': False}, 
    {'nome': 'Pizza Suprema', 'categoria': 'Pizza', 'ativo': True},
    {'nome': 'Cantina', 'categoria': 'Italiano', 'ativo': False}
]`

### Características
---------------

*   **Ordenação**: Os elementos são armazenados em ordem definida pela posição na lista.
    
*   **Acesso aos Elementos**: Os elementos podem ser acessados pelo índice da lista. Cada elemento é um dicionário, e os valores dentro do dicionário podem ser acessados por suas chaves.
    
*   **Flexibilidade**: Cada dicionário pode ter um conjunto diferente de chaves e valores, proporcionando flexibilidade na representação dos dados.
    
*   **Mutabilidade**: Os elementos da lista podem ser modificados, adicionados ou removidos conforme necessário.

## DOCSTRINGS

A docstring em Python é uma forma de documentar as funções, fornecendo informações sobre a função, seus inputs e outputs. Ela é uma prática recomendada para facilitar o entendimento e o uso do código, tanto para outras pessoas quanto para nós mesmos no futuro. A docstring pode conter uma breve descrição da função, especificação dos inputs necessários e até mesmo o output esperado. Ela é útil para documentar o código e auxiliar no entendimento das funções, principalmente quando outras pessoas vão utilizar o nosso código ou quando precisamos nos lembrar de como utilizar uma função no futuro.

```

def calcular_media(notas):
    '''
    Função responsável por calcular a média de um conjunto de notas.

    Args:
        notas (list): Uma lista contendo as notas dos alunos.

    Returns:
        float: A média das notas.

    Raises:
        ValueError: Se a lista de notas estiver vazia.

    Exemplo de uso:
        notas = [7.5, 8.0, 6.5, 9.0]
        media = calcular_media(notas)
        print(media)  # Saída: 7.75
    '''
    if len(notas) == 0:
        raise ValueError("A lista de notas não pode estar vazia.")

    soma = sum(notas)
    media = soma / len(notas)
    return media

```