---
layout: default
title: Soluções de Ecercícios | Introdução à Programação em Python
description: Material didático do workshop promovido pela PyLadies Beira
---

# BLOCO 1 – Fundamentos e Condições

---

## Exercício 1 – Sistema de Maioridade

```python
nome = input("Digite seu nome: ")
idade = int(input("Digite sua idade: "))

if idade >= 18:
    print("Olá", nome + ", você é maior de idade.")
else:
    print("Olá", nome + ", você é menor de idade.")
```

---

## Exercício 2 – Sistema de Nota

```python
nome = input("Digite o nome do aluno: ")
nota = float(input("Digite a nota: "))

if nota >= 10:
    print(nome, "- Aprovado")
elif nota >= 8:
    print(nome, "- Recuperação")
else:
    print(nome, "- Reprovado")
```

---

## Desafio Extra – Positivo, Negativo ou Zero

```python
numero = float(input("Digite um número: "))

if numero > 0:
    print("Número positivo")
elif numero < 0:
    print("Número negativo")
else:
    print("Zero")
```

---

# BLOCO 2 – Laços e Listas

---

## Exercício 3 – Contagem 1 a 10

```python
for i in range(1, 11):
    print(i)

```

### Apenas números pares

```python
for i in range(1, 11):
    if i % 2 == 0:
        print(i)
```

---

## Exercício 4 – Cadastro de Nomes

```python
nomes = []

for i in range(3):
    nome = input("Digite um nome: ")
    nomes.append(nome)

print("Lista de nomes:")
for nome in nomes:
    print(nome)
```

---

## Exercício 5 – Soma de 5 Números

```python
soma = 0

for i in range(5):
    numero = float(input("Digite um número: "))
    soma += numero

print("Soma total:", soma)
```

---

# MINI PROJETO FINAL

---

## Versão Simples

```python
import random

numero = random.randint(1, 10)

tentativa = int(input("Adivinhe o número de 1 a 10: "))

if tentativa == numero:
    print("Acertou!")
else:
    print("Errou! O número era", numero)
```

---

## Versão Melhorada

```python
import random

numero = random.randint(1, 10)
tentativa = 0
contador = 0

while tentativa != numero:
    tentativa = int(input("Adivinhe o número de 1 a 10: "))
    contador += 1

    if tentativa == numero:
        print("Acertou!")
    else:
        print("Tente novamente.")

print("Você acertou em", contador, "tentativas!")
```

## Versão com limite de tentativa (Opcional)

```python
import random

numero = random.randint(1, 10)
contador = 0
max_tentativas = 3
acertou = False

while contador < max_tentativas and not acertou:
    tentativa = int(input("Adivinhe o número de 1 a 10: "))
    contador += 1

    if tentativa == numero:
        acertou = True
        print("Acertou!")
    else:
        print("Tente novamente.")

if not acertou:
    print("Você perdeu! O número era", numero)
```
