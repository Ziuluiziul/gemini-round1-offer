# Playbook curto — Gemini API free-tier (AI Studio ATLAS)

Entrega amostra ROUND1. Free Studio only. Recebedor PIX: LUIZ. Contato: z99003303@gmail.com

## Fontes oficiais
- Modelos: https://ai.google.dev/gemini-api/docs/models
- Rate limits: https://ai.google.dev/gemini-api/docs/rate-limits
- Erros: https://ai.google.dev/gemini-api/docs/api-errors
- Studio: https://aistudio.google.com · rate-limit · apikey

## Cotas (sem inventar números)
Monitore RPM / TPM / RPD **por projeto e por modelo** no painel do AI Studio.
RPD reseta à meia-noite PT. Números mudam — consulte o Studio; não copie RPM de fórum.

## Operação ATLAS
1. Um `generateContent` em voo por modelo (fila sequencial).
2. 429 / `quota_exceeded` → exponential backoff + jitter (não tight-loop).
3. Projeto OVER / exhausted → fallback Gemini chat web (`gemini.google.com`).
4. Sem billing pago sem dono financeiro explícito.
5. API key só em env / secret manager — nunca no repo.

## Mini-receita
`POST https://generativelanguage.googleapis.com/v1beta/models/{MODEL}:generateContent?key=...`
Payload mínimo: `contents[].parts[].text` + `generationConfig` opcional.

## Checklist
- [ ] Projeto Free Tier no Studio
- [ ] Key em variável de ambiente
- [ ] Limites lidos no painel (não inventados)
- [ ] Backoff em 429/503
- [ ] Plano exhausted → chat web

## Amostra copy-brief (SKU R$20)
Ver samples em round1/round2; landing com PIX: https://ziuluiziul.github.io/gemini-round1-offer/
Hub: https://ziuluiziul.github.io/round1-cumulunimbus/
Gist: https://gist.github.com/Ziuluiziul/0e6771fe58fa79906722f89a05d82369
