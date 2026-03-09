---
layout: default
title: Guia - Conteúdo Programático | Introdução à Programação em Python
description: Material didático do workshop promovido pela PyLadies Beira
---

## Guia - Conteúdo Programático

# O que é Programação?

Programar é dar instruções ao computador para que ele execute tarefas.

Essas instruções são escritas em uma linguagem que o computador consegue entender.

Hoje vamos usar **Python**, uma linguagem simples e muito utilizada no mercado.

Python é usado em áreas como:

- Desenvolvimento web com Django
- Análise de dados com Pandas
- Inteligência Artificial com TensorFlow

---

# 2 - Exibindo informações na tela

## Função `print()`

A função `print()` é usada para mostrar informações na tela.

```python
print("Olá, mundo!")
```

O texto entre aspas é chamado de **string** (texto).

---

# 3 - Variáveis

Uma variável é um espaço onde guardamos uma informação.

```python
nome = "Maria"
idade = 20
```

O símbolo `=` significa **atribuição**.  
Estamos dizendo: guarde esse valor dentro dessa variável.

Podemos mostrar o valor assim:

```python
print(nome)
print(idade)
```

# 4 - Tipos de Dados

Em Python, cada valor tem um tipo.

## String (`str`)

Representa texto.

```python
nome = "João"
```

Texto sempre entre aspas.

---

## Inteiro (`int`)

Representa números inteiros.

```python
idade = 25
```

---

## Decimal (`float`)

Representa números com casas decimais.

```python
altura = 1.75
```

---

## Booleano (`bool`)

Representa valores lógicos.

```python
ativo  =  True
```

Valores possíveis:

- `True`
- `False`

---

## Comparando texto e número

```python
print("2" + "2")
print(2 + 2)
```

Texto se junta.  
Número soma.

---

# 5 - Entrada de Dados

Usamos `input()` para receber dados do usuário.

```python
nome = input("Digite seu nome: ")
```

Importante:  
`input()` sempre retorna texto.

Para converter para número:

```python
idade = int(input("Digite sua idade: "))
nota = float(input("Digite sua nota: "))
```

---

# 6 - Estruturas Condicionais

Permitem que o programa tome decisões.

```python
if idade >= 18:
  print("Maior de idade")
else:
  print("Menor de idade")
```

Se a condição for verdadeira -> executa o bloco do `if`.  
Caso contrário -> executa o bloco do `else`.

---

## Operadores de comparação

- `==` igual
- `!=` diferente
- `>` maior que
- `<` menor que
- `>=` maior ou igual
- `<=` menor ou igual

Atenção:

- `=` é usado para atribuir valor
- `==` é usado para comparar

---

## Operador `%` (módulo)

O símbolo `%` retorna o resto de uma divisão.

```python
numero = 7
print(numero % 2)
```

Se o resto da divisão por 2 for 0 - número é par.

---

# 7 - Estruturas de Repetição

Permitem repetir um bloco de código várias vezes.

---

## For

Usado quando sabemos quantas vezes queremos repetir algo.

```python
for i in range(1, 6):
  print(i)
```

### `range(início, fim)`

Gera uma sequência de números.

O número final não é incluído.

`range(1, 6)` gera:  
1, 2, 3, 4, 5

---

## While

Executa enquanto a condição for verdadeira.

```python
contador = 1

while contador <= 5:
  print(contador)
  contador += 1
```

### `+=`

É uma forma resumida de:

contador = contador + 1

---

# 8 - Listas

Lista é uma estrutura que armazena vários valores.

```python
nomes = ["Ana", "Carlos", "João"]
```

Podemos acessar um item:

```python
print(nomes[0])
```

O índice começa em 0.

---

## Adicionando itens

```python
nomes.append("Maria")
```

## Percorrendo lista

```python
for nome in nomes:
  print(nome)
```

---

# 9 - Funções

Função é um bloco de código reutilizável.

```python
def saudacao(nome):
  print("Olá", nome)
```

Chamando a função:

```python
saudacao("Maria")
```

Funções ajudam a organizar melhor o código.

---
