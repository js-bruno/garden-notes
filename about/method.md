---
title: Method
aliases:
  - method
  - o método
description: Como este jardim funciona — Feynman + Knowledge Flow + Learn In Public.
tags:
  - fruit
  - learning-in-public
  - meta
---

Este jardim não é um fichário. Um fichário otimiza **acesso**; um jardim otimiza
**generatividade**. A diferença prática: no fichário você guarda o que já sabe,
no jardim você planta o que ainda não sabe pra descobrir o que é.

Três métodos combinados, mais quatro camadas de suporte.

---

## 1. Feynman Technique — o motor de cada nota

Atribuída a Richard Feynman, popularizada por Scott Young em *Ultralearning*.

| Passo | O que fazer | Sinal de que funcionou |
|---|---|---|
| **1. Ensine** | Explique o conceito como se o leitor fosse inteligente mas nunca tivesse visto aquilo. Sem jargão. | Você não usou nenhuma palavra que não saberia definir |
| **2. Ache o gap** | Onde você travou, disse "basicamente", ou usou termo técnico pra não explicar — **isso é o seu gap real**. Volte à fonte. | Você tem uma lista concreta do que não sabe |
| **3. Simplifique** | Crie uma analogia. | Se não consegue construir analogia, ainda não entendeu |
| **4. Refine ensinando** | Publique, grave, explique em voz alta. | Alguém de fora conseguiu reproduzir |

**O passo 2 é o que faz disto um método de ensino e não só tomada de notas.**
Jargão é o esconderijo da ignorância — ele te deixa *sentir* que explicou sem
ter explicado. A técnica te tira do esconderijo à força.

Neste jardim, gaps são marcados com:

```markdown
> [!question] gap
> o que especificamente eu não sei
```

Eles ficam **visíveis e não preenchidos**. Preencher o gap pelo autor seria
destruir o método.

Molde: `templates/feynman-note.md`

---

## 2. Knowledge Flow — o formato do vault

Vocabulário direto de [*Networked Thought*](https://jzhao.xyz/posts/networked-thought),
do autor do Quartz. Adotar a linguagem da ferramenta faz o jardim se explicar sozinho.

```
seeds/      🌱  captura. fricção ~zero. 1-3 linhas. perguntas são bem-vindas
   ↓
saplings/   🌿  um conceito por nota. passagens Feynman 1-3. ainda não ensinável
   ↓
fruits/     🌳  acabado, ensinável, publicável. ensaios longos, coisas maduras
```

Mais duas pastas que não são estágio:

```
projects/         build logs com começo, meio e fim
logs/             learning logs, TIL, revisão semanal, /now
internet-finds/   catálogo do que vem de fora — o único silo temático legítimo
about/            o próprio jardim
```

### Por que estágio e não tópico

Tópico em pasta cria **silo**, e silo mata conexão cruzada — que é o único
motivo pra um jardim existir em vez de um Notion. jzhao é explícito:

> There is way too much upfront friction that by the time I've thought about how
> to organize my thought into folders categories, I've lost it.

Estágio em pasta não cria silo: diz o quão cozida está a ideia e nada mais.
**Tópico vem de tags + wikilinks + MOCs**, que são muitos-para-muitos e não
exclusivos.

Mover arquivo de `seeds/` pra `fruits/` não quebra URL: `alias-redirects` está
ativo e o frontmatter aceita `permalink`.

---

## 3. Learn In Public — a prática

Do [ensaio canônico do swyx](https://www.swyx.io/learn-in-public).

- **Learning exhaust.** Crie o *hábito* de excretar aprendizado. Blog, tutorial,
  cheatsheet, vídeo, TIL. O formato importa menos que a regularidade.
- **Escreva pra você de 3 meses atrás.** Não pra audiência. Não meça por clap,
  star ou upvote. *"by far the biggest beneficiary of you trying to help past
  you is future you."*
- **Make the thing you wish you had found.**
- **Talk while you code.** Os melhores processos seletivos dele foram os que ele
  falou *como professor* em vez de tentar provar algo.
- **Try your best to be right, but don't worry when you're wrong.** Use a
  noobice na manga. Deixe a internet te corrigir.
- **Pick up what they put down.** Quem te corrige virou seu mentor de graça.

Isto já estava em [[learning-in-public]] antes desta nota existir — o que é
evidência de que o método foi descoberto, não importado.

---

## 4. Camadas de suporte

### Bloom's Taxonomy — o diagnóstico
1956, revisada por Anderson & Krathwohl em 2001:

```
Create  →  Evaluate  →  Analyze  →  Apply  →  Understand  →  Remember
```

Serve pra saber **onde** uma nota está. No estado inicial este vault era ~95%
`Remember` (35 stubs de sites com uma URL e uma frase). `projects/` é `Create` —
o topo. O método existe pra te empurrar pra cima da pirâmide.

### Protégé Effect — por que ensinar funciona
Chase, Chin, Oppezzo & Schwartz (2009), *Teachable agents and the protégé effect*:
estudantes que ensinavam um agente aprendiam mais do que os que só estudavam.
Base empírica pra escrever **sempre** em modo professor, mesmo sem leitor.

### Active recall / spaced retrieval — por que revisar funciona
Ebbinghaus (curva do esquecimento); Roediger & Karpicke (2006), *test-enhanced
learning*. Testar a si mesmo supera reler.

**Reler não conta.** Reler é reconhecer, e reconhecer não é saber.

Ritual: semanalmente, escolha 3 saplings, tente re-explicar **sem abrir**, só
então compare. O que falhou volta pra fila.

### Gibbs' Reflective Cycle — a estrutura do log
1988: Description → Feelings → Evaluation → Analysis → Conclusion → Action Plan.

Os 5 passos de [[learning-in-public]] são uma versão comprimida disso:

1. O que você queria fazer
2. O que você tentou
3. O que deu errado
4. O que resolveu o problema
5. O que você ainda não entendeu

O passo 5 é o que conecta de volta ao Feynman passo 2. **O ciclo fecha aí.**

Molde: `templates/learning-log.md`

### Zettelkasten — o que se aproveita e o que se rejeita
Aproveita: **atomicidade** (um conceito por nota), **palavras próprias**,
**links densos**.

Rejeita: o sistema formal completo (numeração, índices hierárquicos, categorias
fixas). Motivo idem ao de jzhao sobre Notion — fricção upfront mata a ideia antes
de ela existir.

---

## 5. Regras de conexão

Do próprio jzhao, as três que ele destaca depois de um ano de jardim:

1. **Link por conceito, não por match exato.** Use `See also:` quando dois
   assuntos estão associados mas não são a mesma coisa. Conectar conhecimento
   novo a conhecimento velho é o que faz lembrar.
2. **Nomeie notas o mais simples possível.** Substantivos ou verbos. Nomes
   curtos são mais fáceis de linkar.
3. **Busca boa importa.** Você busca justamente quando *não* sabe o nome exato.
   Busca é porta de entrada num nó; daí você recalled por associação, não por índice.

Regra adicional deste jardim: **toda nota nova sai com no mínimo 2 wikilinks.**
Nota sem link de saída é nota que o grafo não vê.

---

## 6. O ciclo completo

```
   consome algo
        │
        ▼
   seeds/  ────────────── captura sem fricção, pode ser só uma pergunta
        │
        ▼
   saplings/  ─────────── Feynman 1: ensina sem jargão
        │                 Feynman 2: acha o gap  →  [!question] gap
        │                 volta à fonte
        │                 Feynman 3: analogia
        ▼
   fruits/  ───────────── Feynman 4: ensina de verdade (publica / grava)
        │
        ▼
   logs/  ─────────────── revisão semanal, active recall
        │
        └───────────────▶ o que falhou volta pra fila
```

E em paralelo, `projects/` é onde Bloom chega em `Create` — o [[self-hosted-habbo-server]]
é o primeiro.

---

## Fontes

- Richard Feynman / Scott Young, *Ultralearning* (2019) — técnica Feynman
- Jacky Zhao, [*Networked Thought*](https://jzhao.xyz/posts/networked-thought) (2021) — seeds/saplings/fruits
- Jacky Zhao, [*Philosophy of Quartz*](https://quartz.jzhao.xyz/philosophy) — rizoma vs. árvore
- Maggie Appleton, *The Garden and the Stream* — jardim como topologia
- swyx, [*Learn In Public*](https://www.swyx.io/learn-in-public) (2018)
- Anderson & Krathwohl, *A Taxonomy for Learning, Teaching, and Assessing* (2001)
- Chase, Chin, Oppezzo & Schwartz, *Teachable agents and the protégé effect* (2009)
- Roediger & Karpicke, *Test-Enhanced Learning* (2006)
- Graham Gibbs, *Learning by Doing: A Guide to Teaching and Learning Methods* (1988)

See also: [[learning-in-public]], [[consume-less-produce-more]], [[index]],
[[internet-finds]], [[now]]
