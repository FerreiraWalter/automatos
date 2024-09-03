# Autômatos

## O que são Autômatos?

Autômatos são modelos matemáticos que representam máquinas de estados finitos. Eles são usados para modelar sistemas que possuem um número limitado de estados e que transitam entre esses estados com base em entradas externas. Autômatos são fundamentais na teoria da computação e são amplamente utilizados para descrever linguagens formais, reconhecedores de padrões e na construção de compiladores.

## Tipos de Autômatos

### 1. Autômato Finito Determinístico (DFA)

Um **Autômato Finito Determinístico** (DFA - *Deterministic Finite Automaton*) é um tipo de autômato onde, para cada estado e símbolo de entrada, existe uma única transição definida. Isso significa que, dado o estado atual e a entrada, o próximo estado é sempre previsível e único.

#### Características do DFA:
- **Determinístico**: Não há ambiguidades; para cada estado e entrada, há exatamente uma transição possível.
- **Simples**: A implementação de um DFA é direta, pois não há necessidade de considerar múltiplos caminhos.

#### Exemplo de uso:
- **Validação de uma senha**: Verificar se uma senha atende a certos critérios, como ter pelo menos uma letra maiúscula, uma minúscula, e um número.

### 2. Autômato Finito Não Determinístico (NFA)

Um **Autômato Finito Não Determinístico** (NFA - *Non-deterministic Finite Automaton*) é um tipo de autômato onde, para cada estado e símbolo de entrada, pode haver várias transições possíveis, incluindo transições que não consomem nenhum símbolo (transições-ε).

#### Características do NFA:
- **Não-determinístico**: Pode haver múltiplos caminhos possíveis para processar uma entrada.
- **Flexível**: Pode representar certas linguagens de maneira mais compacta que um DFA.
- **Conversão**: Qualquer NFA pode ser convertido em um DFA equivalente, embora o DFA resultante possa ter um número exponencialmente maior de estados.

#### Exemplo de uso:
- **Reconhecimento de padrões em textos**: Buscar todas as ocorrências de uma palavra em um texto, considerando possíveis variações.

## Comparação entre DFA e NFA

| **Características** | **DFA** | **NFA** |
|---------------------|---------|---------|
| Transições          | Única transição por estado e símbolo | Múltiplas transições possíveis |
| Eficiência          | Mais rápido, pois segue um único caminho | Pode ser mais lento devido à necessidade de explorar múltiplos caminhos |
| Complexidade        | Simples de implementar e entender | Mais flexível, mas pode ser mais complexo |

## Conclusão

Autômatos, sejam eles determinísticos ou não determinísticos, são ferramentas poderosas na teoria da computação e têm aplicações práticas em muitas áreas, como linguagens formais, processamento de texto, e design de sistemas. Entender as diferenças entre DFA e NFA é essencial para escolher a abordagem correta para um problema específico.

- site para testes: https://ivanzuzak.info/noam/webapps/fsm_simulator/
