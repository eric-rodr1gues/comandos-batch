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

- ```else```: O comando "else" acompanha o comando "if" e, assim como ele, é um comando condicional. 
