# Falhas Distribuídas

Em um sistema distribuído, uma parte pode falhar enquanto as outras continuam funcionando. Isso é chamado de falha parcial.

Alguns exemplos:

- uma máquina fica fora do ar;
- uma mensagem demora muito;
- a resposta chega duas vezes;
- a conexão cai depois que o pedido foi enviado.

Por isso, é importante pensar em timeout, retry e idempotência. Repetir uma operação só é seguro quando fazê-la duas vezes não causa um efeito inesperado.

Esta nota se conecta ao [[Sistema Distribuído]] e à [[Agenda - Sistemas Distribuídos]].
