---
title: Nix OS
aliases:
  - NixOS
  - nix-os
tags:
  - find/article
  - nix
  - linux
  - selfhost
description: NixOS — distribuição Linux baseada no gerenciador de pacotes Nix.
---

NixOS e uma distribui'cao linux do balacubaco, baseado em um gerenciado de pacote chamado [[nix]]. Ele usa o principio de desing [atomic update model](https://www.howtogeek.com/what-is-an-immutable-linux-distro/), que facilita manutenibilidade do OS e a seguranca em questao de estabilidade.

A sua grande questao e forma de se instalar e configurar os pacotes, por meio do package-manager nix e uma linguagem de programacao declarativa.

[[home-manager]]

## Por que importa

É a mesma aposta declarativa do [[astral_python]] (dois binários substituindo uma
pilha de scripts), só que no nível do sistema operacional inteiro. Configuração
como código, upgrade reversível, e o ambiente reproduzível de máquina a máquina.

See also: [[nix]], [[home-manager]], [[self-hosted-habbo-server]], [[nix-livestream]], [[internet-finds]]
