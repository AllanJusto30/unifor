# UNIFOR
**Nome**: Allan Justo de Freitas 

**professor**: Carubbi

**Disciplina**: Raciocínio lógico algorítm

## Lista de exercícios 01

### Exercício 01 
Calcule a média de quatro números inteiros dados.

#### Fluxograma 
```mermaid
flowchart TD
A([INICIO]) --> B{{Digite o primeiro número inteiro}}
    B --> C[Digite o segundo número inteiro]
    C --> D[Digite o terceiro número inteiro]
    D --> E[Digite o quarto número inteiro]
    E --> F{Calcular média}
    F --> G[Exibir média]
    G --> H([FIM_ALGORITMO])
```

#### Pseudocódigo
```
ALGORITMO Calcular_Media
DECLARE num1, num2, num3, num4, media NUMÉRICO

ESCREVA "Digite o primeiro número inteiro:"
LEIA num1

ESCREVA "Digite o segundo número inteiro:"
LEIA num2

ESCREVA "Digite o terceiro número inteiro:"
LEIA num3

ESCREVA "Digite o quarto número inteiro:"
LEIA num4

media = (num1 + num2 + num3 + num4) / 4

ESCREVA "A média dos quatro números é:", media
FIM_ALGORITMO
```

#### Teste de mesa

| nome_coluna1 | nome_coluna2 | nome_coluna3 | nome_coluna4 | nome_coluna5 | 
|      --      |      --      |      --      |      --      |      --      | 
| Adicione     | espaço       | se quiser    |  alinhar     | as barras    |
| verticais,   | mas          | não é        | obrigatório. | Entendido ?  |

### Exercício 02 
Leia uma temperatura dada em Celsius (C) e imprima o equivalente em Fahrenheit (F). (Fórmula de conversão: F = (9/5) * C + 32)

#### Fluxograma
```mermaid
flowchart TD
A([INICIO]) --> B{{digite a temperatura em Celsius }}
B --> C{Temperatura em Celsius}
C -- Sim --> D{{Calcular Fahrenheit F = 9/5 * C + 32}}
D --> E[Exibir temperatura em Fahrenheit]
E --> F([FIM])
C -- Não --> G[Exibir mensagem de erro] 
G --> F
```

#### Pseudocódigo 
ALGORITMO_Celsius_Fahrenheit 
DECLARE Celsius, Fahrenheit NUMÉRICO


ESCREVA "Insira a temperatura em graus Celsius:"
Leia em Celsius

Fahrenheit = (9/5) * Celsius + 32

Escreva "A temperatura Fahrenheit (F) é" em graus Fahrenheit.
FIM_ALGORITMO
```
Algoritmo ConverteCelsiusFarenheit:
```
#### Teste de mesa 

| nome_coluna1 | nome_coluna2 | nome_coluna3 | nome_coluna4 | nome_coluna5 | 
|      --      |      --      |      --      |      --      |      --      | 
| Adicione     | espaço       | se quiser    |  alinhar     | as barras    |
| verticais,   | mas          | não é        | obrigatório. | Entendido ?  |

### Exercício 03 
Receba dois números reais e um operador e efetue a operação correspondente com os valores recebidos (operandos). 
O algoritmo deve retornar o resultado da operação selecionada simulando todas as operações de uma calculadora simples.

#### Fluxograma 








