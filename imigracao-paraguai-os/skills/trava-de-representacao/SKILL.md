---
name: trava-de-representacao
description: "GATE 2 — interessado pessoal, mandatário = advogado matriculado PY, poder do art. 41, gestoria e escalonamento. Frentes 👤💼⚖️. Travas T1. Paraguai — Ley 6984/2022 + MERCOSUL + Res. DNM 407/2026. Zero número operacional hardcoded; URL oficial + data. Use em: representar, OAB, matriculado, gestor, DNM, sem comparecer."
---

> **🖱️ Escolhas = botões:** nas listas fechadas use **AskUserQuestion** (máx. 4 opções; se houver mais, divida).

# TRAVA DE REPRESENTACAO

> **Camada C1** · Frentes: 👤 imigrante · 💼 comercial · ⚖️ advogado  
> Plugin: `imigracao-paraguai-os` · Régua: `context/anexo-travas-paraguai.md` (9 travas)

## Papel
GATE 2 — interessado pessoal, mandatário = advogado matriculado PY, poder do art. 41, gestoria e escalonamento

## Anexos
`context/anexo-representacao.md`, `context/anexo-travas-paraguai.md`

## Travas aplicáveis
- **T1:** Mandatário administrativo = **advogado matriculado no Paraguai** com poder do art. 41 da Ley 6715. OAB sozinha não basta. Pedido de residência é pessoal/presencial na DNM. Gestoria 174/2018 é gap de vigência.

## Disclaimer (uma linha)
Não substitui advogado matriculado no Paraguai nem garante residência, cédula, RUC ou naturalização. BACN e páginas oficiais vencem a memória do modelo.


## A interseção paraguaia (não é 292.1, OA nem abogacía espanhola)

| Quem | Pode | Não pode |
|---|---|---|
| **Cliente** | Atuar por si; comparecimento presencial exigido pela DNM | Delegar o pedido de residência “sem ir” |
| **Mandatário** | Acompanhar/defender **se** for advogado matriculado PY + poder art. 41 | Ser só OAB, consultor ou gestor |
| **Gestor documental** | Apoio material estreito, se existir base vigente (gap 174/2018) | Parecer, recurso, patrocínio, “representante DNM” |
| **Só OAB** | Direito BR, documentos BR, logística, coordenação | Representar na DNM/CONARE/CSJ |
| **Advogado matriculado CSJ** | Mandato administrativo e judicial nos limites da matrícula | Dispensar o comparecimento pessoal quando a DNM o exige |
| **Refúgio** | Pedido pessoal e gratuito do interessado | Gestor protocolar no lugar do solicitante |

### Frases bloqueadas
- “Com OAB você representa na DNM.”
- “MERCOSUL valida a OAB no Paraguai.”
- “Protocolamos sem você ir.”
- “Gestor registrado = mandatário jurídico.”


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
