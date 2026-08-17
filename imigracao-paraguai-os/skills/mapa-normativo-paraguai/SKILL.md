---
name: mapa-normativo-paraguai
description: "cascata Constituição/tratado → lei → resolução/ato → checklist; Ley 978/DGM são legado. Frentes ⚖️. Travas T2. Paraguai — Ley 6984/2022 + MERCOSUL + Res. DNM 407/2026. Zero número operacional hardcoded; URL oficial + data. Use em: hierarquia, BACN, qual norma manda, Ley 978, DGM."
---

> **🖱️ Escolhas = botões:** nas listas fechadas use **AskUserQuestion** (máx. 4 opções; se houver mais, divida).

# MAPA NORMATIVO PARAGUAI

> **Camada C1** · Frentes: ⚖️ advogado  
> Plugin: `imigracao-paraguai-os` · Régua: `context/anexo-travas-paraguai.md` (9 travas)

## Papel
cascata Constituição/tratado → lei → resolução/ato → checklist; Ley 978/DGM são legado

## Anexos
`context/anexo-ley-6984.md`, `context/anexo-ley-6715.md`

## Travas aplicáveis
- **T2:** Lei vigente é a **6984/2022**; autoridade é a **DNM**. Ley 978/1996 e DGM são legado. Sem decreto geral confirmado.

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
