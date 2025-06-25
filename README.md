# ULA-8-BITS

1. Apresentação
   
O projeto visa desenvolver uma ULA de 8 bits capaz de realizar operações
aritméticas (como adição e subtração) e lógicas (como AND, OR, NOT e XOR). A
ULA será utilizada para simular o funcionamento básico de um processador,
servindo como base para o aprendizado de arquitetura de computadores e sistemas
digitais. Sua aplicação se estende a projetos simples de hardware e ao ensino
prático de lógica digital.
-Unidade de Operações Aritméticas (UA) que realiza operações de: o Adição; o
Subtração; o Transferência; o Incremento; o Decremento;
-Unidade de Operações Lógicas (UL) que realiza operações de: o AND o OR o
NAND o NOR o NOT o XOR o XNOR o CMP
-Processamento de flags para sinalizar o resultado das operações: o Carry (C) o
Overflow (V) o Negative (N) o Zero (Z).

2. Projeto
   
Etapas para o projeto:
a) Explicar a implementação da Unidade Aritmética:
A Unidade Aritmética foi implementada utilizando somadores completos (full adders)
encadeados para operar sobre dois operandos de 8 bits. A subtração é feita por
meio do complemento de dois: invertem-se os bits do segundo operando e
soma-se 1. Um sinal de controle define se a operação será soma ou subtração.
O carry-out é utilizado para verificar overflow.
b) Explicar a implementação da Unidade Lógica:
A Unidade Lógica foi construída com portas lógicas básicas (AND, OR, XOR, NOT).
Um multiplexador de 4 entradas escolhe qual operação lógica será executada,
de acordo com os sinais de controle. Cada operação atua bit a bit sobre os
operandos A e B (8 bits).
c) Explicar a implementação dos teclados, LEDs, displays e sinais de sincronismo.
Teclados: Utilizados para inserir os operandos e a operação desejada. Leitura feita
por varredura (scanning), onde linhas e colunas são ativadas sequencialmente.
LEDs: Mostram o resultado das operações em tempo real, com cada LED
representando um bit da saída.
Displays de 7 segmentos: Exibem os valores inseridos e o resultado em formato
decimal ou hexadecimal.
Sinais de sincronismo: Um clock principal controla o tempo de leitura dos teclados e
a atualização das saídas, garantindo que os dados sejam processados de forma
ordenada e sem ruído.
