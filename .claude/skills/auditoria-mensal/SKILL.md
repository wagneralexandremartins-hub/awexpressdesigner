---
name: auditoria-mensal
description: Rodar a auditoria mensal de manutenção do site AWEXPRESS Designer (segurança, SEO, desempenho, acessibilidade e links), só de leitura, sem alterar nada até eu autorizar.
---

# Auditoria mensal do site AWEXPRESS Designer

Regras: só leitura. Não alterar código, textos, preços, layout nem publicar nada. Seguir o CLAUDE.md do projeto. Qualquer correção só depois de autorização explícita, em branch nova, e commit/push só com autorização.

Passos:
1. Conferir o estado do repositório (git pull, git log recente) e se o index.html mudou desde a última auditoria.
2. Links: testar os links externos do portfólio e de WhatsApp (resposta HTTP e redirecionamentos) e as âncoras internas.
3. SEO: title (50-60 caracteres), meta description (até ~158), canonical, robots.txt, sitemap.xml, JSON-LD válido, Open Graph.
4. Acessibilidade: hierarquia de títulos, foco por teclado, contraste, menu mobile com aria-expanded, alt em imagens.
5. Desempenho: peso do HTML, recursos externos (fontes), animações pesadas no celular.
6. Segurança do front-end: nenhuma chave secreta no código, links com rel="noopener noreferrer", sem dados pessoais expostos além dos contatos públicos do negócio.
7. Formulário: validar (sem enviar de verdade) telefone curto, e-mail inválido e mensagem sem serviço.
8. Comparar com o relatório anterior e listar o que é novo, o que foi corrigido e o que continua pendente.

Entrega: relatório curto por prioridade (alto, médio, baixo), com evidência e sugestão, e a pergunta do que posso aplicar.
