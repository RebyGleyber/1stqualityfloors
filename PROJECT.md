# 1st Quality Floors — Campanha LVP $2.99/sq ft (Nov–Dez 2026)

**Status em 18/11/2026, 10:50 ET:** campanha montada em rascunho no Meta; LP e formulário criados no GHL, mas ainda não publicados. Nada está no ar e nada foi gasto.

## Contexto
- Empresa: 1st Quality Floors, instalação de pisos, Suite 14, 849 Pickens Industrial Dr NE, Marietta GA. Atende Metro Atlanta, raio de 50 mi, de segunda a sábado.
- Oferta: **$2.99/sq ft, LVP, material + instalação**. Público: homeowners americanos (anúncios em inglês).
- Verba: **$500 no total por 30 dias** (18/11 → 18/12/2026).
- Artes: `ads/1stQuality_Main.png` (feed 4:5) e `ads/1stQuality_Story.png` (stories 9:16). As artes dizem "Offer ends Nov 30". O plano é trocar por um novo prazo no fim do mês (ver DECISIONS).

## Meta (Business: N1 International Flooring, ID 3592311174326077)
- Conta de anúncios: **1st Quality Floors, `2590014361504349`**. ⚠️ Sem forma de pagamento cadastrada.
- Página FB: `258782390648115`. Instagram: @1stqualityfloorscompany (`17841405920202812`).
- Imagens já na conta (hashes): Main `e07dbc1a65017af2e1252836db521f8f`, Story `4358f72706a8f84af71092acee3cd8e7`.
- **Campanha válida (rascunho):** `120255757614340699`, "1Q | Leads | LVP $2.99 | Metro ATL 50mi | $500/30d". OUTCOME_LEADS, orçamento total de $500, de 18/11 a 18/12.
  - Conjunto de anúncios `120255757615880699`: raio de 50 mi a partir de Marietta (33.9706, -84.5316), Advantage+ (sugestão de 30–65 anos), ainda configurado como **formulário instantâneo (ON_AD)**. **Precisa virar website + Pixel, com evento Lead**, quando a LP estiver no ar.
  - Ainda sem anúncio criado.
- **Rascunho antigo a descartar:** campanha `120255757570260699` (estrutura duplicada com $35/dia). Aguardando o "sim" do Gleyber.
- Pixel existente: "1st Quality" `674668794633920`. Pertence ao portfólio da N1 e **não está atribuído** à conta de anúncios. Hoje só dispara no 1qfloors.com.

## GoHighLevel (agência Reby, white-label links.rebyagency.com)
- Subconta: 1st Quality Floors, location `X9tt7P1Y6b0MhL7UeHce`.
- Formulário **"1Q LVP 2.99 - LP"**, ID `aBDuCyZrbqaI32tU4Fy9`. Campos: nome, sobrenome, telefone, e-mail, 2 consentimentos de SMS. On Submit ainda está como "Message"; **trocar para Redirect** para a página de obrigado.
  - Embed: `https://links.rebyagency.com/widget/form/aBDuCyZrbqaI32tU4Fy9`
- Funil **"1Q - LVP 2.99"**, ID `wqrbGF6wEZmMDW1KFk9x`.
  - Etapa "LP LVP 2.99", caminho `/lvp-299`. Página ainda vazia.
  - Etapa "Thank You", caminho `/lvp-299-thank-you`. Página ainda vazia.
  - Head tracking code: Pixel `674668794633920`, com PageView mais o evento Lead quando o caminho contém "thank-you".
  - ⚠️ **Sem domínio.** O único domínio da subconta é store.n1flooring.com, que é da N1. Plano: `promo.1qfloors.com`, com CNAME na HostGator.

## Arquivos da LP
- `lp/LP-colar-no-GHL.html`: LP final, com as imagens embutidas em base64 e o form do GHL. Para colar num elemento Custom Code (~650 KB).
- `lp/ThankYou-colar-no-GHL.html`: página de obrigado.
- `lp/LP-source.html`: fonte original, com placeholders `REPLACE_` de imagem. As imagens estão no Mac, em `~/Pictures/1st-quality-lp/images`.

## Próximos passos
Ver `tasks/TASK-001-lancar-campanha-lvp.md`.
