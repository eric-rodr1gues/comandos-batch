# Comandos batch
---
**Descrição do Script**

O script foi feito para funcionar como um calendário, onde ao escrever qualquer ano e mês, ele mostrará o dias do mês que for pedido, e falará se o ano é bissexto ou não. O comando fará um cálculo para descobrir se o ano é bissexto ou não, caso o ano seja bissexto, será enviado um recado que mostrará quando será o próximo ano bissexto. Ao pedir as datas, o script vai criar pastas e diretórios dos anos, meses e dias que forem solicitados.

---
**Explicação do código**

- ```set```: As variáveis são espaços que recebem e armazenam dados que podem ser usados ao longo do script. O comando para se criar uma variável é o "set". Exemplo:

```set dias=31```

Assim uma variável com o valor de 31 foi criada, podendo ser usada ao londo do script.

- ```if```: Esse comando executa processos condicionais no programa. No caso desse script o comando é:

```if not exist %1 ( mkdir %1 )```

Ou seja, o comando verificará se a variável "%1" já existe, caso ela não exista, será criada.

- ```else```: O comando "else" acompanha o comando "if" e, assim como ele, é um comando condicional e serve como um caminho alternativo do if. Por exemplo: 

if %resto%==0 (
    set fevereiro=29
    echo o proximo ano bissexto e %bissexto%
) else (
    set fevereiro=28
)

Assim, caso o comando "if", não aconteca, o comando "else" será executado e criará a variável "fevereiro" de valor 28.

- ```for```: O comando "for" serve para repetir uma instrução ou um conjunto de instruções em um número determinado de vezes. Exemplo:

for /L %%D in (1,1,%dias%) do (
    if not exist %%D (
        mkdir %%D
    )
)

Logo, o comando "for" repete a instrução de começar com o valor 1, ir aumentando de 1 em 1 até que chegue no número de dias que é determinado pela variável "%dias%". E se caso não exista a variável "%%D", uma será criada.

---
**Desafios e Soluções**

Durante o processo de fazer o script, pessoalmente, foi bem desafiador para conseguir entender como cada comando funcionava e a função deles exatamente, também foi difícil escrever os comandos do jeito correto e de modo que tudo funcionasse em harmonia e corretamente. Mas consegui solucionar esses problemas perguntando aos professores e colegas como cada parte funciona.

---
**Possíveis Melhorias**

Em questão de melhorias, algo que deve ser aprimorado é a questão do cálculo dos anos bissextos, pois os cálculos têm dado errado, então é uma melhoria que precisa ser feita.  

---
**O que aprendi**

Aprendi novos comandos que são o: if, for, else e set. Aprendi como criar e usar variáveis, resolver problemas, melhorei também meu raciocínio lógico, aprendi a colocar cáculos dentro do código e a criar meu próprio calendário por meio de pastas e diretórios. 
