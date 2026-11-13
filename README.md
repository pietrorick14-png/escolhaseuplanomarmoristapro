# Escolha seu plano · Marmorista Pro

Página única (`index.html`), sem build. É o passo que vem depois da VSL: a pessoa escolhe o plano (PRO ou PRO Equipe),
escolhe a forma de pagamento (cartão ou Pix, mensal ou anual) e vai direto pro checkout da Stripe.

Preços de Black Friday (ancoragem + gatilho de escassez). Os valores batem com os reais da função `compra-site` do app —
se o preço mudar lá, mude aqui também (`PL` dentro do `<script>`).

## Publicar na Cloudflare

**Opção 1 — Workers & Pages → Criar → Pages → Conectar ao Git**
- Repositório: `escolhaseuplanomarmoristapro`
- Framework: nenhum
- Comando de build: (vazio)
- Pasta de saída: `/`

**Opção 2 — linha de comando**
```
npx wrangler deploy
```

Depois de publicar, coloca o link do domínio direto no botão de CTA do VTurb (na VSL).
