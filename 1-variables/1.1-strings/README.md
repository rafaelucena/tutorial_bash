---
title: variables-strings-pt/br
---

## Strings
# Armazenando Strings em Variáveis em BASH

````bash
#exemplo 1
txt=Eita;
echo ${txt};
 
#exemplo 2
txt='Eita Giovana!';
echo ${txt};
 
#exemplo 3
txt='Giovana!';
txt="Eita ${txt}";
echo ${txt};
````

* Strings (textos) contendo símbolos ou espaços precisam estar encapsulados entre aspas para serem incorporados por uma variável

##### Nota1: Tecnicamente, tudo é String em BASH, mas vamos trabalhar específicamente com texto nessa parte

# Diferenças Entre Aspas Simples `'abc'` e Duplas `"abc"`

````bash
txt='assim';
txt='Aspas simples não funcionam ${txt} como as duplas!';
echo ${txt};
 
txt='assim';
txt="Aspas duplas funcionam ${txt} como magia negra!";
echo ${txt};
````

* Aspas simples são a forma mais prática de utilizar texto literal
* Aspas duplas são principalmente voltadas para utilizações de variáveis, funções dentro da própria string, etc

# Concatenando Strings

# Comparando Strings

# Localizando Strings

# Substituindo Strings

#### Mais Informações:
###### @TODO
<!-- Please add any articles you think might be helpful to read before writing the article -->
