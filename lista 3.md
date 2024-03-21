# UNIFOR
**Nome**: Allan Justo

**professor**: Carubbi

**Disciplina**: Raciocínio lógico algorítmico
### Exercício 01 
Atualize o algoritmo para determinar se um número inteiro e positivo é par ou ímpar, usando uma laço condicional para aceitar apenas números maiores ou iguais a zero. 

#### Fluxograma
```mermaid
flowchart TD
A([inicio])--> 
   Entrada(Entrada)
    Entrada --> Verifica_Positivo{numero >= 0}
    Verifica_Positivo -->|Sim| Verifica_Par_Impar{numero % 2 == 0}
    Verifica_Positivo -->|Não| Nova_Entrada[Digite um número inteiro e positivo]
    Nova_Entrada --> Entrada
    Verifica_Par_Impar -->|Sim| Par[O número é par]
    Verifica_Par_Impar -->|Não| Impar[O número é ímpar]
    Par --> Fim(Fim)
    Impar --> Fim
```

#### Pseudocódigo 
```
ALGORITMO CLASSIFICAR_CATEGORIA
Algoritmo Verifica_Par_Impar
    // Variáveis
    inteiro numero
    
    // Entrada
    Escreva("Digite um número inteiro e positivo: ")
    Leia(numero)
    
    // Verificação de número positivo
    Enquanto numero < 0
        Escreva("O número digitado não é positivo. Digite um número inteiro e positivo: ")
        Leia(numero)
    
    // Verificação de par ou ímpar
    Se numero % 2 = 0 Então
        Escreva("O número ", numero, " é par.")
    Senão
        Escreva("O número ", numero, " é ímpar.")
    FIM_ALGORITIMO

  #### Teste de mesa
```
nome_coluna1	nome_coluna2	nome_coluna3	nome_coluna4	nome_coluna5
Adicionar	espaço	se quiser	alinhar	como barras
verticais,	mas	não é	obrigatório.	Entendeu?
```

### Exercício 02

### Faça um algoritmo que exiba na tela uma contagem de 0 até 30, exibindo apenas os múltiplos de 3.
````
#### Fluxograma
```mermaid
flowchart TD
A([INICIO]) --> B{{Inicializar contador = 0}}
B--LOOP-->C[enquanto contador<=30]
 C--> D{Se contador % 3 == 0}
 D-->E[Verdadeiro] 
  D-->F[falso] 
E-->I(Exibir Contador)
I-->H([FIM])
F-->G[incrementar contador]
G--LOOP-->D
```
#### Pseudocódigo
```
ALGORITIMO_MULTIPLOS_DE_3
contador = 0  // Inicialize o contador

ENQUANTO contador <= 30 FAÇA
    SE contador % 3 == 0 ENTÃO
        EXIBIR contador  // Exibir apenas os múltiplos de 3
    FIM SE
    contador = contador + 1  // Incrementar o contador
FIM ENQUANTO

FIM_ALGORITIMO

````
#### Teste de mesa (0.5 ponto)

| nome_coluna1 | nome_coluna2 | nome_coluna3 | nome_coluna4 | nome_coluna5 | 
|      --      |      --      |      --      |      --      |      --      | 
| Adicione     | espaço       | se quiser    |  alinhar     | as barras    |
| verticais,   | mas          | não é        | obrigatório. | Entendido ?  |
```

### Exercício 03 
Dada uma sequência de números inteiros, calcular a sua soma. 
Por exemplo, para a sequência {12, 17, 4, -6, 8, 0}, o seu programa deve escrever o número 35.

#### Fluxograma 
```
#### Fluxograma
```mermaid
flowchart TD
A([INICIO]) --> definir_sequencia[Definir a sequência de números inteiros]
    definir_sequencia --> inicializar_soma[Inicializar soma = 0]
    inicializar_soma --> loop[Para cada número na sequência]
    loop --> adicionar_numero{Adicionar número à soma?}
    adicionar_numero --> |Sim| adicionar[Adicionar número à soma]
    adicionar_numero --> |Não| proximo_numero[Próximo número na sequência]
    adicionar --> atualizar_soma[Atualizar valor da soma]
    atualizar_soma --> proximo_numero
    proximo_numero --> verificar_fim{Todos os números verificados?}
    verificar_fim --> |Não| loop
    verificar_fim --> |Sim| exibir_soma[Exibir soma total]
    exibir_soma --> fim([FIM])
```

#### Pseudocódigo (1.0 ponto)
```
AlGORITIMO_SOMA_NÚMEROS_INTEIROS
// Definir a sequência de números inteiros
sequencia = {12, 17, 4, -6, 8, 0}
// Inicializar a variável para armazenar a soma
soma = 0
// Iterar sobre cada elemento da sequência
PARA cada número NA sequencia FAÇA
    // Adicionar o número à soma
    soma = soma + número
FIM PARA

// Exibir a soma total
EXIBIR soma
FIM_ALGORITMO
```
#### Teste de mesa

| nome_coluna1 | nome_coluna2 | nome_coluna3 | nome_coluna4 | nome_coluna5 | 
|      --      |      --      |      --      |      --      |      --      | 
| Adicione     | espaço       | se quiser    |  alinhar     | as barras    |
| verticais,   | mas          | não é        | obrigatório. | Entendido ?  |


### Exercício 04
Escreva um programa que leia a nota de diversos alunos, até que seja digitada uma nota negativa. 
Nesse momento, ele mostra a média aritmética de todas as notas lidas e quantas notas foram lidas. 
Ex. Foram lidas 14 notas. A média aritmética é 6.75!

#### Fluxograma 
```mermaid
flowchart TD
A([INICIO]) -->  ler_nota[Ler a primeira nota]
    ler_nota --> nota_negativa{Nota é negativa?}
    nota_negativa --> |Não| somar[Somar nota à soma total e contar o número de notas lidas]
    somar --> ler_nova_nota[Ler uma nova nota]
    ler_nova_nota --> nota_negativa
    nota_negativa --> |Sim| calcular_media[Calcular média aritmética]
    calcular_media --> exibir_resultado[Exibir o número de notas lidas e a média aritmética=6,75]
    exibir_resultado --> fim[FIM]
```

#### pseudocódigo
```
ALGORITIMO_VARIÁVEIS 
// Inicializar variáveis
soma_notas = 0
numero_notas = 0
// Ler a primeira nota
LER nota
ENQUANTO nota >= 0 FAÇA
    // Somar a nota à soma total
    soma_notas = soma_notas + nota
    // Contar o número de notas lidas
    numero_notas = numero_notas + 1
    // Ler a próxima nota
    LER nota
FIM ENQUANTO
// Calcular a média aritmética
SE numero_notas > 0 ENTAO
    media = soma_notas / numero_notas
    // Exibir o número de notas lidas e a média aritmética
    EXIBIR "Foram lidas ", numero_notas, " notas. A média aritmética é ", media, "!"
SENÃO
    // Se nenhum nota foi lida, exibir mensagem
    EXIBIR "Nenhuma nota foi lida!"
FIM_ENQUANTO
FIM
```

#### Teste de mesa 
| nome_coluna1 | nome_coluna2 | nome_coluna3 | nome_coluna4 | nome_coluna5 | 
|      --      |      --      |      --      |      --      |      --      | 
| Adicione     | espaço       | se quiser    |  alinhar     | as barras    |
| verticais,   | mas          | não é        | obrigatório. | Entendido ?  |
