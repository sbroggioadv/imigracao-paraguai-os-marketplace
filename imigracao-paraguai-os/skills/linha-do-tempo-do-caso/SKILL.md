---
name: linha-do-tempo-do-caso
description: "organiza vencimentos, janelas, notificações, ausências e eventos sem prometer processamento. Frentes 👤⚖️. Travas T3,T4,T7,T8,T9. Paraguai — Ley 6984/2022 + MERCOSUL + Res. DNM 407/2026. Zero número operacional hardcoded; URL oficial + data. Use em: linha do tempo, vencimento, 90 dias, janela de conversão."
---

> **🖱️ Escolhas = botões:** nas listas fechadas use **AskUserQuestion** (máx. 4 opções; se houver mais, divida).

# LINHA DO TEMPO DO CASO

> **Camada C2** · Frentes: 👤 imigrante · ⚖️ advogado  
> Plugin: `imigracao-paraguai-os` · Régua: `context/anexo-travas-paraguai.md` (9 travas)

## Papel
organiza vencimentos, janelas, notificações, ausências e eventos sem prometer processamento

## Anexos
`context/anexo-ley-6715.md`

## Travas aplicáveis
- **T3:** A rota nasce da categoria jurídica, não do rótulo. Sem job seeker / nômade / rentista / visto de estudante autônomos confirmados. MERCOSUL ≠ permanente automática.
- **T4:** Checklist vigente no dia. Precário/recibo ≠ deferimento. Conflito MERCOSUL × apostila permanece visível. Sem protocolo 100% online confirmado.
- **T7:** Naturalização: triênio conta da **permanente**, não da chegada. Sem SLA de 30 dias. Dupla nacionalidade PY é gap; EC 131/2023 afasta perda automática BR.
- **T8:** Refúgio (Ley 1938/CONARE) é pessoal, gratuito e humanitário. Não regulariza projeto econômico. Certificado provisório ≠ residência definitiva.
- **T9:** Recurso exige ato + notificação + regime. **Não suspende sozinho.** Não transplantar prazos da 6715 para refúgio/naturalização.

## Disclaimer (uma linha)
Não substitui advogado matriculado no Paraguai nem garante residência, cédula, RUC ou naturalização. BACN e páginas oficiais vencem a memória do modelo.


## Como operar esta skill

1. Confirmar **frente** e se os gates já rodaram; se não, chamar `varredura-de-vigencia` e `trava-de-representacao`.
2. Pedir os **fatos mínimos**: nacionalidade, onde está, objetivo, categoria atual, datas de ingresso/residência/notificação, se há mandatário matriculado.
3. **Classificar a rota** (transitório / ocasional / 6984 / MERCOSUL / Investor Pass / refúgio / naturalização) **antes** do checklist.
4. Mapear **finalidade → dispositivo (6984 / Acordo / resolução) → checklist DNM vivo → órgão**.
5. Profundidade da frente:
   - 👤 checklist e decisões honestas, sem minuta de mandato PY
   - 💼 escopo vendável, contrato e o que **não** vender
   - ⚖️ matriz norma→requisito→prova→remédio, com referral ao matriculado se faltar habilitação
6. Toda afirmação operacional: **URL oficial + data**. Sem fonte atual → `NAO-PROVADO`.
7. Fechar entrega normativa com `validador-imigratorio`.


## URLs de topo (sempre preferir estas)
- BACN Ley 6984: https://www.bacn.gov.py/leyes-paraguayas/10973/ley-n-6984-de-migraciones
- BACN Ley 6715: https://www.bacn.gov.py/leyes-paraguayas/10974/ley-n-6715-
- DNM: https://migraciones.gov.py
- Temporária geral: https://migraciones.gov.py/residencia-temporal/
- Temporária MERCOSUL: https://migraciones.gov.py/residencia-temporaria-mercosur/
- Permanente MERCOSUL: https://migraciones.gov.py/residencia-permanente-mercosur/
- Res. DNM 407/2026: https://migraciones.gov.py/wp-content/uploads/2026/06/RESOLUCION-DNM-Nro-407-28.05.2026-ACREDITACION-DE-SOLVENCIA-ECONOMICA-PARA-RESIDENCIA-PERMANENTE-1.pdf
- CONARE: https://www2.mre.gov.py/conare/index.php/solicitar-refugio
- CSJ naturalização: https://www.pj.gov.py/contenido/463-carta-de-naturalizacion/463

## Saída esperada
1. Frente + fase + nacionalidade + rota + **data do ato** usada.  
2. Regime jurídico aplicável (dispositivo + URL + data de leitura).  
3. O que fazer agora / o que não fazer (⛔).  
4. Lacunas `NAO-PROVADO` / conflitos oficiais declarados.  
5. Próxima skill ou referral (advogado matriculado / DNM / CONARE / CSJ / Policía / DNIT).

## Guard
- Zero taxa/cota/piso/SLA hardcoded.  
- Zero promessa de resultado ou prazo de aprovação.  
- Zero copiar trava dos EUA (292.1), Portugal (OAB≠OA) ou Espanha (OAB≠abogacía).  
- Byte cap: manter este arquivo ≤ 11.000 B.
