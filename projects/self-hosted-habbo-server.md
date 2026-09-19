---
title: Servidor Self Hosted De Habbo
aliases:
  - self-hosted-habbo-server
  - Servidor Habbo
tags:
  - project
  - selfhost
  - habbo
description: Subir um servidor privado de Habbo Hotel completo — emulador, CMS e client.
---

## O Que eu estava procurando

A mais ou menos a pouco tempo venho procurando algum servico para usar de chat fora da caixa e lembrei que em 2016 exista varias copias piratas de habbo hotel, mas era o jogo up em um servidor privado onde a comunidade implementava dinheiro infinito e divesas outras coisas que nao exisitam no habbo original, como mods e etc.

Fazendo uma pesquisa  encontrei um repositorio que sobe o codigo do jogo em java chamado [Morningstar](https://git.krews.org/krews/Morningstar) esse repo e responsavel pelo servidor do jogo, conexoes e etc para ter o servico do habbo completo precisamos do
portal de login com gerenciamento de contas e etc (cms) e o client que rodara o jogo no navegado.


Alternativamente eu quero fazer um tela de login rapido, algo como um convite http que carregue o cadastro de usuario mais rapidamente
onde aparece o nome do usuario e o avatar ele imediatamente e teleportado a pra sala onde estou.

## Desenvolvimento e deploy

O Servidor onde o jogo roda e o [ Arcturus Morningstar ](https://git.krews.org/krews/Morningstar)

## As três peças

O texto acima já identifica que "habbo completo" não é um serviço, são três:

| Peça | Função | Estado |
|---|---|---|
| **Emulador** | servidor do jogo, conexões, lógica de sala | Arcturus Morningstar (Java) |
| **CMS** | portal de login, cadastro, gerenciamento de contas | — |
| **Client** | o que roda o jogo no navegador | — |

> [!question] gap
> Qual CMS? Qual client? A nota nomeia o emulador duas vezes mas deixa as outras
> duas peças em aberto — e é nelas que o deploy trava.

> [!question] gap
> "convite http que carregue o cadastro de usuario mais rapidamente" — isto é
> auth por token mágico (link único que cria/loga a conta). Precisa decidir:
> token assinado ou sessão descartável? Expiração?

## Por que este projeto importa pro jardim

É o único item do vault que chega em **Create** na [[method|Bloom's Taxonomy]] —
todo o resto está em `Remember` ou `Understand`. E é o candidato natural a
*"talk while you code"* do swyx: build log escrito como ensino, não como diário.

Também é [[selfhost]] de verdade, o que conecta com [[nix-os]] e [[nix-livestream]].

See also: [[method]], [[nix-livestream]], [[selfhost]], [[now]]
