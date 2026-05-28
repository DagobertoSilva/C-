C++ para Programação Competitiva


# Roadmap 

## Parte 1 — Fundamentos

1. Introdução ao C++
2. Estrutura de um programa
3. Compilação
4. Entrada e saída
5. Variáveis
6. Tipos primitivos
7. Tipos especiais
8. Operadores
9. Condicionais
10. Loops
11. Funções
12. Recursão
13. Arrays
14. Strings
15. Ponteiros
16. Referências
17. Struct
18. Classes
19. OOP
20. Templates

---

# Introdução ao C++

## O que é C++?

C++ é uma linguagem:

- compilada
- rápida
- poderosa
- utilizada em:
  - jogos
  - sistemas operacionais
  - engines
  - maratonas de programação

---

# Estrutura Básica de um Programa

```cpp
#include <iostream>

using namespace std;

int main() {

    cout << "Olá mundo";

    return 0;
}
```

---

# Explicando Linha por Linha

## include

```cpp
#include <iostream>
```

Permite utilizar:

- `cout`
- `cin`

---

## namespace

```cpp
using namespace std;
```

Evita escrever:

```cpp
std::cout
std::cin
```

---

## main

```cpp
int main()
```

Função principal do programa.

Todo programa começa nela.

---

## cout

```cpp
cout << "Olá";
```

Exibe dados na tela.

---

## return 0

```cpp
return 0;
```

Indica que o programa terminou corretamente.

---

# Entrada e Saída

# cout

```cpp
cout << "Texto";
```

---

# cin

```cpp
int idade;

cin >> idade;
```

---

# Exemplo Completo

```cpp
#include <iostream>

using namespace std;

int main() {

    string nome;
    int idade;

    cin >> nome;
    cin >> idade;

    cout << nome << "\n";
    cout << idade << "\n";

    return 0;
}
```

---

# Quebra de Linha

## Usando endl

```cpp
cout << "Olá" << endl;
```

---

## Usando \\n

```cpp
cout << "Olá\n";
```

⚠️ Em maratona prefira:

```cpp
"\n"
```

pois é mais rápido.

---

# Variáveis

# O que são?

Variáveis armazenam valores na memória.

---

# Tipos Primitivos

| Tipo | Uso |
|---|---|
| int | inteiros |
| long long | inteiros grandes |
| float | reais |
| double | reais precisos |
| char | caracteres |
| bool | verdadeiro/falso |

---

# int

```cpp
int idade = 20;
```

Armazena números inteiros.

---

# long long

## Muito importante para maratona

```cpp
long long x = 1000000000000LL;
```

Usado para números grandes.

---

# double

```cpp
double altura = 1.75;
```

---

# char

```cpp
char letra = 'A';
```

---

# bool

```cpp
bool ligado = true;
```

---

# string

```cpp
string nome = "Dagoberto";
```

---

# Operadores

# Soma

```cpp
a + b
```

---

# Subtração

```cpp
a - b
```

---

# Multiplicação

```cpp
a * b
```

---

# Divisão

```cpp
a / b
```

---

# Resto

```cpp
a % b
```

---

# Incremento

```cpp
i++;
```

---

# Decremento

```cpp
i--;
```

---

# Condicionais

# if

```cpp
if(x > 0) {
    cout << "positivo";
}
```

---

# else

```cpp
if(x > 0) {
    cout << "positivo";
}
else {
    cout << "negativo";
}
```

---

# else if

```cpp
if(nota >= 9) {
    cout << "A";
}
else if(nota >= 7) {
    cout << "B";
}
else {
    cout << "C";
}
```

---

# Operadores Relacionais

| Operador | Significado |
|---|---|
| == | igual |
| != | diferente |
| > | maior |
| < | menor |
| >= | maior igual |
| <= | menor igual |

---

# Operadores Lógicos

| Operador | Significado |
|---|---|
| && | E |
| || | OU |
| ! | NÃO |

---

# Loops

# for

```cpp
for(int i = 0; i < 10; i++) {

    cout << i << "\n";

}
```

---

# while

```cpp
while(n > 0) {

    n--;

}
```

---

# do while

```cpp
do {

    cout << n;

} while(n > 0);
```

---

# Funções

# Criando Funções

```cpp
int soma(int a, int b) {

    return a + b;

}
```

---

# Chamando Funções

```cpp
cout << soma(2, 3);
```

---

# Passagem por Valor

```cpp
void teste(int x) {

    x++;

}
```

Não altera variável original.

---

# Passagem por Referência

```cpp
void teste(int &x) {

    x++;

}
```

Altera variável original.

---

# Arrays

# O que são?

Estruturas contíguas na memória.

---

# Declarando

```cpp
int v[5];
```

---

# Inicializando

```cpp
int v[5] = {1,2,3,4,5};
```

---

# Acessando

```cpp
cout << v[0];
```

---

# Vetores (vector)

# Biblioteca

```cpp
#include <vector>
```

---

# Criando

```cpp
vector<int> v;
```

---

# Inserindo

```cpp
v.push_back(10);
```

---

# Removendo

```cpp
v.pop_back();
```

---

# Tamanho

```cpp
v.size();
```

---

# Percorrendo

```cpp
for(int x : v) {

    cout << x << "\n";

}
```

---

# Ordenação

```cpp
sort(v.begin(), v.end());
```

---

# Ordem Decrescente

```cpp
sort(v.rbegin(), v.rend());
```

---

# Strings em C++

# std::string

```cpp
string nome = "Carlos";
```

---

# Tamanho

```cpp
nome.size();
```

---

# Concatenando

```cpp
nome += " Silva";
```

---

# Acessando Caracteres

```cpp
nome[0];
```

---

# Percorrendo String

```cpp
for(char c : nome) {

    cout << c << "\n";

}
```

---

# Pair

```cpp
pair<int,int> p;
```

---

# Inicializando

```cpp
p = {10,20};
```

---

# Acessando

```cpp
p.first
p.second
```

---

# Stack

# Pilha

```cpp
stack<int> st;
```

---

# Inserir

```cpp
st.push(10);
```

---

# Remover

```cpp
st.pop();
```

---

# Topo

```cpp
st.top();
```

---

# Queue

# Fila

```cpp
queue<int> q;
```

---

# Inserir

```cpp
q.push(10);
```

---

# Remover

```cpp
q.pop();
```

---

# Primeiro Elemento

```cpp
q.front();
```

---

# Priority Queue

# Heap

```cpp
priority_queue<int> pq;
```

---

# Menor no Topo

```cpp
priority_queue<
    int,
    vector<int>,
    greater<int>
> pq;
```

---

# Set

```cpp
set<int> s;
```

---

# Inserir

```cpp
s.insert(10);
```

---

# Buscar

```cpp
s.count(10);
```

---

# Map

```cpp
map<string,int> mp;
```

---

# Inserindo

```cpp
mp["Ana"] = 10;
```

---

# Complexidade Big-O

# O que é?

Mede desempenho do algoritmo.

---

# Complexidades comuns

| Complexidade | Nome |
|---|---|
| O(1) | constante |
| O(log n) | logarítmica |
| O(n) | linear |
| O(n log n) | quase linear |
| O(n²) | quadrática |

---

# Busca Binária

## Pré-requisito

Vetor ordenado.

---

# Exemplo

```cpp
int l = 0;
int r = n - 1;

while(l <= r) {

    int mid = (l + r) / 2;

    if(v[mid] == x) {
        break;
    }
    else if(v[mid] < x) {
        l = mid + 1;
    }
    else {
        r = mid - 1;
    }

}
```

---

# BFS

# Busca em largura

```cpp
queue<int> q;

q.push(src);

while(!q.empty()) {

    int u = q.front();
    q.pop();

    for(int v : adj[u]) {

        q.push(v);

    }

}
```

---

# DFS

# Busca em profundidade

```cpp
void dfs(int u) {

    vis[u] = true;

    for(int v : adj[u]) {

        if(!vis[v]) {
            dfs(v);
        }

    }

}
```

---

# Dijkstra

```cpp
priority_queue<
    pair<int,int>,
    vector<pair<int,int>>,
    greater<pair<int,int>>
> pq;
```

---

# Dynamic Programming

# Ideia

Guardar resultados já calculados.

---

# Fibonacci

```cpp
dp[0] = 0;
dp[1] = 1;

for(int i = 2; i <= n; i++) {

    dp[i] = dp[i-1] + dp[i-2];

}
```

---

# Template ICPC

```cpp
#include <bits/stdc++.h>

using namespace std;

#define fastio ios::sync_with_stdio(false); cin.tie(nullptr);

using ll = long long;

int main() {

    fastio;

    return 0;
}
```

---

# Erros Comuns

## Overflow

Use:

```cpp
long long
```

---

# Índices

Cuidado com:

```cpp
0-based
1-based
```

---

# Recursão infinita

Sempre tenha caso base.

---

# Exercícios Básicos

## Exercício 1

Leia dois números e mostre soma.

---

## Exercício 2

Leia um vetor e mostre o maior elemento.

---

## Exercício 3

Conte quantos números pares existem.

---

## Exercício 4

Faça busca linear.

---

## Exercício 5

Implemente busca binária.

---

# Exercícios Intermediários

## Exercício 6

Ordene um vetor.

---

## Exercício 7

Implemente pilha.

---

## Exercício 8

Implemente fila.

---

## Exercício 9

Conte frequência usando map.

---

## Exercício 10

Resolva Fibonacci com DP.

---

# Exercícios Avançados

## Exercício 11

Implemente BFS.

---

## Exercício 12

Implemente DFS.

---

## Exercício 13

Implemente Dijkstra.

---

## Exercício 14

Implemente Union Find.

---

## Exercício 15

Implemente Segment Tree.

---

# Sites para Treino

| Site | Uso |
|---|---|
| Codeforces | maratona |
| AtCoder | algoritmos |
| CSES | prática |
| Beecrowd | iniciantes |
| LeetCode | entrevistas |

---

# Roadmap de Estudos

## Iniciante

- variáveis
- loops
- arrays
- funções

---

## Intermediário

- STL
- busca binária
- grafos
- recursão

---

## Avançado

- DP
- segment tree
- strings avançadas
- teoria dos grafos

---

# Dicas de Maratona

- Leia o problema inteiro
- Faça casos pequenos
- Teste extremos
- Use fast I/O
- Evite overflow
- Treine diariamente

---

# Checklist Antes de Submeter

- Entrada correta?
- Saída correta?
- Complexidade boa?
- Overflow?
- Índices corretos?
- Casos extremos?
- Removeu debug?

---

# Fim
