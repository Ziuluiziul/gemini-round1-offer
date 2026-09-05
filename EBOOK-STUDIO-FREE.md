# Ebook — Google AI Studio free-tier, feito pra vender

**Recebedor PIX:** LUIZ · Contato: z99003303@gmail.com  
**Landing:** https://ziuluiziul.github.io/gemini-round1-offer/  
**Hub:** https://ziuluiziul.github.io/round1-cumulunimbus/  
**Docs oficiais:** https://ai.google.dev/gemini-api/docs · https://ai.google.dev/gemini-api/docs/rate-limits · https://aistudio.google.com/rate-limit

## 1. O que é o free-tier (sem inventar cotas)

- Cotas **vivas** estão no AI Studio (`/rate-limit`), não em RPM inventado.
- Docs de rate-limits mandam consultar o Studio por projeto.
- Reset de RPD: meia-noite Pacific (conforme docs/Studio).
- Billing pago **só** com autorização do Luiz.

## 2. Operação segura (swarm / agente)

1. Abrir Studio rate-limit antes de volume.
2. **1** `generateContent` em voo por modelo.
3. Pular IDs **OVER** (ex.: Flash 3.5/3.6/3.7 e Lites estourados nesta conta).
4. Preferir IDs com folga (ex.: `gemini-3.8-flash`, Gemma 4) — só se a UI mostrar headroom.
5. `429` → `Retry-After` / backoff; `503` → backoff + outro ID com folga.
6. API exhausted → **Gemini chat web**; continue vendendo.

## 3. Pacotes desta oferta

| SKU | Preço | Entrega |
| --- | ---: | --- |
| Copy brief (3 variações) | R$ 20 | markdown no dia útil |
| Playbook ATLAS + checklist | R$ 50 | markdown + checklist |
| Pack 5 prompts (este ebook) | tip / upsell | markdown nesta Pages |
| Mini-curso copy | tip / upsell | ver `MINI-CURSO-COPY.md` |

PIX **por valor** (`pix-r20` / `pix-r50`) — nunca índice `qr_0` como R$20.

## 4. Checklist ATLAS (1 página)

- [ ] Projeto certo no Studio  
- [ ] Key criada (nunca colar no chat)  
- [ ] Rate-limit aberto  
- [ ] IDs OVER listados e bloqueados no harness  
- [ ] Fallback chat web definido  
- [ ] Landing/hub com PIX embutido  

## 5. Fontes

Só docs oficiais Gemini API + UI Studio. Sem corpus externo como verdade de cota.
