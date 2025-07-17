# 1. Introdução – em atualização

Python é uma linguagem de programação de alto nível, interpretada e com tipagem dinâmica. Foi criada para ser simples, legível e poderosa, permitindo desenvolvimento rápido e conciso em diversas áreas como ciência de dados, automação, web, scripts, inteligência artificial e muito mais.

Características principais:

    - Simples, legível e elegante.
    - Multiplataforma (Linux, Windows, Mac).
    - Comunidade ativa e enorme quantidade de bibliotecas.
    - Ampla aplicação: scripts, web, IA, automação, jogos, etc.

# 2. História

    - 1989 – Guido van Rossum inicia o projeto durante as férias de Natal.
    - 1991 – Primeira versão pública do Python (0.9.0).
    - 2000 – Lançado o Python 2.0 com coleta de lixo e list comprehensions.
    - 2008 – Chega o Python 3.0, com mudanças profundas (não retrocompatível).
    - 2020 – Fim do suporte oficial ao Python 2.

    Atual – Python 3.x é amplamente utilizado em projetos modernos.

# 3. Conceitos Básicos

    Python é interpretado: o código é executado linha por linha, sem necessidade de compilação.

# 4. Comandos

    4.1 Comentários

    - # Comentário de uma linha
    - """ Comentário em várias linhas """

    4.2 Importação de Bibliotecas

    - import math  # Biblioteca matemática.
    - import random  # Geração de números aleatórios.
    - from datetime import datetime  # Data e hora.

    4.3 Ponto de entrada

    Python não exige main(), mas é prática comum:

    def main():
        print("Olá, mundo!")
        if __name__ == "__main__":
        main()

    4.4 Variáveis

    - numero = 10 - # Inteiro.
    - preco = 9.99 - # Float.
    - nome = "Python" - # String.
    - ativo = True - # Booleano.

    4.5 Caracteres especiais

    - \n # Quebra de linha.
    - \t # Tabulação.
    - \\ # Barra invertida.
    - \" # Aspas duplas.

    4.6 Funções principais

    - print("Mensagem") - # Exibe na tela.
    - input("Digite algo: ") - # Entrada de dados do usuário.
    - len("texto") - # Retorna o tamanho da string.
    - type(123) - # Retorna o tipo da variável.

    4.7 Tipos de Dados

    - int, float, str, bool, list, tuple, dict, set.
    - Conversão: int(), str(), float(), bool().

# 5. Operadores e Expressões

    - Aritméticos: +, -, *, /, //, %, **
    - Comparação: ==, !=, <, >, <=, >=
    - Lógicos: and, or, not
    - Atribuição: =, +=, -=, etc.

# 6. Estruturas de Controle

    Condições:

    if x > 0:
        print("Positivo")
    elif x == 0:
        print("Zero")
    else:
        print("Negativo")

    for i in range(5):
        print(i)
    while condição:

# 7. Funções

    def saudacao(nome):
    return f"Olá, {nome}!"

    print(saudacao("Maria"))

    *args, **kwargs

    Funções lambda: lambda x: x*2

# 8. Listas e Coleções

    - lista = [1, 2, 3]
    - tupla = (4, 5, 6)
    - conjunto = {7, 8, 9}
    - dicionario = {"nome": "Python", "versao": 3.11}

# 9. Orientação a Objetos

    class Pessoa:
        def __init__(self, nome):
            self.nome = nome

    def falar(self):
        print(f"Olá, eu sou {self.nome}.")

    p = Pessoa("João")
    p.falar()

# 10. Manipulação de Arquivos

    with open("arquivo.txt", "r") as f:
        conteudo = f.read()
        
# 11. Exceções

    try:
        x = int(input("Número: "))
    except ValueError:
        print("Entrada inválida")
    finally:
        print("Fim")

# 12. Modularização e Organização

    - Separar funções em arquivos .py
    - Usar import e __init__.py para pacotes
    - Estrutura recomendada para projetos Python

# 13. Criando um Módulo

    - arquivo: saudacao.py

    def ola(nome):
        return f"Olá, {nome}"

    - Em outro arquivo

    from saudacao import ola
        print(ola("Pedro"))
