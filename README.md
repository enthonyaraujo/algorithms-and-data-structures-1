# Algoritmos e Estruturas de Dados I

Material de estudo da disciplina **Algoritmos e Estruturas de Dados I**, com foco na linguagem C. Este documento reúne o cronograma, os conceitos fundamentais, exemplos completos e as principais operações das estruturas estudadas durante o semestre.

## Sumário

* [Objetivos](#objetivos)
* [Organização do conteúdo](#organização-do-conteúdo)
* [1. Introdução à disciplina](#1-introdução-à-disciplina)

  * [Por que estudar estruturas de dados?](#por-que-estudar-estruturas-de-dados)
* [2. Ponteiros](#2-ponteiros)

  * [2.1 Conceito](#21-conceito)
  * [2.2 Operadores fundamentais](#22-operadores-fundamentais)
  * [2.3 Exemplo completo](#23-exemplo-completo)
  * [2.4 Ponteiro nulo](#24-ponteiro-nulo)
  * [2.5 Ponteiros e funções](#25-ponteiros-e-funções)
  * [2.6 Ponteiros e vetores](#26-ponteiros-e-vetores)
  * [2.7 Aritmética de ponteiros](#27-aritmética-de-ponteiros)
  * [2.8 Ponteiros e strings](#28-ponteiros-e-strings)
  * [2.9 Ponteiros para estruturas](#29-ponteiros-para-estruturas)
  * [2.10 Ponteiro para ponteiro](#210-ponteiro-para-ponteiro)
* [3. Alocação dinâmica de memória](#3-alocação-dinâmica-de-memória)

  * [3.1 Memória automática e memória dinâmica](#31-memória-automática-e-memória-dinâmica)
  * [3.2 Funções principais](#32-funções-principais)
  * [3.3 Vetor dinâmico completo](#33-vetor-dinâmico-completo)
  * [3.4 Redimensionamento com realloc](#34-redimensionamento-com-realloc)
  * [3.5 Matrizes dinâmicas](#35-matrizes-dinâmicas)
  * [3.6 Erros comuns](#36-erros-comuns)
* [4. Tipos estruturados](#4-tipos-estruturados)

  * [4.1 Registros com struct](#41-registros-com-struct)
  * [4.2 Estruturas aninhadas](#42-estruturas-aninhadas)
  * [4.3 Vetores de estruturas](#43-vetores-de-estruturas)
  * [4.4 Estruturas dinâmicas](#44-estruturas-dinâmicas)
  * [4.5 Uniões](#45-uniões)
  * [4.6 Enumerações](#46-enumerações)
* [5. Manipulação de arquivos](#5-manipulação-de-arquivos)

  * [5.1 Conceito](#51-conceito)
  * [5.2 Arquivos de texto e binários](#52-arquivos-de-texto-e-binários)
  * [5.3 Modos de abertura](#53-modos-de-abertura)
  * [5.4 Funções para arquivos de texto](#54-funções-para-arquivos-de-texto)
  * [5.5 Funções para arquivos binários](#55-funções-para-arquivos-binários)
  * [5.6 Exemplo completo: texto e binário](#56-exemplo-completo-texto-e-binário)
* [6. Complexidade de algoritmos](#6-complexidade-de-algoritmos)

  * [6.1 Objetivo](#61-objetivo)
  * [6.2 Complexidade de tempo e espaço](#62-complexidade-de-tempo-e-espaço)
  * [6.3 Casos de análise](#63-casos-de-análise)
  * [6.4 Notações assintóticas](#64-notações-assintóticas)
  * [6.5 Ordens de crescimento comuns](#65-ordens-de-crescimento-comuns)
  * [6.6 Regras práticas](#66-regras-práticas)
* [7. Tipos Abstratos de Dados](#7-tipos-abstratos-de-dados)

  * [7.1 Interface e implementação](#71-interface-e-implementação)
  * [7.2 Vantagens](#72-vantagens)
* [8. Algoritmos de busca](#8-algoritmos-de-busca)

  * [8.1 Busca sequencial](#81-busca-sequencial)
  * [8.2 Busca binária](#82-busca-binária)
  * [8.3 Exemplo completo](#83-exemplo-completo)
  * [8.4 Comparação](#84-comparação)
* [9. Listas encadeadas](#9-listas-encadeadas)

  * [9.1 Conceito](#91-conceito)
  * [9.2 Tipos de lista](#92-tipos-de-lista)

    * [Lista simplesmente encadeada](#lista-simplesmente-encadeada)
    * [Lista duplamente encadeada](#lista-duplamente-encadeada)
    * [Lista circular](#lista-circular)
    * [Lista de tipos estruturados](#lista-de-tipos-estruturados)
  * [9.3 Operações principais](#93-operações-principais)
  * [9.4 Exemplo completo](#94-exemplo-completo)
  * [9.5 Complexidade típica](#95-complexidade-típica)
* [10. Filas](#10-filas)

  * [10.1 Conceito](#101-conceito)
  * [10.2 Tipos de fila](#102-tipos-de-fila)
  * [10.3 Aplicações](#103-aplicações)
  * [10.4 Exemplo completo com lista encadeada](#104-exemplo-completo-com-lista-encadeada)
* [11. Pilhas](#11-pilhas)

  * [11.1 Conceito](#111-conceito)
  * [11.2 Aplicações](#112-aplicações)
  * [11.3 Exemplo completo com lista encadeada](#113-exemplo-completo-com-lista-encadeada)
* [12. Comparações importantes](#12-comparações-importantes)

  * [12.1 Vetor e lista encadeada](#121-vetor-e-lista-encadeada)
  * [12.2 Pilha e fila](#122-pilha-e-fila)
  * [12.3 Complexidade resumida](#123-complexidade-resumida)
* [13. Compilação dos exemplos](#13-compilação-dos-exemplos)
* [14. Boas práticas](#14-boas-práticas)
* [Licença e finalidade](#licença-e-finalidade)


## Objetivos

A disciplina apresenta técnicas para organizar, armazenar, acessar e processar dados de forma eficiente. Ao final do conteúdo, espera-se que o estudante seja capaz de:

- compreender endereços de memória e utilizar ponteiros;
- alocar e liberar memória durante a execução do programa;
- criar tipos estruturados para representar dados complexos;
- ler, escrever e atualizar arquivos de texto e arquivos binários;
- analisar o custo de execução de algoritmos;
- implementar algoritmos de busca;
- compreender o conceito de Tipo Abstrato de Dados;
- implementar listas encadeadas, pilhas e filas.

## Organização do conteúdo

| Unidade | Conteúdos principais |  |
|---|---|---|
| 1ª Unidade | Ponteiros, alocação dinâmica, tipos estruturados e manipulação de arquivos | 
| 2ª Unidade | Complexidade de algoritmos, algoritmos de busca e Tipos Abstratos de Dados | 
| 3ª Unidade | Listas encadeadas, filas e pilhas | 

# 1. Introdução à disciplina

Uma **estrutura de dados** define como um conjunto de informações será organizado na memória e quais operações poderão ser executadas sobre ele. A escolha da estrutura correta influencia diretamente a clareza do código, o consumo de memória e o tempo de execução do programa.

Exemplos de decisões importantes:

- usar um vetor quando é necessário acesso direto por índice;
- usar uma lista encadeada quando o tamanho varia durante a execução;
- usar uma pilha quando o último elemento inserido deve sair primeiro;
- usar uma fila quando os elementos devem ser atendidos por ordem de chegada;
- usar busca binária quando os dados estão ordenados e é necessário reduzir o número de comparações.

## Por que estudar estruturas de dados?

- **Eficiência:** permite resolver problemas utilizando menos tempo e memória.
- **Organização:** facilita a representação de dados complexos.
- **Reutilização:** estruturas podem ser transformadas em módulos independentes.
- **Base para outras áreas:** sistemas operacionais, bancos de dados, compiladores, redes, inteligência artificial e desenvolvimento de jogos utilizam estruturas de dados.

---

# 2. Ponteiros

## 2.1 Conceito

Um **ponteiro** é uma variável que armazena o endereço de memória de outra variável. Em C, o tipo do ponteiro indica o tipo de dado armazenado no endereço apontado.

```c
int numero = 10;
int *ponteiro = &numero;
```

Nesse exemplo:

- `numero` armazena o valor `10`;
- `&numero` representa o endereço de `numero`;
- `ponteiro` armazena esse endereço;
- `*ponteiro` acessa o valor presente no endereço apontado.

## 2.2 Operadores fundamentais

| Operador | Nome | Função |
|---|---|---|
| `&` | Operador de endereço | Obtém o endereço de uma variável |
| `*` | Operador de indireção | Acessa ou altera o valor apontado |

## 2.3 Exemplo completo

```c
#include <stdio.h>

void dobrar(int *valor) {
    if (valor != NULL) {
        *valor = *valor * 2;
    }
}

int main(void) {
    int numero = 15;
    int *ponteiro = &numero;

    printf("Valor de numero: %d\n", numero);
    printf("Endereco de numero: %p\n", (void *)&numero);
    printf("Endereco armazenado no ponteiro: %p\n", (void *)ponteiro);
    printf("Valor acessado pelo ponteiro: %d\n", *ponteiro);

    *ponteiro = 20;
    dobrar(&numero);

    printf("Valor final: %d\n", numero);
    return 0;
}
```

## 2.4 Ponteiro nulo

Um ponteiro que não aponta para uma região válida deve receber `NULL`.

```c
int *ponteiro = NULL;
```

Antes de acessar `*ponteiro`, é necessário verificar se o endereço é válido:

```c
if (ponteiro != NULL) {
    printf("%d\n", *ponteiro);
}
```

Desreferenciar um ponteiro nulo causa comportamento indefinido e normalmente encerra o programa.

## 2.5 Ponteiros e funções

Ponteiros podem ser utilizados como parâmetros para:

- modificar variáveis da função chamadora;
- evitar cópias de estruturas grandes;
- devolver mais de um resultado;
- manipular vetores e estruturas dinâmicas.

```c
void trocar(int *a, int *b) {
    int temporario = *a;
    *a = *b;
    *b = temporario;
}
```

## 2.6 Ponteiros e vetores

O nome de um vetor geralmente é convertido no endereço de seu primeiro elemento.

```c
int valores[3] = {10, 20, 30};
int *p = valores;

printf("%d\n", p[0]);
printf("%d\n", *(p + 1));
```

As expressões `p[i]` e `*(p + i)` são equivalentes.

## 2.7 Aritmética de ponteiros

Ao somar `1` a um ponteiro, o endereço avança o número de bytes correspondente ao tipo apontado.

```c
int valores[] = {5, 10, 15};
int *p = valores;

printf("%d\n", *p);       // 5
printf("%d\n", *(p + 1)); // 10
```

A aritmética deve permanecer dentro dos limites do mesmo vetor. Acessar posições externas provoca comportamento indefinido.

## 2.8 Ponteiros e strings

Strings em C são vetores de caracteres terminados por `\0`.

```c
char nome[] = "UFERSA";
char *p = nome;

printf("%s\n", p);
```

Uma literal de string não deve ser modificada. Para indicar essa restrição, utiliza-se `const`:

```c
const char *mensagem = "Algoritmos";
```

## 2.9 Ponteiros para estruturas

Campos de uma variável `struct` são acessados com `.`, enquanto campos acessados por um ponteiro são acessados com `->`.

```c
struct Aluno {
    char nome[50];
    float media;
};

struct Aluno aluno = {"Ana", 8.5f};
struct Aluno *p = &aluno;

printf("%s: %.1f\n", p->nome, p->media);
```

## 2.10 Ponteiro para ponteiro

Um ponteiro também possui endereço. Um ponteiro para ponteiro é declarado com dois asteriscos:

```c
int valor = 7;
int *p = &valor;
int **pp = &p;

printf("%d\n", **pp);
```

Esse recurso aparece em matrizes dinâmicas, alteração de ponteiros dentro de funções e estruturas encadeadas.

---

# 3. Alocação dinâmica de memória

## 3.1 Memória automática e memória dinâmica

A memória automática é reservada ao entrar em um bloco e liberada ao sair dele:

```c
int valor = 10;
```

A memória dinâmica é solicitada durante a execução e permanece alocada até que seja liberada explicitamente. Ela é útil quando o tamanho necessário só é conhecido em tempo de execução.

## 3.2 Funções principais

As funções estão declaradas em `<stdlib.h>`.

| Função | Finalidade |
|---|---|
| `malloc` | Reserva uma quantidade de bytes sem inicializar o conteúdo |
| `calloc` | Reserva memória para vários elementos e inicializa os bytes com zero |
| `realloc` | Altera o tamanho de uma área previamente alocada |
| `free` | Libera uma área de memória dinâmica |

## 3.3 Vetor dinâmico completo

```c
#include <stdio.h>
#include <stdlib.h>

int main(void) {
    size_t quantidade;

    printf("Quantidade de valores: ");
    if (scanf("%zu", &quantidade) != 1 || quantidade == 0) {
        fprintf(stderr, "Quantidade invalida.\n");
        return 1;
    }

    double *valores = malloc(quantidade * sizeof *valores);
    if (valores == NULL) {
        fprintf(stderr, "Falha ao alocar memoria.\n");
        return 1;
    }

    double soma = 0.0;

    for (size_t i = 0; i < quantidade; i++) {
        printf("Valor %zu: ", i + 1);
        if (scanf("%lf", &valores[i]) != 1) {
            fprintf(stderr, "Entrada invalida.\n");
            free(valores);
            return 1;
        }
        soma += valores[i];
    }

    printf("Media: %.2f\n", soma / quantidade);

    free(valores);
    valores = NULL;
    return 0;
}
```

## 3.4 Redimensionamento com `realloc`

```c
int *temporario = realloc(vetor, novo_tamanho * sizeof *vetor);

if (temporario == NULL) {
    // O ponteiro original continua valido.
    free(vetor);
    return 1;
}

vetor = temporario;
```

É recomendável armazenar o resultado de `realloc` em um ponteiro temporário para não perder o endereço original em caso de falha.

## 3.5 Matrizes dinâmicas

Uma matriz pode ser alocada como um vetor único e contínuo:

```c
int *matriz = malloc(linhas * colunas * sizeof *matriz);

// Acesso ao elemento da linha i e coluna j:
matriz[i * colunas + j] = 10;
```

Também é possível utilizar um ponteiro para ponteiro, alocando um vetor de linhas e depois cada linha separadamente. Nesse caso, todas as linhas e o vetor principal precisam ser liberados.

## 3.6 Erros comuns

- **Vazamento de memória:** perder o endereço de uma área alocada sem executar `free`.
- **Ponteiro pendente:** continuar utilizando um endereço depois de `free`.
- **Liberação dupla:** executar `free` duas vezes para a mesma área.
- **Acesso fora dos limites:** utilizar índices inválidos.
- **Falha não verificada:** acessar o resultado de `malloc`, `calloc` ou `realloc` sem verificar `NULL`.

Regra prática: toda alocação deve possuir uma liberação correspondente.

---

# 4. Tipos estruturados

## 4.1 Registros com `struct`

Uma estrutura agrupa valores de tipos diferentes sob um único nome.

```c
struct Produto {
    int codigo;
    char nome[80];
    double preco;
};
```

É possível criar um apelido de tipo com `typedef`:

```c
typedef struct {
    int codigo;
    char nome[80];
    double preco;
} Produto;
```

## 4.2 Estruturas aninhadas

Uma estrutura pode conter outra estrutura:

```c
typedef struct {
    int dia;
    int mes;
    int ano;
} Data;

typedef struct {
    char nome[80];
    Data nascimento;
} Pessoa;
```

## 4.3 Vetores de estruturas

```c
Produto estoque[100];
```

Essa organização é apropriada quando vários elementos compartilham o mesmo formato.

## 4.4 Estruturas dinâmicas

```c
Produto *estoque = malloc(quantidade * sizeof *estoque);

if (estoque == NULL) {
    return 1;
}

free(estoque);
```

Estruturas dinâmicas servem de base para listas, filas, pilhas, árvores e grafos.

## 4.5 Uniões

Em uma `union`, todos os campos compartilham a mesma região de memória. Apenas um valor deve ser considerado ativo por vez.

```c
union Dado {
    int inteiro;
    float real;
    char caractere;
};
```

Uniões economizam memória, mas exigem controle sobre qual campo está válido.

## 4.6 Enumerações

Uma enumeração cria nomes para valores inteiros, tornando o código mais legível.

```c
typedef enum {
    PENDENTE,
    EM_EXECUCAO,
    CONCLUIDO
} Estado;
```

---

# 5. Manipulação de arquivos

## 5.1 Conceito

Arquivos permitem manter dados mesmo depois do encerramento do programa. Em C, um arquivo é manipulado por meio de um ponteiro do tipo `FILE *`, declarado em `<stdio.h>`.

Fluxo básico:

1. abrir o arquivo com `fopen`;
2. verificar se a abertura foi bem-sucedida;
3. ler ou escrever os dados;
4. fechar o arquivo com `fclose`.

```c
FILE *arquivo = fopen("dados.txt", "r");

if (arquivo == NULL) {
    perror("Nao foi possivel abrir o arquivo");
    return 1;
}

fclose(arquivo);
```

## 5.2 Arquivos de texto e binários

| Característica | Arquivo de texto | Arquivo binário |
|---|---|---|
| Representação | Caracteres codificados | Dados em representação binária |
| Leitura humana | Pode ser aberto em editor de texto | Normalmente não é legível diretamente |
| Portabilidade | Geralmente maior | Pode depender da arquitetura e do compilador |
| Precisão numérica | Depende da conversão para texto | Preserva a representação armazenada |
| Funções comuns | `fprintf`, `fscanf`, `fgets`, `fgetc` | `fwrite`, `fread` |

## 5.3 Modos de abertura

| Modo | Descrição |
|---|---|
| `r` | Leitura; o arquivo precisa existir |
| `w` | Escrita; cria ou apaga o conteúdo existente |
| `a` | Adição ao final; preserva o conteúdo existente |
| `r+` | Leitura e escrita; o arquivo precisa existir |
| `w+` | Leitura e escrita; cria ou apaga o arquivo |
| `a+` | Leitura e adição ao final |
| `rb`, `wb`, `ab` | Equivalentes para arquivos binários |
| `rb+`, `wb+`, `ab+` | Leitura e escrita binária |

## 5.4 Funções para arquivos de texto

| Função | Uso |
|---|---|
| `fputc` | Escreve um caractere |
| `fputs` | Escreve uma string |
| `fprintf` | Escreve dados formatados |
| `fgetc` | Lê um caractere |
| `fgets` | Lê uma linha ou quantidade limitada de caracteres |
| `fscanf` | Lê dados formatados |

## 5.5 Funções para arquivos binários

| Função | Uso |
|---|---|
| `fwrite` | Escreve blocos de dados |
| `fread` | Lê blocos de dados |
| `fseek` | Move o indicador de posição |
| `ftell` | Retorna a posição atual |
| `rewind` | Retorna ao início do arquivo |

Constantes utilizadas por `fseek`:

- `SEEK_SET`: posição relativa ao início;
- `SEEK_CUR`: posição relativa ao local atual;
- `SEEK_END`: posição relativa ao final.

## 5.6 Exemplo completo: texto e binário

```c
#include <stdio.h>
#include <stdlib.h>

#define TAM_NOME 50

typedef struct {
    int matricula;
    char nome[TAM_NOME];
    float media;
} Aluno;

int salvar_texto(const char *caminho, const Aluno *aluno) {
    FILE *arquivo = fopen(caminho, "w");
    if (arquivo == NULL) {
        return 0;
    }

    int sucesso = fprintf(
        arquivo,
        "%d;%s;%.2f\n",
        aluno->matricula,
        aluno->nome,
        aluno->media
    ) > 0;

    fclose(arquivo);
    return sucesso;
}

int salvar_binario(const char *caminho, const Aluno *aluno) {
    FILE *arquivo = fopen(caminho, "wb");
    if (arquivo == NULL) {
        return 0;
    }

    size_t gravados = fwrite(aluno, sizeof *aluno, 1, arquivo);
    fclose(arquivo);
    return gravados == 1;
}

int ler_binario(const char *caminho, Aluno *aluno) {
    FILE *arquivo = fopen(caminho, "rb");
    if (arquivo == NULL) {
        return 0;
    }

    size_t lidos = fread(aluno, sizeof *aluno, 1, arquivo);
    fclose(arquivo);
    return lidos == 1;
}

int main(void) {
    Aluno original = {2025001, "Maria", 9.2f};
    Aluno recuperado;

    if (!salvar_texto("aluno.txt", &original)) {
        fprintf(stderr, "Erro ao salvar o arquivo de texto.\n");
        return EXIT_FAILURE;
    }

    if (!salvar_binario("aluno.bin", &original)) {
        fprintf(stderr, "Erro ao salvar o arquivo binario.\n");
        return EXIT_FAILURE;
    }

    if (!ler_binario("aluno.bin", &recuperado)) {
        fprintf(stderr, "Erro ao ler o arquivo binario.\n");
        return EXIT_FAILURE;
    }

    printf(
        "Matricula: %d\nNome: %s\nMedia: %.2f\n",
        recuperado.matricula,
        recuperado.nome,
        recuperado.media
    );

    return EXIT_SUCCESS;
}
```

> A gravação direta de uma `struct` em arquivo binário é prática para exercícios, mas pode não ser portátil entre arquiteturas, compiladores ou versões diferentes da estrutura.

---

# 6. Complexidade de algoritmos

## 6.1 Objetivo

A análise de complexidade estima como o consumo de tempo ou memória cresce quando o tamanho da entrada aumenta. O objetivo não é medir segundos exatos, mas comparar a taxa de crescimento dos algoritmos.

Normalmente, `n` representa a quantidade de elementos da entrada.

## 6.2 Complexidade de tempo e espaço

- **Complexidade de tempo:** quantidade de operações relevantes executadas.
- **Complexidade de espaço:** quantidade adicional de memória utilizada.

## 6.3 Casos de análise

- **Melhor caso:** entrada que exige o menor trabalho.
- **Caso médio:** comportamento esperado considerando entradas comuns.
- **Pior caso:** entrada que exige o maior número de operações.

## 6.4 Notações assintóticas

| Notação | Interpretação |
|---|---|
| `O(g(n))` | Limite superior assintótico |
| `Ω(g(n))` | Limite inferior assintótico |
| `Θ(g(n))` | Limite assintótico exato |

Em análises introdutórias, a notação `O` é frequentemente usada para descrever o pior caso.

## 6.5 Ordens de crescimento comuns

| Complexidade | Nome | Exemplo |
|---|---|---|
| `O(1)` | Constante | Acessar `vetor[i]` |
| `O(log n)` | Logarítmica | Busca binária |
| `O(n)` | Linear | Percorrer um vetor |
| `O(n log n)` | Linear-logarítmica | Algoritmos eficientes de ordenação |
| `O(n²)` | Quadrática | Dois laços aninhados sobre a entrada |
| `O(2^n)` | Exponencial | Algumas soluções recursivas por força bruta |
| `O(n!)` | Fatorial | Geração de todas as permutações |

## 6.6 Regras práticas

- constantes multiplicativas são ignoradas: `O(2n)` torna-se `O(n)`;
- termos menores são ignorados: `O(n² + n + 1)` torna-se `O(n²)`;
- blocos sequenciais são somados e o maior termo prevalece;
- laços aninhados geralmente multiplicam seus custos;
- uma entrada reduzida pela metade a cada passo sugere `O(log n)`.

### Exemplo linear

```c
for (size_t i = 0; i < n; i++) {
    printf("%d\n", vetor[i]);
}
```

O laço executa `n` vezes: `O(n)`.

### Exemplo quadrático

```c
for (size_t i = 0; i < n; i++) {
    for (size_t j = 0; j < n; j++) {
        printf("%zu %zu\n", i, j);
    }
}
```

O bloco interno executa `n × n` vezes: `O(n²)`.

---

# 7. Tipos Abstratos de Dados

Um **Tipo Abstrato de Dados**, ou **TAD**, descreve um conjunto de dados e as operações permitidas, sem exigir que o usuário conheça os detalhes internos da implementação.

## 7.1 Interface e implementação

- **Interface:** declara o que o TAD oferece.
- **Implementação:** define como as operações funcionam internamente.
- **Encapsulamento:** impede que outras partes do programa dependam diretamente da representação interna.

Exemplo de interface de uma pilha:

```c
#ifndef PILHA_H
#define PILHA_H

#include <stddef.h>

typedef struct Pilha Pilha;

Pilha *pilha_criar(void);
int pilha_empilhar(Pilha *pilha, int valor);
int pilha_desempilhar(Pilha *pilha, int *valor);
int pilha_vazia(const Pilha *pilha);
size_t pilha_tamanho(const Pilha *pilha);
void pilha_destruir(Pilha *pilha);

#endif
```

O arquivo de cabeçalho mostra apenas as operações públicas. Os campos internos de `struct Pilha` podem permanecer no arquivo de implementação.

## 7.2 Vantagens

- reduz o acoplamento entre módulos;
- permite trocar a implementação sem alterar o código cliente;
- melhora testes, manutenção e reutilização;
- protege invariantes da estrutura.

Listas, pilhas e filas podem ser implementadas como TADs.

---

# 8. Algoritmos de busca

## 8.1 Busca sequencial

A busca sequencial percorre os elementos desde o início até encontrar o valor ou atingir o final.

- não exige dados ordenados;
- implementação simples;
- pior caso: `O(n)`;
- melhor caso: `O(1)`.

## 8.2 Busca binária

A busca binária compara o valor procurado com o elemento central e elimina metade do intervalo a cada etapa.

- exige dados ordenados;
- pior caso: `O(log n)`;
- melhor caso: `O(1)`.

## 8.3 Exemplo completo

```c
#include <stdio.h>
#include <stddef.h>

int busca_sequencial(const int vetor[], size_t tamanho, int alvo) {
    for (size_t i = 0; i < tamanho; i++) {
        if (vetor[i] == alvo) {
            return (int)i;
        }
    }
    return -1;
}

int busca_binaria(const int vetor[], size_t tamanho, int alvo) {
    size_t inicio = 0;
    size_t fim = tamanho;

    while (inicio < fim) {
        size_t meio = inicio + (fim - inicio) / 2;

        if (vetor[meio] == alvo) {
            return (int)meio;
        }

        if (vetor[meio] < alvo) {
            inicio = meio + 1;
        } else {
            fim = meio;
        }
    }

    return -1;
}

int main(void) {
    int valores[] = {3, 7, 12, 18, 25, 31, 44};
    size_t tamanho = sizeof valores / sizeof valores[0];
    int alvo = 25;

    int posicao_sequencial = busca_sequencial(valores, tamanho, alvo);
    int posicao_binaria = busca_binaria(valores, tamanho, alvo);

    printf("Busca sequencial: %d\n", posicao_sequencial);
    printf("Busca binaria: %d\n", posicao_binaria);
    return 0;
}
```

## 8.4 Comparação

| Critério | Busca sequencial | Busca binária |
|---|---|---|
| Dados precisam estar ordenados | Não | Sim |
| Pior caso | `O(n)` | `O(log n)` |
| Estrutura mais adequada | Vetores e listas | Vetores com acesso por índice |
| Simplicidade | Alta | Média |

A busca binária não é eficiente em uma lista encadeada comum, pois a lista não oferece acesso direto ao elemento central.

---

# 9. Listas encadeadas

## 9.1 Conceito

Uma lista encadeada é formada por nós alocados dinamicamente. Cada nó armazena um dado e pelo menos um ponteiro de ligação.

```c
typedef struct No {
    int valor;
    struct No *proximo;
} No;
```

Ao contrário de um vetor, os nós não precisam ocupar posições consecutivas na memória.

## 9.2 Tipos de lista

### Lista simplesmente encadeada

Cada nó aponta apenas para o próximo. O percurso ocorre em um único sentido.

### Lista duplamente encadeada

Cada nó possui um ponteiro para o próximo e outro para o anterior. Permite percurso nos dois sentidos, mas utiliza mais memória.

### Lista circular

O último nó aponta para o primeiro. É útil em problemas cíclicos, como escalonamento circular e buffers.

### Lista de tipos estruturados

O campo de dados do nó pode ser uma estrutura completa, como um aluno, produto ou processo.

## 9.3 Operações principais

- inserção no início, no final ou em uma posição;
- remoção de um elemento;
- busca;
- percurso;
- liberação de todos os nós.

## 9.4 Exemplo completo

```c
#include <stdio.h>
#include <stdlib.h>

typedef struct No {
    int valor;
    struct No *proximo;
} No;

int inserir_final(No **inicio, int valor) {
    No *novo = malloc(sizeof *novo);
    if (novo == NULL) {
        return 0;
    }

    novo->valor = valor;
    novo->proximo = NULL;

    if (*inicio == NULL) {
        *inicio = novo;
        return 1;
    }

    No *atual = *inicio;
    while (atual->proximo != NULL) {
        atual = atual->proximo;
    }

    atual->proximo = novo;
    return 1;
}

No *buscar(No *inicio, int valor) {
    for (No *atual = inicio; atual != NULL; atual = atual->proximo) {
        if (atual->valor == valor) {
            return atual;
        }
    }
    return NULL;
}

int remover(No **inicio, int valor) {
    No *atual = *inicio;
    No *anterior = NULL;

    while (atual != NULL && atual->valor != valor) {
        anterior = atual;
        atual = atual->proximo;
    }

    if (atual == NULL) {
        return 0;
    }

    if (anterior == NULL) {
        *inicio = atual->proximo;
    } else {
        anterior->proximo = atual->proximo;
    }

    free(atual);
    return 1;
}

void imprimir(const No *inicio) {
    for (const No *atual = inicio; atual != NULL; atual = atual->proximo) {
        printf("%d -> ", atual->valor);
    }
    puts("NULL");
}

void liberar_lista(No **inicio) {
    No *atual = *inicio;

    while (atual != NULL) {
        No *proximo = atual->proximo;
        free(atual);
        atual = proximo;
    }

    *inicio = NULL;
}

int main(void) {
    No *lista = NULL;

    if (!inserir_final(&lista, 10) ||
        !inserir_final(&lista, 20) ||
        !inserir_final(&lista, 30)) {
        fprintf(stderr, "Falha de memoria.\n");
        liberar_lista(&lista);
        return EXIT_FAILURE;
    }

    imprimir(lista);

    No *encontrado = buscar(lista, 20);
    printf("Busca: %s\n", encontrado != NULL ? "encontrado" : "nao encontrado");

    remover(&lista, 20);
    imprimir(lista);

    liberar_lista(&lista);
    return EXIT_SUCCESS;
}
```

## 9.5 Complexidade típica

| Operação | Lista simplesmente encadeada |
|---|---|
| Acesso por posição | `O(n)` |
| Busca | `O(n)` |
| Inserção no início | `O(1)` |
| Inserção no final sem ponteiro de cauda | `O(n)` |
| Inserção no final com ponteiro de cauda | `O(1)` |
| Remoção no início | `O(1)` |

---

# 10. Filas

## 10.1 Conceito

Uma fila segue o princípio **FIFO**: *First In, First Out*. O primeiro elemento inserido é o primeiro a ser removido.

Operações principais:

- `enqueue`: insere no final;
- `dequeue`: remove do início;
- `front`: consulta o primeiro elemento;
- `rear`: consulta o último elemento;
- verificação de fila vazia.

## 10.2 Tipos de fila

- **Fila simples:** segue estritamente a ordem FIFO.
- **Fila circular:** reaproveita posições de um vetor.
- **Deque:** permite inserção e remoção nas duas extremidades.
- **Fila de prioridade:** a remoção considera uma prioridade, e não apenas a ordem de chegada.

## 10.3 Aplicações

- escalonamento de processos;
- filas de impressão;
- buffers de entrada e saída;
- transmissão de pacotes;
- simulação de atendimento;
- processamento de tarefas.

## 10.4 Exemplo completo com lista encadeada

```c
#include <stdio.h>
#include <stdlib.h>

typedef struct NoFila {
    int valor;
    struct NoFila *proximo;
} NoFila;

typedef struct {
    NoFila *inicio;
    NoFila *fim;
    size_t tamanho;
} Fila;

void fila_inicializar(Fila *fila) {
    fila->inicio = NULL;
    fila->fim = NULL;
    fila->tamanho = 0;
}

int enqueue(Fila *fila, int valor) {
    NoFila *novo = malloc(sizeof *novo);
    if (novo == NULL) {
        return 0;
    }

    novo->valor = valor;
    novo->proximo = NULL;

    if (fila->fim == NULL) {
        fila->inicio = novo;
    } else {
        fila->fim->proximo = novo;
    }

    fila->fim = novo;
    fila->tamanho++;
    return 1;
}

int dequeue(Fila *fila, int *valor) {
    if (fila->inicio == NULL) {
        return 0;
    }

    NoFila *removido = fila->inicio;
    *valor = removido->valor;
    fila->inicio = removido->proximo;

    if (fila->inicio == NULL) {
        fila->fim = NULL;
    }

    free(removido);
    fila->tamanho--;
    return 1;
}

void fila_destruir(Fila *fila) {
    int descartado;
    while (dequeue(fila, &descartado)) {
        // Remove todos os elementos.
    }
}

int main(void) {
    Fila fila;
    fila_inicializar(&fila);

    if (!enqueue(&fila, 10) || !enqueue(&fila, 20) || !enqueue(&fila, 30)) {
        fprintf(stderr, "Falha de memoria.\n");
        fila_destruir(&fila);
        return EXIT_FAILURE;
    }

    int valor;
    while (dequeue(&fila, &valor)) {
        printf("Removido: %d\n", valor);
    }

    return EXIT_SUCCESS;
}
```

Com ponteiros para o início e para o fim, inserção e remoção possuem custo `O(1)`.

---

# 11. Pilhas

## 11.1 Conceito

Uma pilha segue o princípio **LIFO**: *Last In, First Out*. O último elemento inserido é o primeiro a ser removido.

Operações principais:

- `push`: insere no topo;
- `pop`: remove do topo;
- `peek` ou `top`: consulta o topo sem remover;
- verificação de pilha vazia.

## 11.2 Aplicações

- chamadas e retornos de funções;
- desfazer e refazer ações;
- histórico de navegação;
- avaliação de expressões;
- busca em profundidade;
- verificação de símbolos balanceados.

## 11.3 Exemplo completo com lista encadeada

```c
#include <stdio.h>
#include <stdlib.h>

typedef struct NoPilha {
    int valor;
    struct NoPilha *proximo;
} NoPilha;

typedef struct {
    NoPilha *topo;
    size_t tamanho;
} Pilha;

void pilha_inicializar(Pilha *pilha) {
    pilha->topo = NULL;
    pilha->tamanho = 0;
}

int push(Pilha *pilha, int valor) {
    NoPilha *novo = malloc(sizeof *novo);
    if (novo == NULL) {
        return 0;
    }

    novo->valor = valor;
    novo->proximo = pilha->topo;
    pilha->topo = novo;
    pilha->tamanho++;
    return 1;
}

int pop(Pilha *pilha, int *valor) {
    if (pilha->topo == NULL) {
        return 0;
    }

    NoPilha *removido = pilha->topo;
    *valor = removido->valor;
    pilha->topo = removido->proximo;

    free(removido);
    pilha->tamanho--;
    return 1;
}

int peek(const Pilha *pilha, int *valor) {
    if (pilha->topo == NULL) {
        return 0;
    }

    *valor = pilha->topo->valor;
    return 1;
}

void pilha_destruir(Pilha *pilha) {
    int descartado;
    while (pop(pilha, &descartado)) {
        // Remove todos os elementos.
    }
}

int main(void) {
    Pilha pilha;
    pilha_inicializar(&pilha);

    if (!push(&pilha, 10) || !push(&pilha, 20) || !push(&pilha, 30)) {
        fprintf(stderr, "Falha de memoria.\n");
        pilha_destruir(&pilha);
        return EXIT_FAILURE;
    }

    int topo;
    if (peek(&pilha, &topo)) {
        printf("Topo: %d\n", topo);
    }

    while (pop(&pilha, &topo)) {
        printf("Removido: %d\n", topo);
    }

    return EXIT_SUCCESS;
}
```

As operações no topo possuem custo `O(1)`.

---

# 12. Comparações importantes

## 12.1 Vetor e lista encadeada

| Critério | Vetor | Lista encadeada |
|---|---|---|
| Organização na memória | Contígua | Nós podem estar separados |
| Acesso por índice | `O(1)` | `O(n)` |
| Inserção no início | `O(n)` | `O(1)` |
| Tamanho | Fixo ou redimensionado | Dinâmico |
| Memória extra | Baixa | Ponteiros em cada nó |
| Localidade de cache | Melhor | Geralmente pior |

## 12.2 Pilha e fila

| Estrutura | Política | Inserção | Remoção |
|---|---|---|---|
| Pilha | LIFO | Topo | Topo |
| Fila | FIFO | Final | Início |

## 12.3 Complexidade resumida

| Estrutura ou algoritmo | Operação | Complexidade típica |
|---|---|---|
| Vetor | Acesso por índice | `O(1)` |
| Vetor | Busca não ordenada | `O(n)` |
| Busca binária | Busca em vetor ordenado | `O(log n)` |
| Lista encadeada | Busca | `O(n)` |
| Lista encadeada | Inserção no início | `O(1)` |
| Pilha | `push`, `pop`, `peek` | `O(1)` |
| Fila encadeada | `enqueue`, `dequeue` | `O(1)` |

---

# 13. Compilação dos exemplos

Os exemplos foram escritos para C11 e podem ser compilados com GCC:

```bash
gcc -std=c11 -Wall -Wextra -Wpedantic arquivo.c -o programa
```

Execução no Linux:

```bash
./programa
```

No Windows com MinGW:

```powershell
gcc -std=c11 -Wall -Wextra -Wpedantic arquivo.c -o programa.exe
.\programa.exe
```

Para detectar diversos erros de memória durante os testes, pode-se utilizar sanitizadores quando disponíveis:

```bash
gcc -std=c11 -Wall -Wextra -Wpedantic \
    -fsanitize=address,undefined -g arquivo.c -o programa
```

---

# 14. Boas práticas

- inicializar ponteiros que ainda não possuem endereço com `NULL`;
- verificar o resultado das alocações de memória;
- liberar toda memória dinâmica quando ela não for mais necessária;
- definir o ponteiro como `NULL` depois de `free` quando ele continuar no escopo;
- verificar se `fopen` retornou `NULL`;
- fechar todos os arquivos abertos;
- evitar acesso fora dos limites de vetores;
- separar interface e implementação ao criar TADs;
- documentar pré-condições e valores de retorno das funções;
- compilar com avisos habilitados;
- testar casos normais, estruturas vazias e falhas de alocação.

---

## Licença e finalidade

Este repositório possui finalidade acadêmica e pode ser utilizado para estudo, revisão e organização das atividades da disciplina.
