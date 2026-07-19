---
tags: [sistema, tutorial]
aliases: [Sincronização, Setup Obsidian Git]
---

# 🔌 Como Conectar o Obsidian a este GitHub

O objetivo: este repositório vira uma pasta no seu computador; essa pasta é aberta como **vault do Obsidian**; um plugin sincroniza tudo com o GitHub automaticamente. Assim, o que eu (Claude) escrevo aqui aparece pra você, e o que você escreve volta pra cá.

## Opção A — Plugin **Obsidian Git** (recomendado)

Melhor para uso no computador. Sincroniza sozinho a cada X minutos.

1. **Instale o Git** no computador → https://git-scm.com
2. **Clone o repositório** para onde quiser guardar o vault:
   ```bash
   git clone https://github.com/ijunior00/CNE-OBSIDIAN.git
   ```
3. No Obsidian: **Open folder as vault** → escolha a pasta `CNE-OBSIDIAN` clonada.
4. **Settings → Community plugins → Turn on community plugins.**
5. **Browse → procure "Obsidian Git" → Install → Enable.**
6. Em **Settings → Obsidian Git**, sugestão de configuração:
   - *Vault backup interval (minutes):* `10` (faz commit+push automático)
   - *Auto pull interval (minutes):* `10` (puxa o que eu enviei)
   - *Pull updates on startup:* ligado
   - *Commit message:* `vault backup: {{date}}`
7. Pronto. Comandos úteis (paleta `Ctrl/Cmd + P`):
   - `Obsidian Git: Pull` → baixa minhas atualizações agora
   - `Obsidian Git: Commit-and-sync` → envia as suas agora

> [!tip] Fluxo diário
> Antes de escrever, rode **Pull** (pega o que fiz). Ao terminar, **Commit-and-sync** (envia o seu). Com os intervalos automáticos ligados, quase nunca precisa fazer manual.

## Opção B — Celular (Obsidian Mobile + Obsidian Git)

Funciona, mas é mais chato. O plugin Obsidian Git roda no mobile; siga o mesmo passo a passo do plugin. Alternativa mais simples no celular: usar o app do **GitHub** só para ler, e editar no computador.

## Opção C — Sem plugin (manual)

Se não quiser plugin: edite no Obsidian normalmente e, pelo terminal na pasta do vault:
```bash
git pull        # pega minhas atualizações
git add . && git commit -m "minhas notas" && git push   # envia as suas
```

## Evitando conflitos

- **Sempre dê `Pull` antes de editar.** Se nós dois mexermos no mesmo arquivo ao mesmo tempo, o Git pode gerar conflito.
- Se aparecer conflito, o arquivo mostra blocos `<<<<<<<` / `=======` / `>>>>>>>`. Escolha o texto certo, apague os marcadores, salve e sincronize de novo.
- Regra prática: quando você me pedir para atualizar algo, **não edite esse mesmo arquivo ao mesmo tempo**; me deixe enviar e depois puxe.

## Ligações
- [[Como Atualizamos o Mundo (Fluxo de Trabalho)]]
- [[Convenções do Vault]]
- [[🗺️ Mapa do Mundo (MOC)]]
