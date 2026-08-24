# AWEXPRESS Designer — Diretrizes do Projeto

Site institucional da AWEXPRESS Designer (Adriana & Wagner), publicado em https://awexpressdesigner.com.br/.

## Regras invioláveis

- **Site 100% estático** — HTML/CSS/JS puro (tudo em `index.html`). Não introduzir frameworks pesados (React, Vue, build tools, bundlers, etc.).
- **Identidade visual fixa** — manter sempre a paleta cobalto/âmbar (`--cobalt`, `--cobalt-glow`, `--amber`, `--amber-glow` já definidos em `:root`) e a tipografia Sora (headings) / Inter (corpo) / JetBrains Mono (kickers/labels). Não trocar fontes nem paleta.
- **Nunca reconstruir o site do zero** sem autorização explícita do Wagner. Alterações são sempre incrementais sobre o que já existe.
- **Hospedagem: GitHub Pages** — o domínio é apontado via `CNAME`. Não usar Vercel, Netlify ou qualquer outra plataforma para este projeto.
- **Preços e conteúdo comercial** (planos, valores, textos de posicionamento/venda) só podem ser alterados mediante aprovação direta do Wagner. Não mudar preços por conta própria.

## Fluxo de trabalho

- **Sempre validar visualmente (desktop + mobile) antes de sugerir commit.** Preferir checagem de geometria real via DOM (`getBoundingClientRect`, scan de overflow) além de screenshot, já que capturas headless neste ambiente podem ter inconsistências de escala/viewport.
- **Sempre perguntar antes de fazer commit e push.** Nunca commitar/enviar automaticamente sem confirmação explícita do usuário na conversa.
- Preservar todo conteúdo, seções, projetos e serviços já existentes — não remover nada sem necessidade clara.
- Ao adicionar algo novo, reaproveitar componentes/classes CSS já existentes sempre que possível, em vez de criar estilos redundantes.
