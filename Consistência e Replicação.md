# Consistência e Replicação

Replicação significa manter os mesmos dados em mais de um lugar. Ela pode melhorar a disponibilidade e a velocidade, mas cria o problema de manter as cópias atualizadas.

Na consistência forte, uma leitura deve enxergar a atualização mais recente. Na consistência eventual, as cópias podem ficar diferentes por algum tempo, mas tendem a convergir.

A escolha depende do problema. Um sistema de pagamentos precisa de mais garantias do que uma contagem de visualizações.

Relacionada a [[Falhas Distribuídas]], [[Consenso Distribuído]] e à [[Agenda - Sistemas Distribuídos]].
