# 🧬 Receita para recriar: Maikon Caldeira — Aplicativos

_Gerada sem IA, lendo 12 arquivo(s). Serve para remontar este app como HTML modular — com qualquer IA, um arquivo por vez._

## 1. O que é

- **Nome:** Maikon Caldeira — Aplicativos
- **Partes de código:** 6 (6 tela, 0 logica, 0 servidor, 0 dados, 0 estilo)
- **Tem servidor (rotas /api):** não — dá para ser só HTML
- **Peças de fora (bibliotecas):** nenhuma

## 2. Estrutura modular proposta

```
index.html            ← a página; chama os módulos NA ORDEM
css/app.css           ← o visual
js/00-core.js         ← a "locomotiva": cria window.APP (registrar, guardar, avisar)
js/10-1.js            ← Auditoria Financeira — Calculadora Sentença (v25/11-K) — Auditoria Fin (era 1.html)
js/15-2.js            ← Calculadora de Sentença — Modelo Geral (v25/11-A) — Auditoria Financei (era 2.html)
js/20-3.js            ← Auditoria Financeira — Calculadora Sentença — Auditoria Financeira — C (era 3.html)
js/25-4.js            ← Montador Simples (v25/11-B) — Montador simples (era 4.html)
js/30-5.js            ← Montador Simples (v25/11-B) — Montador simples (era 5.html)
js/35-inicio.js       ← Maikon Caldeira — Aplicativos — MAIKON CALDEIRA (era index.html)
js/99-app.js          ← o último: monta a tela com o que embarcou
```

## 3. As partes, uma por uma

| # | Era | Vira | Tipo | O que faz | Usa |
|---|---|---|---|---|---|
| 1 | `1.html` | `js/10-1.js` | tela | Auditoria Financeira — Calculadora Sentença (v25/11-K) — Auditoria Financeira — Calculador | — |
| 2 | `2.html` | `js/15-2.js` | tela | Calculadora de Sentença — Modelo Geral (v25/11-A) — Auditoria Financeira — Calculadora de  | — |
| 3 | `3.html` | `js/20-3.js` | tela | Auditoria Financeira — Calculadora Sentença — Auditoria Financeira — Calculadora de Senten | — |
| 4 | `4.html` | `js/25-4.js` | tela | Montador Simples (v25/11-B) — Montador simples | — |
| 5 | `5.html` | `js/30-5.js` | tela | Montador Simples (v25/11-B) — Montador simples | — |
| 6 | `index.html` | `js/35-inicio.js` | tela | Maikon Caldeira — Aplicativos — MAIKON CALDEIRA | manifest.json, icon-192.png |

## 4. Montar passo a passo (cada bloco é um pedido pronto: 📋 Copiar → colar na IA)

### Passo 0 — combinar as regras com a IA

```text
Vamos recriar o app "Maikon Caldeira — Aplicativos" como HTML MODULAR, que abre pelo index.html, sem servidor e sem nada da Replit.
Regras: (1) index.html chama os arquivos js/ na ordem, antes do </body>; (2) js/00-core.js cria window.APP com APP.registrar(modulo), APP.guardar(chave, valor) em IndexedDB/localStorage e APP.avisar(texto); (3) cada arquivo js/NN-nome.js cuida de UM assunto, começa com (function (APP) { e termina com })(window.APP); (4) js/99-app.js vem por último e monta a tela com os módulos registrados; (5) textos em português do Brasil.
Vou pedir UM arquivo por vez. Responda só com o arquivo completo, sem cortar nada. Primeiro: crie index.html, css/app.css e js/00-core.js.
```

### Passo 1 — `js/10-1.js` (era `1.html`, 1419 linhas)

```text
Crie js/10-1.js. Ele faz: Auditoria Financeira — Calculadora Sentença (v25/11-K) — Auditoria Financeira — Calculadora de Sentença · v25/11-K.
No app original ele tinha estas funções/partes: setClock, log, avisar, fmtBRL, fmtPct, fmtFator, toNum, parseDateBR, dateToYM, listMonths, ymToLabel, mesNome, numU, anoU, lerTabelaMeses, lerColunasPorMes, tipoTabela, buscarSerie.
Ele chamava estes endereços: https://api.bcb.gov.br/dados/serie/bcdata.sgs., /api/tjmg/fatores?startYear=. Em HTML, ligue cada um à função equivalente do módulo certo.
Registre com APP.registrar({ nome, icone, abrir }). Devolva só o arquivo completo.
```

### Passo 2 — `js/15-2.js` (era `2.html`, 1408 linhas)

```text
Crie js/15-2.js. Ele faz: Calculadora de Sentença — Modelo Geral (v25/11-A) — Auditoria Financeira — Calculadora de Sentença · Geral v25/11-A.
No app original ele tinha estas funções/partes: setClock, log, avisar, fmtBRL, fmtPct, fmtFator, toNum, parseDateBR, dateToYM, listMonths, ymToLabel, mesNome, numU, anoU, lerTabelaMeses, lerColunasPorMes, tipoTabela, buscarSerie.
Ele chamava estes endereços: https://api.bcb.gov.br/dados/serie/bcdata.sgs., /api/tjmg/fatores?startYear=. Em HTML, ligue cada um à função equivalente do módulo certo.
Registre com APP.registrar({ nome, icone, abrir }). Devolva só o arquivo completo.
```

### Passo 3 — `js/20-3.js` (era `3.html`, 1034 linhas)

```text
Crie js/20-3.js. Ele faz: Auditoria Financeira — Calculadora Sentença — Auditoria Financeira — Calculadora de Sentença.
No app original ele tinha estas funções/partes: setClock, log, fmtBRL, fmtPct, fmtFator, toNum, parseDateBR, dateToYM, listMonths, ymToLabel, fetchBCB, fetchTJMG, getTJMGCorrection, calcularRecursal, calcular, renderParecer, salvarDados.
Ele chamava estes endereços: https://api.bcb.gov.br/dados/serie/bcdata.sgs., /api/tjmg/fatores?startYear=, /api/share/parecer, /api/export/word. Em HTML, ligue cada um à função equivalente do módulo certo.
Registre com APP.registrar({ nome, icone, abrir }). Devolva só o arquivo completo.
```

### Passo 4 — `js/25-4.js` (era `4.html`, 387 linhas)

```text
Crie js/25-4.js. Ele faz: Montador Simples (v25/11-B) — Montador simples.
No app original ele tinha estas funções/partes: esc, lerPref, gravarPref, mesNome, num, anoU, consertarLetras, separador, colunas, csv, cel, tabelaHtml, lerColunasPorMes, tira, tipoData, achar, plano, mostrarPecas.
Registre com APP.registrar({ nome, icone, abrir }). Devolva só o arquivo completo.
```

### Passo 5 — `js/30-5.js` (era `5.html`, 385 linhas)

```text
Crie js/30-5.js. Ele faz: Montador Simples (v25/11-B) — Montador simples.
No app original ele tinha estas funções/partes: esc, lerPref, gravarPref, mesNome, num, anoU, consertarLetras, separador, colunas, csv, cel, tabelaHtml, lerColunasPorMes, tira, tipoData, achar, plano, mostrarPecas.
Registre com APP.registrar({ nome, icone, abrir }). Devolva só o arquivo completo.
```

### Passo 6 — `js/35-inicio.js` (era `index.html`, 136 linhas)

```text
Crie js/35-inicio.js. Ele faz: Maikon Caldeira — Aplicativos — MAIKON CALDEIRA.
No app original ele tinha estas funções/partes: lerInfo, procurar, pintar, abrir, fechar.
Registre com APP.registrar({ nome, icone, abrir }). Devolva só o arquivo completo.
```

### Passo 7 — `js/99-app.js` e conferir

```text
Crie js/99-app.js: ele olha APP.modulos e monta o menu/abas com um botão para cada módulo. Depois, me mande o index.html atualizado com todos os <script src="js/…"> na ordem certa: js/00-core.js, js/10-1.js, js/15-2.js, js/20-3.js, js/25-4.js, js/30-5.js, js/35-inicio.js, js/99-app.js.
```

## 5. Conferir no final

- [ ] Abrir o index.html na prévia: aparece a tela sem erro (▤ console vazio)?
- [ ] Cada botão abre a sua parte?
- [ ] Fechar e abrir de novo: os dados continuam?
- [ ] Nada com "replit", "REPL_", "@workspace" no código (🏗️ Preparar confere).
- [ ] 📱 PWA → deixar instalável; 📦 APK ou 🖥️ .exe.
