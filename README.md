[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/7EVNAYx2)
# ClientServerBasics (2.0)
Starter code for the basic client-server assignment


Este template corresponde ao exemplo da Fig. 2.3 do livro. O exercício consiste em acrescentar funcionalidade ao servidor para torná-lo mais útil. Essa funcionalidade deve ser acessível aos clientes. Por exemplo, o servidor pode ser uma espécie de calculadora remota. O cliente passa dois valores numéricos, juntamente com o nome de uma operação (ex.: add, subtract, multiply, divide) e o servidor executa a operação respectiva e retorna seu resultado para o cliente. Você pode implementar um servidor com outras funcionalidades (diferente da calculadora). O imporante é que ele ofereça pelo menos três operações diferentes que os clientes podem utilizar remotamente, passando dados para serem processados e recebendo o resultado desse processamento como resposta.

Tarefa individual.

Incluir um Readme descritivo do sistema implementado.
# Client-Server com Sockets TCP

Este projeto implementa um sistema cliente-servidor em Python utilizando sockets TCP.

O código foi baseado no exemplo visto em aula e foi modificado para permitir maior processamento no servidor e múltiplas funcionalidades para o cliente.

## Funcionalidade

O servidor funciona como uma calculadora remota.  
O cliente envia uma operação e dois valores, e o servidor retorna o resultado.

## Operações disponíveis

- add (soma)
- sub (subtração)
- mul (multiplicação)
- div (divisão)
- pow (potência)

## Formato das requisições

As mensagens seguem o formato:

operacao;valor1;valor2

Exemplo:
add;10;5

## Como executar

1. No arquivo constCS.py, configure:

Para execução local:
HOST = '127.0.0.1'

2. Execute o servidor:
python server.py

3. Em outro terminal, execute o cliente:
python client.py

## Observações

- O servidor trata erros como divisão por zero e operações inválidas
- O cliente pode fazer várias requisições na mesma conexão

## Autor

Matheus Felipe de Borba Machado Vieira
