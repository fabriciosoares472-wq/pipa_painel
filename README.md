# 📊 PiPA — Painel Pedagógico · Simulado 2026

> Plataforma de análise de desempenho do **Instituto Pipa (PiPA)** para professores e coordenação pedagógica. Dashboard interativo gerado a partir dos resultados do 1º Simulado 2026.

---

## 🌐 Acesso

**[pipasimulado.netlify.app](https://pipasimulado.netlify.app)**

---

## 🎯 O que é

Sistema de visualização pedagógica desenvolvido para apoiar professores, coordenadores e direção na leitura dos resultados do simulado preparatório para ingresso no ensino técnico. Todo o processamento acontece no browser — sem servidor, sem banco de dados, sem login.

---

## ✅ Funcionalidades

### Filtros em tempo real
- **Por turma** — Turma 1, 2, 3 ou 4 (ou visão geral)
- **Por disciplina** — Atualidades, Biologia, Interpretação, História, Geografia, Matemática, Gramática, Química, Física
- Todos os indicadores, gráficos e tabelas se recalculam instantaneamente ao aplicar filtros

### KPIs dinâmicos
- Total de alunos no recorte selecionado
- Média geral de acertos
- Melhor aluno da seleção
- Disciplina crítica (menor aproveitamento médio)
- Melhor disciplina
- Quantidade de alunos acima da média

### Acerto por questão
- 50 cards com percentual de acerto colorido por faixa
- Verde ≥ 60% · Âmbar 35–59% · Vermelho < 35%
- Questões da disciplina filtrada em destaque, demais desbotadas

### Gráficos interativos
- Distribuição de acertos (histograma por faixa de pontuação)
- Média por disciplina (barras horizontais)
- Comparativo entre turmas (responde ao filtro de disciplina)

### Quadrantes pedagógicos
Classificação dos alunos em 4 perfis baseados em nota × consistência entre disciplinas:

| Quadrante | Perfil | Ação sugerida |
|-----------|--------|---------------|
| ⭐ | Alta nota + Alta consistência | Referência — tutores de pares |
| 🚀 | Alta nota + Oscilante | Potencial — disciplinar estudo |
| 📈 | Baixa nota + Consistente | Reforço de conteúdo |
| ⚠ | Baixa nota + Oscilante | Intervenção prioritária |

### Gabaritados por disciplina
Lista todos os alunos que acertaram 100% das questões de cada disciplina, filtrado por turma.

### Mapa de calor
Tabela aluno × disciplina com células coloridas por nível de desempenho. Clicável para abrir perfil individual.

### Inteligência pedagógica
6 insights automáticos gerados a partir do recorte ativo — questão mais difícil, disciplina crítica, alunos em risco, gabaritados, questão mais fácil.

### Ranking individual
- Medalhas para os 3 primeiros
- Colunas por disciplina com acertos e percentual
- Badge de faixa (Avançado / Adequado / Básico / Crítico)
- Clique em qualquer aluno para abrir o perfil completo

### Perfil individual do aluno
- Gráfico radar: desempenho do aluno vs média da turma
- 4 KPIs: acertos totais, aproveitamento %, rank geral, rank na turma
- Barras detalhadas por disciplina

---

## 📐 Dados do simulado

| Item | Detalhe |
|------|---------|
| Edição | 1º Simulado 2026 |
| Alunos | 124 |
| Turmas | Turma 1, 2, 3 e 4 |
| Questões | 50 |
| Disciplinas | 9 |
| Média geral | 23,0 / 50 |

### Distribuição das questões por disciplina

| Disciplina | Questões | Total |
|------------|----------|-------|
| Atualidades | Q1–Q5 | 5 |
| Biologia | Q6–Q10 | 5 |
| Interpretação | Q11–Q21 | 11 |
| História | Q22–Q26 | 5 |
| Geografia | Q27–Q31 | 5 |
| Matemática | Q32–Q38 | 7 |
| Gramática | Q39–Q40 | 2 |
| Química | Q41–Q45 | 5 |
| Física | Q46–Q50 | 5 |

---

## 🚀 Deploy e atualização

### Estrutura do repositório

```
pipa_painel/
└── index.html      ← dashboard completo (autocontido)
└── README.md
```

### Para atualizar com um novo simulado

1. Gere o novo `index.html` com os dados atualizados
2. Substitua o arquivo no repositório GitHub
3. O Netlify faz redeploy automático em ~30 segundos

```bash
# Via Git
git add index.html
git commit -m "2º Simulado 2026 — dados atualizados"
git push origin main
```

Ou pelo GitHub web: abra `index.html` → ícone de lápis → cole o novo conteúdo → **Commit changes**.

---

## 🛠 Tecnologias

| Tecnologia | Uso |
|------------|-----|
| HTML / CSS / JavaScript | Interface e lógica |
| [Chart.js 4.4](https://www.chartjs.org/) | Gráficos |
| [Google Fonts](https://fonts.google.com/) | Tipografia (Syne + IBM Plex Sans + IBM Plex Mono) |
| [Netlify](https://netlify.com) | Hospedagem via GitHub |

> Sem framework, sem build, sem dependência local. Arquivo único, abre em qualquer browser.

---

## 🏫 Sobre o PiPA

**Instituto Pipa** é uma organização de preparação de jovens para ingresso no ensino técnico público. O simulado avalia 9 disciplinas do currículo preparatório e orienta a estratégia pedagógica dos professores.

---

*Desenvolvido com dados reais do 1º Simulado 2026 · PiPA – Instituto Pipa*
