---
name: imigracao-master
description: "identifica frente, fase, nacionalidade, objetivo e risco; chama os dois gates antes de rotear. Frentes 👤💼⚖️. Travas T1-T9. Paraguai — Ley 6984/2022 + MERCOSUL + Res. DNM 407/2026. Zero número operacional hardcoded; URL oficial + data. Use em: imigracao paraguai, master, quero imigrar para o paraguai, /imigracao-paraguai."
---

> **🖱️ Escolhas = botões:** nas listas fechadas use **AskUserQuestion** (máx. 4 opções; se houver mais, divida).

# IMIGRACAO MASTER

> **Camada C0** · Frentes: 👤 imigrante · 💼 comercial · ⚖️ advogado  
> Plugin: `imigracao-paraguai-os` · Régua: `context/anexo-travas-paraguai.md` (9 travas)

## Papel
identifica frente, fase, nacionalidade, objetivo e risco; chama os dois gates antes de rotear

## Anexos
`context/anexo-travas-paraguai.md`

## Travas aplicáveis
- **T1:** Mandatário administrativo = **advogado matriculado no Paraguai** com poder do art. 41 da Ley 6715. OAB sozinha não basta. Pedido de residência é pessoal/presencial na DNM. Gestoria 174/2018 é gap de vigência.
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


## Protocolo do master (ordem fixa)

1. **Frente** (botões AskUserQuestion): 👤 Imigrante · 💼 Comercial · ⚖️ Advogado · Ainda não sei.
2. **Fase**: pensando · escolhendo rota · montando pasta · protocolado · notificado · recorrendo.
3. **Nacionalidade / MERCOSUL:** brasileiro · outro MERCOSUL · outro.
4. **Localização:** no Brasil · no Paraguai regular · no Paraguai irregular/vencido · não sei.
5. **Objetivo:** entrar · temporária · permanente · Investor Pass · cédula/RUC · naturalização · defesa.
6. **Habilitação PY (se 💼/⚖️):** matriculado na CSJ · só OAB · gestor · não sei.
7. **GATE 1** `varredura-de-vigencia` — sempre.
8. **GATE 2** `trava-de-representacao` — sempre.
9. Rotear; fechar entrega normativa com `validador-imigratorio`.

### Mapa rápido de camadas
- **C2** triagem / diagnóstico / linha do tempo · **C3** entrada e temporária
- **C4** permanente, solvência 407, Investor Pass, cédula/RUC · **C5** refúgio / expulsão / recursos
- **C6** naturalização · **C7** comercial · **C8** ponte BR + dossiê

### Conflito entre skills
1. Trava do corpus > skill. 2. Lei > resolução > checklist. 3. Fonte lida hoje > memória. 4. Não transplantar 292.1, OAB≠OA nem OAB≠abogacía.


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
