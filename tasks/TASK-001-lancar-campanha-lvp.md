# TASK-001 — Lançar a campanha LVP $2.99 (LP no GHL + Meta)

**Dono:** Gleyber (PO). **Executor:** qualquer IA com acesso ao Meta Ads e ao GHL.

## Feito
- [x] Artes de feed e stories subidas na conta de anúncios 2590014361504349
- [x] Campanha `120255757614340699` e conjunto `120255757615880699` em rascunho ($500 por 30 dias, 50 mi de Marietta)
- [x] Formulário GHL `aBDuCyZrbqaI32tU4Fy9` criado, com os consentimentos de SMS ajustados
- [x] Funil GHL `wqrbGF6wEZmMDW1KFk9x` com as etapas `/lvp-299` e `/lvp-299-thank-you`
- [x] Pixel e evento Lead no head do funil
- [x] HTML final da LP e da página de obrigado em `lp/`

## Falta
1. [ ] **Domínio:** no GHL, adicionar `promo.1qfloors.com` (Settings → Domains); criar o CNAME `promo` na HostGator; selecionar o domínio no funil. *(precisa de login do Gleyber na HostGator)*
2. [ ] **Página da LP:** etapa `/lvp-299` → Create from blank → elemento Custom Code → colar `lp/LP-colar-no-GHL.html` → salvar e publicar.
3. [ ] **Página de obrigado:** etapa `/lvp-299-thank-you` → Custom Code → colar `lp/ThankYou-colar-no-GHL.html` → salvar e publicar.
4. [ ] **Formulário:** On Submit → Redirect URL `https://promo.1qfloors.com/lvp-299-thank-you`.
5. [ ] **Pixel na conta de anúncios:** atribuir o Pixel 674668794633920 à conta 2590014361504349 (exige a chave de acesso do Gleyber no Business Suite) **ou** criar um Pixel novo na própria conta via API e trocar o ID no head do funil.
6. [ ] **Testar:** abrir a LP, enviar o formulário de teste, conferir se o contato cai no GHL e se o Lead dispara no Pixel.
7. [ ] **Meta:** trocar o conjunto para destino WEBSITE com promoted_object {pixel_id, custom_event_type: LEAD}; se não der para editar, criar um conjunto novo na mesma campanha.
8. [ ] **Anúncio:** criativo com as 2 artes (feed e stories), link `https://promo.1qfloors.com/lvp-299`, 2 textos, 3 títulos, CTA GET_QUOTE. Mostrar a prévia ao Gleyber.
9. [ ] **Cartão** cadastrado na conta de anúncios. *(Gleyber)*
10. [ ] **Descartar** a campanha rascunho antiga `120255757570260699`. *(pedir confirmação)*
11. [ ] **Publicar.** *(só com o "ok" do Gleyber)*
12. [ ] **Até 27/11:** trocar as artes "Offer ends Nov 30" por um novo prazo.

## Automação (depois)
- Workflow no GHL: gatilho "Form submitted" (1Q LVP 2.99 - LP) → tag "LVP 2.99" → SMS e e-mail imediato ao cliente → notificação interna para ligar em até 5 minutos.

## Copy sugerida (em inglês)
- **Primary A:** New floors. Installed. $2.99/sq ft — flooring AND installation included. 🏡 Serving Metro Atlanta. Get your free quote in 30 seconds and have new floors before the holidays. ⏰ Limited install slots.
- **Primary B:** Tired of looking at old carpet and scratched floors? Luxury vinyl plank, installed, from $2.99/sq ft — old floor removal included. Free in-home estimate across Metro Atlanta.
- **Headlines:** "$2.99/sq ft Installed" · "New Floors Before the Holidays" · "Free In-Home Estimate"
