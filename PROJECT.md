# 1st Quality Floors — Campanha LVP $2.99/sq ft (Nov–Dez 2026)

**Handoff em 19/11/2026 (ET):** landing page e página de obrigado publicadas no GoHighLevel. Campanha, conjunto e anúncio seguem em rascunho no Meta na última conferência. Gleyber autorizou iniciar a campanha, que ainda depende das pendências da TASK-001.

## Contexto
- Empresa: 1st Quality Floors, instalação de pisos, Suite 14, 849 Pickens Industrial Dr NE, Marietta GA. Atende Metro Atlanta, raio de 50 mi, de segunda a sábado.
- Oferta: **$2.99/sq ft, LVP, material + instalação**. Público: homeowners americanos (anúncios em inglês).
- Verba: **$500 no total por 30 dias** (18/11 → 18/12/2026).
- Artes: `ads/1stQuality_Main.png` (feed 4:5) e `ads/1stQuality_Story.png` (stories 9:16). As artes dizem "Offer ends Nov 30". O plano é trocar por um novo prazo no fim do mês (ver DECISIONS).

## Meta (Business: N1 International Flooring, ID 3592311174326077)
- Conta de anúncios: **1st Quality Floors, `2590014361504349`**. A Visão geral ainda pede forma de pagamento e confirmação da Página.
- Página FB: `258782390648115`. Instagram: @1stqualityfloorscompany (`17841405920202812`).
- Imagens já na conta (hashes): Main `e07dbc1a65017af2e1252836db521f8f`, Story `4358f72706a8f84af71092acee3cd8e7`.
- **Campanha válida (rascunho):** `120255757614340699`, "1Q | Leads | LVP $2.99 | Metro ATL 50mi | $500/30d". OUTCOME_LEADS, orçamento total de $500, de 18/11 a 18/12.
  - Conjunto `120255757615880699`: raio de 50 mi de Marietta (33.9706, -84.5316), Advantage+ (sugestão de 30–65 anos). Destino **Site**, Pixel `2611615095987566` e evento **Lead** salvos. O nome do conjunto ainda contém “Instant Form”.
  - Anúncio em rascunho **1Q | LVP $2.99 | Feed + Stories**. Página e Instagram corretos aparecem selecionados no editor. Faltam mídia, textos, título, CTA, link e prévia.
- **Rascunho antigo a descartar:** campanha `120255757570260699` (estrutura duplicada com $35/dia). Aguardando o "sim" do Gleyber.
- Pixel da campanha: **1st Quality Floors | LVP Leads** (`2611615095987566`), confirmado no Gerenciador de Eventos e selecionado no conjunto. O Pixel antigo `674668794633920` permanece como ativo separado.

## GoHighLevel (agência Reby, white-label links.rebyagency.com)
- Subconta: 1st Quality Floors, location `X9tt7P1Y6b0MhL7UeHce`.
- Formulário **"1Q LVP 2.99 - LP"**, ID `aBDuCyZrbqaI32tU4Fy9`. Campos: nome, sobrenome, telefone, e-mail, 2 consentimentos de SMS. On Submit está em **Redirect to URL** com `https://promo.1stqualityfloors.com/lvp-299-thank-you`, confirmado após recarregar. Os links de privacidade e termos ainda apontam para `example.com`.
  - Embed: `https://links.rebyagency.com/widget/form/aBDuCyZrbqaI32tU4Fy9`
- Funil **"1Q - LVP 2.99"**, ID `wqrbGF6wEZmMDW1KFk9x`.
  - **LP LVP 2.99:** HTML original inserido via Custom Code. URL pública conferida com o formulário visível: `https://promo.1stqualityfloors.com/lvp-299-page`. O caminho da etapa é `/lvp-299`.
  - **Thank You:** HTML original inserido e publicação confirmada pelo GHL. O caminho da etapa é `/lvp-299-thank-you`; o editor mostra também `/lvp-299-thank-you-page`. O redirecionamento ainda precisa de teste por envio real.
  - **Head tracking code:** Pixel `2611615095987566` com PageView no funil e Lead nos dois caminhos de agradecimento. Código conferido após recarregar; recebimento de eventos ainda pendente de teste.
  - **Domínio:** `promo.1stqualityfloors.com`, com CNAME `promo` → `sites.ludicrous.cloud` no cPanel da HostGator. Domínio validado e vinculado ao funil, com LP como etapa padrão.

## Arquivos da LP
- `lp/LP-colar-no-GHL.html`: LP final, com as imagens embutidas em base64 e o form do GHL. Para colar num elemento Custom Code (~650 KB).
- `lp/ThankYou-colar-no-GHL.html`: página de obrigado.
- `lp/LP-source.html`: fonte original, com placeholders `REPLACE_` de imagem. As imagens estão no Mac, em `~/Pictures/1st-quality-lp/images`.

## Próximos passos
Ver `tasks/TASK-001-lancar-campanha-lvp.md`.
