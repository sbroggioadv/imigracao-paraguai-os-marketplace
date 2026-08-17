---
name: varredura-de-vigencia
description: "GATE 1 — relê BACN + DNM/checklist/resolução no dia e devolve data, conflito ou gap. Frentes 👤💼⚖️. Travas T2,T3,T4,T5,T6,T7,T8,T9. Paraguai — Ley 6984/2022 + MERCOSUL + Res. DNM 407/2026. Zero número operacional hardcoded; URL oficial + data. Use em: vigência, atualizou, Ley 6984, Res. 407/2026, arancel, checklist."
---

> **🖱️ Escolhas = botões:** nas listas fechadas use **AskUserQuestion** (máx. 4 opções; se houver mais, divida).

# VARREDURA DE VIGENCIA

> **Camada C1** · Frentes: 👤 imigrante · 💼 comercial · ⚖️ advogado  
> Plugin: `imigracao-paraguai-os` · Régua: `context/anexo-travas-paraguai.md` (9 travas)

## Papel
GATE 1 — relê BACN + DNM/checklist/resolução no dia e devolve data, conflito ou gap

## Anexos
`context/anexo-travas-paraguai.md`, `context/anexo-ley-6984.md`

## Travas aplicáveis
- **T2:** Lei vigente é a **6984/2022**; autoridade é a **DNM**. Ley 978/1996 e DGM são legado. Sem decreto geral confirmado.
- **T3:** A rota nasce da categoria jurídica, não do rótulo. Sem job seeker / nômade / rentista / visto de estudante autônomos confirmados. MERCOSUL ≠ permanente automática.
- **T4:** Checklist vigente no dia. Precário/recibo ≠ deferimento. Conflito MERCOSUL × apostila permanece visível. Sem protocolo 100% online confirmado.
- **T5:** Solvência permanente = **Res. DNM 407/2026**. Sem depósito mágico. Investor Pass tem modalidades vivas no MIC/SUACE — número = URL do dia.
- **T6:** Residência (DNM) ≠ cédula (Policía) ≠ RUC (DNIT) ≠ residência fiscal ≠ nacionalidade (CSJ). Residência PY não encerra IR brasileiro.
- **T7:** Naturalização: triênio conta da **permanente**, não da chegada. Sem SLA de 30 dias. Dupla nacionalidade PY é gap; EC 131/2023 afasta perda automática BR.
- **T8:** Refúgio (Ley 1938/CONARE) é pessoal, gratuito e humanitário. Não regulariza projeto econômico. Certificado provisório ≠ residência definitiva.
- **T9:** Recurso exige ato + notificação + regime. **Não suspende sozinho.** Não transplantar prazos da 6715 para refúgio/naturalização.

## Disclaimer (uma linha)
Não substitui advogado matriculado no Paraguai nem garante residência, cédula, RUC ou naturalização. BACN e páginas oficiais vencem a memória do modelo.


## Como rodar o GATE 1

Para **cada** afirmação operacional (taxa, checklist, solvência, Investor Pass, cédula, prazo de processamento):

1. Abrir o texto na **BACN** (lei/tratado).
2. Abrir a **página/checklist/resolução** viva da DNM, MIC/SUACE, Policía, DNIT ou CSJ.
3. Registrar **URL + data/hora**.
4. Classificar: `CONFIRMADO` · `TRANSICAO` · `CONFLITO` · `NAO-PROVADO`.
5. Conflito (cédula MERCOSUL, apostila do Acordo, prazo CONARE, gestoria 174/2018) **permanece visível**.

### ⛔ Recusar de memória
Ley 978 vigente · DGM como autoridade atual · depósito mágico · Res. 710/905/2024 como solvência nova · job seeker / nômade / rentista como visto temporário · SLA de fila.


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
