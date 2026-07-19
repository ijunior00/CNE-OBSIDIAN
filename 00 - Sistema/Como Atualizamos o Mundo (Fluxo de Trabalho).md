---
tags: [sistema, tutorial]
aliases: [Fluxo de Trabalho, Workflow]
---

# 🔄 Como Atualizamos o Mundo a Partir das Conversas

Este é o coração do "segundo cérebro". Ele descreve como transformar nossas conversas (e as sessões jogadas) em notas organizadas aqui no vault.

## O ciclo

```
Você joga / conversa  →  me conta o que aconteceu  →  eu escrevo/atualizo as notas .md
        ↑                                                          ↓
   você puxa no Obsidian  ←──────── push pro GitHub  ←────────────┘
```

## O que me mandar

Quando quiser registrar algo, me diga em linguagem natural. Exemplos que eu sei processar:

- **"Rodamos a Sessão 2, aconteceu X, Y, Z."** → eu crio `02 - Sessões/Sessão 02 - ....md`, atualizo os personagens envolvidos, crio locais/NPCs novos e ligo tudo com `[[wikilinks]]`.
- **"O grupo capturou um Growlithe, dono é o Aiden."** → crio a nota do Pokémon e atualizo [[Aiden]].
- **"Criei um NPC novo: a líder de ginásio de Pewter, chama-se ..."** → crio a nota do NPC no template certo.
- **"Muda o objetivo do Kanye, agora ele também quer ..."** → edito a nota dele mantendo o resto.
- **"Revela que a Coroa de Ônix na verdade é ..."** → atualizo o artefato e marco como segredo.

## O que eu faço automaticamente

1. Escolho a pasta e o **template** corretos (ver [[Convenções do Vault]]).
2. Crio `[[wikilinks]]` entre tudo que se relaciona (personagem ↔ local ↔ sessão ↔ organização).
3. Marco **segredos do Mestre** com `> [!danger] SEGREDO DO MESTRE` e `tags: [spoiler]`.
4. Atualizo a [[Linha do Tempo]] quando um evento tem data/ordem.
5. Faço commit com mensagem descritiva e push para a branch do repositório.
6. Te aviso o que mudou.

## Boas práticas para não perder nada

- Depois que eu enviar, rode **Pull** no Obsidian (ver [[Como Conectar Obsidian ao GitHub]]).
- Se você editar bastante à mão, me avise para eu puxar sua versão antes de escrever por cima.
- Prefira me dar os fatos crus ("o quê, quem, onde"); eu cuido da formatação e das ligações.

## Ligações
- [[Como Conectar Obsidian ao GitHub]]
- [[Convenções do Vault]]
- [[🗺️ Mapa do Mundo (MOC)]]
