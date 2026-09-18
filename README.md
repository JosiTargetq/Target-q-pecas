# Target-q-pecas

Hospedagem das **imagens das peças de marketing da Target-Q**, para que a ferramenta de
publicação (Postiz) consiga baixá-las por URL pública.

## Por que este repositório existe

O Postiz precisa de um **endereço público** para buscar a imagem sozinho. As peças são
geradas localmente (HTML + Chrome headless), então o arquivo nasce no computador, sem URL.
Este repositório dá o endereço.

Escolhido por ser **independente do que está mudando**: o site em WordPress sai do ar, o
site novo entra em Next.js/Vercel, e as URLs daqui continuam de pé.

## Organização

```
2026-09/          imagens prontas, por mês de publicação
_fontes/          o HTML que gerou cada peça (permite reeditar sem refazer)
```

## Como uma imagem vira URL

Arquivo `2026-09/exemplo.png` fica acessível em:

```
https://raw.githubusercontent.com/JosiTargetq/Target-q-pecas/main/2026-09/exemplo.png
```

⚠️ O endereço **respeita maiúsculas e minúsculas** — `Target-q-pecas` com T maiúsculo.

## Regras

- O repositório é **público** de propósito: privado faz o Postiz levar 403.
- Só imagens de peças de marketing. Nada pessoal, nada de cliente, nada sigiloso —
  qualquer pessoa com o link enxerga o conteúdo.
- O HTML fonte fica em `_fontes/`: mudar uma data é editar uma linha, não refazer a peça.
