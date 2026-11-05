# F1 Drinks — Site de pedidos (prévia)

Proposta de site de pedidos para a **F1 Drinks**, delivery de bebidas em Santos – SP.
Prévia não oficial, criada por Guilherme Greg ([@gframe](https://instagram.com/gframe)) para apresentar à loja.

**Ver online:** https://greghi-ai.github.io/f1drinks/

## O que o site faz

- Capa com fotos dos produtos e etiquetas de preço clicáveis
- "Os mais pedidos" em destaque e letreiro de promoções
- **Monte seu combo:** o cliente escolhe a garrafa e o acompanhamento (Red Bull, Bally, Energético 2L)
- Cardápio completo (250+ itens) com busca e categorias
- Sacola com aviso de pedido mínimo (R$ 20)
- Finalização em 3 etapas (dados, entrega, pagamento: Pix, cartão online, cartão na entrega ou dinheiro), que gera a mensagem do pedido e abre o WhatsApp da loja
- Status "aberto/fechado" pelo horário de Brasília (13h–23h59)

Tudo fica em um único arquivo (`index.html`): HTML, CSS, JavaScript e imagens. Não precisa de servidor nem de banco de dados.

## Como publicar no GitHub Pages (grátis)

1. Crie um repositório **público** no GitHub (ex.: `f1drinks`).
2. Envie o `index.html` e este `README.md` (botão **Add file → Upload files**).
3. Vá em **Settings → Pages**.
4. Em **Build and deployment**, escolha **Deploy from a branch**, branch `main` e pasta `/ (root)`. Clique em **Save**.
5. Em 1 ou 2 minutos o site aparece em `https://greghi-ai.github.io/f1drinks/`.

## Como editar

- **Preços e produtos:** no `index.html`, procure por `const P = [`. Cada linha é um produto:
  `["categoria","Nome","descrição",preço,preçoAntigo,"tags",esgotado]`
  Tags: `p` = promoção, `t` = mais vendido, `n` = novidade, `a` = +18. Coloque `1` no final para marcar como esgotado.
- **Destaques da capa:** procure por `const FEAT=`.
- **WhatsApp da loja:** procure por `const WA=`.
- **Pedido mínimo:** procure por `MIN=`.
