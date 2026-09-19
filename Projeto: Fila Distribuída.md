# Projeto: Fila Distribuída

O projeto será uma fila simples com dois processos:

- um produtor envia tarefas;
- um consumidor busca e processa tarefas.

## Etapas

1. Fazer produtor e consumidor conversarem.
2. Guardar tarefas em uma lista.
3. Adicionar confirmação de recebimento.
4. Simular a queda do consumidor.
5. Adicionar retry sem processar a mesma tarefa duas vezes.
6. Escrever o que funcionou e o que falhou.

O objetivo não é criar uma fila pronta para produção. É observar na prática os problemas descritos em [[Falhas Distribuídas]].

O projeto acompanha a [[Agenda - Sistemas Distribuídos]] e será publicado usando a rotina de [[Aprender em Público]].
