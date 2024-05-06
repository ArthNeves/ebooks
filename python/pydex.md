# Python Commands for eBook

Este eBook é uma introdução abrangente aos comandos em Python, estruturado para oferecer desde conceitos básicos até programação avançada. Aqui você encontrará descrições simplificadas e exemplos de código real, para que possa aprender e aplicar imediatamente o Python em seus projetos.

```txt
Basics

├─ Variables
│  ├─ Declaring Variables
│  └─ Assigning Values
├─ Data Types
│  ├─ Integers
│  ├─ Floats
│  ├─ Strings
│  └─ Booleans
├─ Operators
│  ├─ Arithmetic Operators
│  ├─ Comparison Operators
│  └─ Logical Operators
└─ Control Flow
   ├─ if-else Statements
   ├─ for Loops
   └─ while Loops

Functions
├─ Defining Functions
├─ Calling Functions
├─ Function Parameters
└─ Return Statements

Data Structures
├─ Lists
│  ├─ Creating Lists
│  ├─ Accessing List Elements
│  └─ List Methods
├─ Tuples
│  ├─ Creating Tuples
│  └─ Accessing Tuple Elements
└─ Dictionaries
   ├─ Creating Dictionaries
   ├─ Accessing Dictionary Elements
   └─ Dictionary Methods

File I/O
├─ Opening Files
├─ Reading Files
├─ Writing Files
└─ Closing Files

Modules
├─ Importing Modules
├─ Creating Modules
└─ Exploring Standard Library Modules

Exception Handling
├─ try-except Blocks
├─ Raising Exceptions
└─ Custom Exceptions

Object-Oriented Programming
├─ Classes
│  ├─ Defining Classes
│  ├─ Creating Objects
│  └─ Class Attributes and Methods
└─ Inheritance
   ├─ Subclassing
   └─ Method Overriding

Web Development
├─ Flask
│  ├─ Creating a Flask App
│  ├─ Routing
│  └─ Templates
└─ Django
   ├─ Creating a Django Project
   ├─ Models
   └─ Views and URLs

Data Analysis
├─ NumPy
│  ├─ Arrays
│  └─ Mathematical Functions
└─ Pandas
   ├─ DataFrames
   └─ Data Manipulation

Automation
├─ os Module
   └─ File and Directory Operations
├─ subprocess Module
   └─ Running Shell Commands
└─ shutil Module
   └─ File and Directory Operation
```

# Basics

## Variables

### Declaring Variables

Para declarar variáveis em Python, basta atribuir um valor a um nome. Python é uma linguagem dinamicamente tipada, então você não precisa especificar o tipo de dados.

```python
x = 10  # Inteiro
y = 20.5  # Ponto flutuante
```

### Assigning Values

Você pode reatribuir valores para uma variável já existente a qualquer momento.

```python
x = 15  # x agora é 15
```

## Data Types

### Integers

São números inteiros, positivos ou negativos, sem parte decimal.

```python
age = 25
```
### Floats

Representam números reais e podem incluir uma parte decimal.

```python
height = 175.5
```
### Strings

Texto entre aspas simples ou duplas.

```python
name = "John Doe"
```

### Booleans

Valores lógicos que podem ser True ou False.

```python
is_online = True
is_online = False
```

## Operators

### Arithmetic Operators

Usados para realizar operações matemáticas como adição, subtração, multiplicação e divisão.

```python
sum = 10 + 5  # 15
product = 10 * 5  # 50
```

### Comparison Operators

Usados para comparar valores. Retorna True ou False.

python
print(10 > 5)  # True
print(10 == 5)  # False

### Logical Operators

Usados para combinar condições lógicas.

python
print(10 > 5 and 10 < 20)  # True
print(10 < 5 or 10 < 20)  # True

## Control Flow

### if-else Statements

Permite que você execute condicionalmente blocos de código.

python
if age >= 18:
    print("Adult")
else:
    print("Minor")

### for Loops
Executa um bloco de código várias vezes, útil para iterar sobre uma sequência.

python
for i in range(5):
    print(i)

### while Loops

Repete um bloco de código enquanto uma condição é verdadeira.

python
i = 0
while i < 5:
    print(i)
    i += 1

# Functions

## Defining Functions

Você pode definir funções para encapsular código para reutilização.

```python
def greet(name):
    return "Hello, " + name
```

## Calling Functions

Chama uma função para executar seu código.

```python
print(greet("Alice"))
```

## Function Parameters

Passa informações para funções através de parâmetros.

```python
def greet(name, message):
    return f"{message}, {name}"
```

## Return Statements

Retorna um valor de uma função.

```python
def sum(a, b):
    return a + b
```

Data Structures
Lists
Creating Lists
Listas são coleções ordenadas e mutáveis.

python
fruits = ["apple", "banana", "cherry"]
Accessing List Elements
Você pode acessar elementos da lista pelo índice.

python
print(fruits[1])  # banana
List Methods
Listas têm métodos como append(), remove(), pop(), etc.

python
fruits.append("orange")
Tuples
Creating Tuples
Tuplas são coleções ordenadas e imutáveis.

python
dimensions = (200, 50)
Accessing Tuple Elements
Acesso similar às listas, mas as tuplas não podem ser alteradas.

python
print(dimensions[0])  # 200
Dictionaries
Creating Dictionaries
Dicionários armazenam pares chave-valor.

python
car = {"brand": "Ford", "model": "Mustang", "year": 1964}
Accessing Dictionary Elements
Acesse elementos por suas chaves.

python
print(car["model"])  # Mustang
Dictionary Methods
Dicionários têm métodos como get(), keys(), values(), e update().

python
car.update({"color": "red"})

Data Structures (Continuação)
Dictionary Methods
Dicionários têm métodos que facilitam o gerenciamento de pares chave-valor.

python
car.update({"color": "red"})  # Atualiza o dicionário com uma nova chave-valor
print(car.get("brand"))  # Retorna o valor da chave 'brand'
File I/O
Opening Files
Para trabalhar com arquivos em Python, primeiro você precisa abrir um arquivo.

python
file = open("example.txt", "r")  # Abre um arquivo para leitura
Reading Files
Depois de abrir um arquivo, você pode ler seu conteúdo.

python
content = file.read()
print(content)
Writing Files
Abrir um arquivo em modo de escrita permite que você escreva nele.

python
file = open("example.txt", "w")
file.write("Hello, Python!")
Closing Files
É importante fechar arquivos para liberar recursos do sistema.

python
file.close()
Modules
Importing Modules
Módulos são conjuntos de funções e classes que você pode importar e usar em seu código.

python
import math
print(math.sqrt(16))  # Imprime a raiz quadrada de 16
Creating Modules
Você pode criar seus próprios módulos simplesmente salvando seu código em um arquivo .py e importando-o.

python
# save this as mymodule.py
def greeting(name):
    print("Hello, " + name)
python
# another Python file
import mymodule
mymodule.greeting("Python")
Exploring Standard Library Modules
Python vem com uma biblioteca padrão que oferece muitos módulos úteis.

python
import os
print(os.getcwd())  # Imprime o diretório de trabalho atual
Exception Handling
try-except Blocks
Trata exceções para evitar que o programa termine de forma inesperada.

python
try:
    print(10 / 0)
except ZeroDivisionError:
    print("You cannot divide by zero!")
Raising Exceptions
Você pode lançar exceções intencionalmente com raise.

python
x = -1
if x < 0:
    raise ValueError("That is not a valid value")
Custom Exceptions
Crie suas próprias exceções derivando da classe base Exception.

python
class MyError(Exception):
    pass

try:
    raise MyError("Something went wrong")
except MyError as e:
    print(e)
Object-Oriented Programming
Classes
Defining Classes
Classes são modelos para criar objetos (instâncias).

python
class Dog:
    species = "Canis familiaris"

    def __init__(self, name, age):
        self.name = name
        self.age = age
Creating Objects
Um objeto é uma instância de uma classe.

python
buddy = Dog("Buddy", 9)
Class Attributes and Methods
Atributos e métodos definem as propriedades e ações dos objetos.

python
print(buddy.name)  # Acessa o atributo 'name' do objeto 'buddy'
print(buddy.species)  # Acessa o atributo da classe 'species'

def bark(self):
    print(f"{self.name} says woof!")
Inheritance
Subclassing
Classes podem herdar características de outras classes.

python
class Bulldog(Dog):  # Herda de Dog
    pass
Method Overriding
Subclasses podem substituir métodos de suas superclasses.

python
class Bulldog(Dog):
    def bark(self):
        print(f"{self.name} says woof woof!")
Web Development
Flask
Creating a Flask App
Flask é um microframework para desenvolvimento web em Python.

python
from flask import Flask
app = Flask(__name__)

@app.route("/")
def home():
    return "Hello, Flask!"
Routing
Definir rotas permite associar funções a URLs específicas.

python
@app.route("/about")
def about():
    return "About Page"
Templates
Flask pode renderizar templates HTML, facilitando a construção de interfaces.

python
from flask import render_template

@app.route("/")
def home():
    return render_template("home.html")
Django
Creating a Django Project
Django é um framework web de alto nível que promove design limpo e pragmático.

python
# Inicie um novo projeto Django usando a linha de comando
django-admin startproject myproject
Models
Models em Django são definidos como classes Python e representam tabelas de banco de dados.

python
from django.db import models

class User(models.Model):
    name = models.CharField(max_length=100)
    age = models.IntegerField()
Views and URLs
Views lidam com a lógica de negócios e são ligadas a URLs específicas.

python
from django.urls import path
from . import views

urlpatterns = [
    path('', views.home, name='home'),
]

Data Analysis
NumPy
Arrays
NumPy é amplamente utilizado para operações numéricas com arrays.

python
import numpy as np

# Criando um array NumPy
data = np.array([1, 2, 3, 4])
print(data)
Mathematical Functions
NumPy oferece funções matemáticas que operam eficientemente em arrays.

python
# Calculando a média
mean = np.mean(data)
print("Média:", mean)

# Calculando o desvio padrão
std_dev = np.std(data)
print("Desvio padrão:", std_dev)
Pandas
DataFrames
Pandas é utilizado para manipulação de dados através de DataFrames, que são tabelas eficientes e poderosas.

python
import pandas as pd

# Criando um DataFrame
df = pd.DataFrame({
    "Name": ["Alice", "Bob", "Charlie"],
    "Age": [25, 30, 35],
    "City": ["New York", "Paris", "London"]
})
print(df)
Data Manipulation
Pandas permite uma vasta gama de manipulações de dados, como seleção, filtragem e agregação.

python
# Selecionando uma coluna
ages = df["Age"]
print(ages)

# Filtrando dados
older_than_30 = df[df["Age"] > 30]
print(older_than_30)
Automation
os Module
File and Directory Operations
O módulo os fornece uma maneira de realizar operações de sistema de arquivos, como mudar o diretório de trabalho e listar arquivos.

python
import os

# Mudando o diretório de trabalho
os.chdir('/path/to/directory')

# Listando arquivos no diretório
files = os.listdir('.')
print(files)
subprocess Module
Running Shell Commands
O módulo subprocess permite que você execute comandos do shell diretamente do Python.

python
import subprocess

# Executando um comando externo
result = subprocess.run(['ls', '-l'], capture_output=True, text=True)
print(result.stdout)
shutil Module
File and Directory Operations
O módulo shutil é útil para operações de arquivo de alto nível, incluindo copiar e mover arquivos.

python
import shutil

# Copiando um arquivo
shutil.copy('source.txt', 'destination.txt')

# Movendo um arquivo
shutil.move('source.txt', 'destination_folder')