# Desafio 7 Dias com IA — Dia 3

## Gerar Nota Clinica SOAP com IA

**Tempo estimado:** 20 minutos
**Ferramenta:** ChatGPT, Claude ou Gemini
**Nivel:** Iniciante

---

## Objetivo

Usar a IA para transformar anotacoes informais de uma consulta em uma nota clinica estruturada no formato SOAP, e entender como isso pode otimizar sua documentacao.

---

## Tarefa

Pegar suas anotacoes informais de uma consulta recente (ja documentada), anonimiza-las, e pedir a IA para gerar uma nota SOAP completa. Depois, comparar com o que voce registrou no prontuario.

---

## Passo a Passo

### 1. Escolha uma consulta recente (2 min)
Selecione uma consulta que voce ja documentou no prontuario. Idealmente, uma consulta de complexidade media.

### 2. Anonimize e prepare (3 min)
Escreva as informacoes da consulta como anotacoes informais (como se estivesse ditando rapidamente). Anonimize todos os dados.

Exemplo de entrada:
```
Paciente masculino, 58 anos, veio por dor no peito ha 2 dias,
tipo aperto, ao esforco, melhora com repouso, nega irradiacao.
HAS ha 10 anos, DM2 ha 5 anos, fumou 30 anos parou ha 2.
Usa metformina, losartana, AAS. Exame: PA 150x90, FC 88, ausculta
limpa, sem edema. ECG: ritmo sinusal, sem alteracoes agudas.
Troponina negativa. Vou pedir teste ergometrico.
```

### 3. Gere a nota SOAP (5 min)
Use o seguinte prompt:

```
Sou medico [especialidade]. Com base nas anotacoes informais abaixo
de uma consulta, gere uma nota clinica completa no formato SOAP.

Anotacoes:
[cole suas anotacoes informais anonimizadas aqui]

Requisitos:
- S (Subjetivo): Queixa principal, HDA detalhada, revisao de sistemas relevante
- O (Objetivo): Exame fisico estruturado, sinais vitais, exames complementares
- A (Avaliacao): Hipoteses diagnosticas em ordem de probabilidade, raciocinio
- P (Plano): Condutas, exames solicitados, medicacoes, orientacoes, retorno

Mantenha linguagem medica profissional. Nao invente informacoes
que nao estao nas anotacoes. Se algo esta incompleto, indique
com [informacao nao disponivel].
```

### 4. Revise criticamente (5 min)
Compare a nota gerada com o que voce escreveu no prontuario:
- A IA adicionou informacoes que voce nao forneceu? (isso seria um erro grave)
- A estrutura esta melhor, pior ou similar a sua?
- O raciocinio clinico na secao "A" faz sentido?
- A linguagem e adequada para seu contexto?

### 5. Ajuste e personalize (5 min)
Peca ajustes a IA, se necessario:
```
Ajustes na nota:
- Na secao A, adicione [informacao]
- O plano deve incluir [conduta especifica]
- Remova [informacao incorreta ou irrelevante]
- Use a terminologia padrao do meu servico: [termos especificos]
```

---

## Criterio de Sucesso

Voce completou o desafio se:
- [ ] Anonimizou os dados corretamente
- [ ] Gerou uma nota SOAP completa com IA
- [ ] Verificou que a IA nao inventou informacoes
- [ ] Identificou pelo menos uma melhoria que a IA trouxe em relacao a sua nota original
- [ ] Identificou pelo menos uma limitacao ou erro na nota gerada

---

## Pergunta de Reflexao

> Se voce usasse IA para gerar o primeiro rascunho de cada nota clinica, quanto tempo economizaria por dia? Quais riscos precisaria gerenciar para adotar isso na pratica?

---

## Dica do Dia

A nota gerada pela IA e sempre um **rascunho** que precisa da sua revisao. O maior risco nao e a IA errar — e voce aceitar o rascunho sem ler. Desenvolva o habito de revisar cada linha antes de incorporar ao prontuario. A responsabilidade pela documentacao e sempre sua.

---

*Desafio 7 Dias com IA — Material educacional do curso IAMed.*
