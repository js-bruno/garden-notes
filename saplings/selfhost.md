---
title: Self-hosting
aliases:
  - selfhost
  - self-hosting
  - self hosted
tags:
  - sapling
  - selfhost
description: Rodar seus próprios serviços em vez de depender de plataforma de terceiros.
---

Self-hosting é trocar o serviço de terceiros pela sua própria máquina. Em vez de
"subir um chat" num SaaS, você roda o [[self-hosted-habbo-server|servidor você
mesmo]].

## Por que importa neste jardim

O [[index|thisdev.notes]] inteiro é self-hosted: build no GitHub Actions, deploy
via `scp` pra um VPS, nginx servindo. O [[self-hosted-habbo-server|servidor de
habbo]] é o segundo serviço. A aposta declarativa do [[nix-os|NixOS]] é o jeito
mais barato de manter tudo isso reproduzível.

## Fricção honesta

Self-host tem custo real: atualizar, expor porta, cuidar de segurança. O oposto
de [[consume-less-produce-more]]? Não — é produção no nível de infraestrutura:
você deixa de ser consumidor do serviço e passa a operar o próprio.

See also: [[self-hosted-habbo-server]], [[nix-os]], [[docs.targetteal.com]],
[[thisdev-space]], [[index]]
