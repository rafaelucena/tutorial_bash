---
title: variables-pt/br
---

## Variáveis
# Criando (Declarando) Variáveis em BASH

Variáveis são "containers" para armazenar informações. 

**Sintaxe:**

````bash
txt='Eita Giovana!';
x=5;
y=10.5;
    
echo ${txt};
echo ${x};
echo ${y};
````

Depois das linhas acima serem executadas, a variável ${txt} armazenará: Eita Giovana!, a variável ${x} armazenará: 5, e a variável ${y} armazenará: 10.5.

###### Nota1: Quando colocar texto numa variável, coloque aspas ao redor do valor.
###### Nota2: Aspas duplas ou aspas simples tem efeitos diferentes na variável.
###### Nota3: Variáveis são GLOBAIS por natureza. Isso é, elas podem ser utilizadas por outros scripts em diferentes momentos de execução.
###### Nota4: Variáveis não tem "tipo". Todas as variáveis em BASH são tratadas como caracteres de texto, mas, dependendo do contexto, BASH permite operações aritméticas. Nesse caso apenas quando o conteúdo da variável for apenas números. 

# Regras para Declarar Variáveis em BASH

* Devem começar com letras (a-Z) ou underline (_)
* Não podem começar com números
* Não podem conter espaços entre a variável, o '=' e o valor a ser declarado na variável
* Podem apenas conter caracteres alfanuméricos (a-Z, 0-9) e underlines (_)
* São case-sensitive (${txt} e ${TXT} são duas variáveis diferentes)

# Exibindo uma Variável

O comando `echo` em BASH é utilizado normalmente para exibir dados na tela. 

O próximo exemplo vai mostrar como exibir texto e uma variável:
````bash
txt='github.com';
echo "Eu amo o ${txt}!";
````

O próximo exemplo vai produzir o mesmo resultado do que o exemplo anterior:
````bash
txt='github.com';
txt="Eu amo o ${txt}!";
echo "${txt}";
````

O próximo exemplo vai produzir a soma de duas variáveis:
````bash
x=5;
y=4;
z=0;

((z=${x} + ${y}))

echo ${z}; 
````

# BASH é uma Linguagem de Programação Com Tipagem de Variáveis Simples

No exemplo, percebam como em nenhum momento foi especificado para o BASH qual tipo de dado a variável vai receber.
Tudo para o BASH é uma string (ou um arranjo[?]), então os dados são utilizados de formas diferentes dependendo do contexto
Em outras linguagens como C, C++, e Java, o programador deve declarar previamente o nome e o tipo da variável antes de utilizá-la.

#### Mais Informações:
###### @TODO
<!-- Please add any articles you think might be helpful to read before writing the article -->
