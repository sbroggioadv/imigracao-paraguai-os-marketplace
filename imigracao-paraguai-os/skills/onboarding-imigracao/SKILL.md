---
name: onboarding-imigracao
description: "primeira interação por botões; registra público, rota, localização, status, prazo crítico e habilitação profissional PY. Frentes 👤💼⚖️. Travas T1,T3,T6. Paraguai — Ley 6984/2022 + MERCOSUL + Res. DNM 407/2026. Zero número operacional hardcoded; URL oficial + data. Use em: /start-imigracao-paraguai, configurar, primeira vez, onboarding."
---

> **🖱️ Escolhas = botões:** nas listas fechadas use **AskUserQuestion** (máx. 4 opções; se houver mais, divida).

# ONBOARDING IMIGRACAO

> **Camada C0** · Frentes: 👤 imigrante · 💼 comercial · ⚖️ advogado  
> Plugin: `imigracao-paraguai-os` · Régua: `context/anexo-travas-paraguai.md` (9 travas)

## Papel
primeira interação por botões; registra público, rota, localização, status, prazo crítico e habilitação profissional PY

## Anexos
`context/anexo-travas-paraguai.md`

## Travas aplicáveis
- **T1:** Mandatário administrativo = **advogado matriculado no Paraguai** com poder do art. 41 da Ley 6715. OAB sozinha não basta. Pedido de residência é pessoal/presencial na DNM. Gestoria 174/2018 é gap de vigência.
- **T3:** A rota nasce da categoria jurídica, não do rótulo. Sem job seeker / nômade / rentista / visto de estudante autônomos confirmados. MERCOSUL ≠ permanente automática.
- **T6:** Residência (DNM) ≠ cédula (Policía) ≠ RUC (DNIT) ≠ residência fiscal ≠ nacionalidade (CSJ). Residência PY não encerra IR brasileiro.

## Disclaimer (uma linha)
Não substitui advogado matriculado no Paraguai nem garante residência, cédula, RUC ou naturalização. BACN e páginas oficiais vencem a memória do modelo.


## Fluxo (botões AskUserQuestion)

1. **Frente:** 👤 Imigrante · 💼 Comercial · ⚖️ Advogado · Só estudar o plugin.
2. **Objetivo:** entrar/turismo · temporária · permanente · investir · família · naturalização · já tenho processo · não sei.
3. **Nacionalidade:** brasileiro · outro MERCOSUL · outro.
4. **Onde está agora:** Brasil · PY com residência · PY sem título / vencido · outro.
5. **Habilitação (se 💼/⚖️):** matriculado PY · só OAB · gestor · não se aplica.
6. **Datas:** tem ingresso/residência/notificação com data? (texto livre se sim).

### ⛔ Se o objetivo for “residência fácil / depósito / sem comparecer”
Aplicar T1 + T5: recusar. Abrir `captacao-honesta-e-o-que-nao-vender`.

### ⛔ Se o objetivo for refúgio por projeto econômico
Aplicar T8: recusar. Abrir `refugio-conare` só se houver risco humanitário verdadeiro.

Grave o perfil e devolva ao `imigracao-master`.


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
