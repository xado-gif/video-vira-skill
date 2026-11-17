# video-vira-skill

Vídeos do YT viram uma skill no Claude.AI, focado no Claude Chat, onde o uso é gratuito.

O Gemini assiste ao vídeo, o Claude audita e escreve o `spec.md` e a skill em texto.
Sem Claude Code e sem plano pago.

## Conteúdo

- `docs/guia.html`: guia interativo (checklist, botões de copiar, tema claro/escuro). Abra no navegador.
- `kit-yt-gratuito.md`: o mesmo fluxo em texto, com prompts e comandos.

## Fluxo

1. O Gemini assiste ao vídeo e lista os passos com timestamps.
2. Legenda do YouTube, mais frames dos momentos-chave (opcional).
3. O Claude cruza as fontes e gera o `spec.md` com status por passo
   (confirmado, fonte única, conflito).
4. Você resolve os conflitos.
5. O Claude escreve o `SKILL.md`.

## Créditos

Baseado na skill `watch` de [bradautomates/claude-video](https://github.com/bradautomates/claude-video)
(licença MIT). Este projeto é independente e não é afiliado a ele.

## Cuidados

- O link do vídeo é enviado ao Google no motor Gemini. Para vídeo privado, use só o modo local.
- Nunca coloque chaves de API no repositório. A chave fica em `~/.config/watch/.env`.
- Limites e preços do plano gratuito do Gemini mudam: confira no AI Studio.
