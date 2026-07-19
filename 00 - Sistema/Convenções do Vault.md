---
tags: [sistema]
aliases: [Convenções, Padrões]
---

# 📐 Convenções do Vault

Padrões que eu sigo ao escrever, para o vault ficar consistente e navegável.

## Frontmatter (metadados no topo)

Toda nota começa com um bloco `---` contendo `tags` e, quando útil, `aliases` e `status`.

## Tags principais

| Tag | Uso |
|---|---|
| `protagonista` | Os 4 personagens dos jogadores |
| `npc` | Personagens não-jogáveis |
| `organização` | Grupos (CNE, etc.) |
| `local` | Cidades, rotas, instalações |
| `pokémon` | Notas de Pokémon |
| `item` | Itens e artefatos |
| `quest` | Missões e ganchos |
| `sessão` | Registros de sessão |
| `spoiler` | Contém segredo do Mestre |
| `sistema` | Notas sobre o próprio vault |

## Ligações (`[[wikilinks]]`)

Sempre que uma nota menciona outra entidade que tem (ou deveria ter) nota própria, eu ligo com `[[Nome da Nota]]`. Isto alimenta o **Graph View** do Obsidian — é o que faz o mundo parecer "vivo".

## Segredos do Mestre

Informação que os jogadores ainda não deveriam saber fica dentro de um callout:

```
> [!danger] SEGREDO DO MESTRE
> A CNE significa Coroa Negra Eterna...
```

E a nota recebe `tags: [..., spoiler]`.

## Callouts que uso

- `> [!info]` contexto público
- `> [!quote]` falas e citações
- `> [!danger] SEGREDO DO MESTRE` verdade oculta
- `> [!tip]` dica de mesa para o Mestre
- `> [!todo]` fios em aberto / a decidir

## Nomes de arquivo

- Pastas com prefixo numérico (`01 - Campanha`) para ordenar.
- Sessões: `Sessão NN - Título.md`.
- Quando um Pokémon pertence a alguém, incluo entre parênteses: `Machop (Kanye).md`.

## Templates

Ficam em `00 - Sistema/Templates/`. Configure o plugin **Templates** (core) do Obsidian apontando para essa pasta para criar notas novas rapidamente.

## Ligações
- [[Como Atualizamos o Mundo (Fluxo de Trabalho)]]
- [[🗺️ Mapa do Mundo (MOC)]]
