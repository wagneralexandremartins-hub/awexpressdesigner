---
name: alteracao-comercial
description: Use para alterar preços, prazos ou textos comerciais do site AWEXPRESS Designer (index.html). Só vale com autorização direta do Wagner no pedido; termina sempre em PR, nunca em push na main.
---

Responda sempre em português do Brasil, de forma direta e sem listas excessivas.

## Quando usar
Quando o Wagner pedir mudança de preço, prazo, promessa ou qualquer texto comercial do site. Se o pedido não trouxer o texto ou valor exato, pergunte antes de mexer.

## Regras fixas
- Mude somente o que foi pedido. Não altere design, cores, fontes, estrutura nem outros textos.
- Nunca faça push direto na main nem merge. O Wagner revisa e faz o merge pelo GitHub.
- Não coloque nada sensível neste repositório público: sem chaves, sem dados de clientes, sem relatórios de auditoria.
- Não altere conteúdo editorial cristão sem autorização explícita.

## Passos
1. Rode git status. Se houver alteração não salva, pare e avise o Wagner antes de continuar.
2. Atualize a main (git checkout main e git pull) e crie uma branch nova com nome conteudo/AAAA-MM-DD-assunto.
3. Faça a alteração pedida, preservando as tags e classes existentes. Em preços, use &nbsp; entre "R$" e o número para o símbolo não se separar do valor.
4. Procure no index.html outras menções ao mesmo valor ou prazo (meta description, og, twitter, JSON-LD, FAQ, textos soltos) e liste para o Wagner, sem alterar sem autorização.
5. Confira o resultado em desktop e celular (por exemplo 1440, 1280, 1024, 768, 390 e 360 px): nada quebra linha de forma feia, não aparece rolagem horizontal e o texto novo fica legível.
6. Mostre o diff ao Wagner e espere a autorização dele para o commit.
7. Com autorização, faça o commit na branch, envie a branch e abra o PR. A descrição do PR deve ter uma tabela antes/depois, as outras menções encontradas e o que não foi alterado. Avise se algum limite ou valor máximo foi removido.
8. Pare no PR. Lembre o Wagner de que texto comercial ou cláusula nova deve passar pelo advogado ou contador antes do merge, e que o GitHub Pages leva cerca de 10 minutos para publicar.
