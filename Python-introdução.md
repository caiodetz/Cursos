### Introdução ao Python

Python é uma linguagem de programação de alto nível, interpretada e de fácil leitura. Criada por Guido van Rossum e lançada em 1991, tornou-se popular por sua simplicidade e versatilidade, sendo amplamente utilizada em desenvolvimento web, ciência de dados, automação, aprendizado de máquina e muito mais.

Vamos explorar alguns conceitos básicos de Python com exemplos de código.

### 1. Sintaxe Básica

#### Hello, World!
O clássico exemplo para começar com qualquer linguagem de programação.

```python
print("Hello, World!")
```

- **`print()`**: Função que exibe o texto ou o valor de uma variável na tela.

#### Variáveis e Tipos de Dados

Em Python, você não precisa declarar explicitamente o tipo de uma variável. A atribuição de um valor determina o tipo dela.

```python
# Inteiro
idade = 25

# Float (número decimal)
altura = 1.75

# String (texto)
nome = "Alice"

# Booleano (Verdadeiro ou Falso)
estudante = True
```

#### Operações Matemáticas
Python permite realizar operações matemáticas básicas de forma intuitiva.

```python
a = 10
b = 5

soma = a + b        # Adição: 15
subtracao = a - b   # Subtração: 5
multiplicacao = a * b # Multiplicação: 50
divisao = a / b     # Divisão: 2.0
modulo = a % b      # Módulo (resto da divisão): 0
potencia = a ** b   # Potência: 100000
```

#### Estruturas de Controle
Controle de fluxo com `if`, `for` e `while`.

```python
# Condicional if
idade = 20

if idade >= 18:
    print("Você é maior de idade.")
else:
    print("Você é menor de idade.")
```

```python
# Loop for
for i in range(5):  # Itera de 0 a 4
    print(f"Iteração número {i}")
```

```python
# Loop while
contador = 0
while contador < 5:
    print(f"Contador: {contador}")
    contador += 1
```

### 2. Estruturas de Dados

#### Listas
Listas são coleções ordenadas de elementos que podem ser alterados.

```python
# Criando uma lista
frutas = ["maçã", "banana", "laranja"]

# Acessando elementos
print(frutas[0])  # maçã

# Adicionando um elemento
frutas.append("uva")

# Removendo um elemento
frutas.remove("banana")

# Tamanho da lista
print(len(frutas))  # 3
```

#### Dicionários
Dicionários são coleções de pares chave-valor.

```python
# Criando um dicionário
pessoa = {
    "nome": "João",
    "idade": 30,
    "cidade": "São Paulo"
}

# Acessando um valor
print(pessoa["nome"])  # João

# Adicionando um novo par chave-valor
pessoa["email"] = "joao@example.com"

# Removendo um par chave-valor
del pessoa["cidade"]
```

### 3. Funções

Funções são blocos de código reutilizáveis que executam uma tarefa específica.

```python
# Definindo uma função
def saudacao(nome):
    print(f"Olá, {nome}!")

# Chamando a função
saudacao("Alice")  # Olá, Alice!
```

```python
# Função com retorno de valor
def soma(a, b):
    return a + b

resultado = soma(10, 5)
print(resultado)  # 15
```

### 4. Módulos e Pacotes

Python possui uma vasta biblioteca padrão com módulos prontos para uso.

```python
import math

# Usando funções do módulo math
raiz_quadrada = math.sqrt(16)  # 4.0
print(raiz_quadrada)
```

### 5. Entrada e Saída de Dados

Interação com o usuário e manipulação de arquivos.

```python
# Entrada de dados
nome = input("Digite seu nome: ")
print(f"Olá, {nome}!")

# Manipulação de arquivos
# Escrevendo em um arquivo
with open("arquivo.txt", "w") as arquivo:
    arquivo.write("Escrevendo em um arquivo de texto.")

# Lendo de um arquivo
with open("arquivo.txt", "r") as arquivo:
    conteudo = arquivo.read()
    print(conteudo)
```

### 6. Trabalhando com Bibliotecas Externas

Python tem uma comunidade enorme, com diversas bibliotecas que facilitam o trabalho em diferentes áreas.

```python
# Instalando uma biblioteca (no terminal)
# pip install requests

# Usando uma biblioteca externa
import requests

resposta = requests.get("https://api.github.com")
print(resposta.json())
```

### 7. Orientação a Objetos

Python suporta programação orientada a objetos.

```python
# Criando uma classe
class Cachorro:
    def __init__(self, nome, idade):
        self.nome = nome
        self.idade = idade

    def latir(self):
        print(f"{self.nome} está latindo!")

# Instanciando um objeto
meu_cachorro = Cachorro("Rex", 5)
meu_cachorro.latir()  # Rex está latindo!
```

Esses são apenas os fundamentos do Python. A linguagem tem muitos outros recursos avançados, como programação funcional, geradores, decoradores, e muito mais. Dependendo de seu interesse, podemos explorar algum tópico específico com mais profundidade!
