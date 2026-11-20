# Template: Diagnóstico Diferencial Estruturado

## Quando usar

Use este template quando precisar que a IA gere uma lista de diagnósticos diferenciais organizada por probabilidade a partir de um quadro clínico. Ideal para casos complexos, atípicos ou quando você quer sistematizar o raciocínio antes de definir a conduta.

O template segue o framework **RCCFR** (Role, Contexto, Comando, Formato, Restrições), que estrutura o prompt para obter respostas mais consistentes e úteis.

---

## Template (copie e cole)

```
Atue como [ESPECIALIDADE] com experiência em diagnóstico clínico no contexto do sistema de saúde brasileiro.

CONTEXTO CLÍNICO:
- Paciente: [SEXO], [IDADE] anos
- Queixa principal: [QUEIXA PRINCIPAL E DURAÇÃO]
- História da doença atual: [HDA DETALHADA]
- Antecedentes pessoais: [COMORBIDADES, CIRURGIAS, INTERNAÇÕES]
- Medicações em uso: [LISTA DE MEDICAÇÕES COM DOSES]
- Antecedentes familiares: [DOENÇAS RELEVANTES NA FAMÍLIA]
- Hábitos: [TABAGISMO, ETILISMO, ATIVIDADE FÍSICA, ALIMENTAÇÃO]
- Exame físico relevante: [ACHADOS POSITIVOS E NEGATIVOS PERTINENTES]
- Exames complementares disponíveis: [RESULTADOS DE EXAMES JÁ REALIZADOS]

COMANDO:
Elabore um diagnóstico diferencial estruturado para este caso, listando as hipóteses da mais provável à menos provável.

FORMATO DE RESPOSTA:
Para cada hipótese diagnóstica, forneça:
1. Nome da condição e CID-10
2. Probabilidade estimada (alta / moderada / baixa)
3. Achados do caso que FAVORECEM esta hipótese
4. Achados do caso que VÃO CONTRA esta hipótese
5. Próximo exame ou teste mais importante para confirmar/excluir
6. Sinal de alarme ("red flag") que, se presente, eleva a urgência

Ao final, apresente:
- Resumo da hipótese mais provável com justificativa
- Proposta de investigação sequencial (do mais simples/disponível ao mais complexo)
- Condições que exigem ação imediata ("não pode esperar")

RESTRIÇÕES:
- Considere a disponibilidade de exames no SUS e na rede privada brasileira
- Não sugira tratamento — foque apenas no diagnóstico diferencial
- Inclua pelo menos 5 hipóteses, mesmo que algumas sejam menos prováveis
- Cite se alguma hipótese exige notificação compulsória
```

---

## Exemplo preenchido

```
Atue como clínico geral com experiência em diagnóstico clínico no contexto do sistema de saúde brasileiro.

CONTEXTO CLÍNICO:
- Paciente: masculino, 58 anos
- Queixa principal: dor torácica intermitente há 3 semanas
- História da doença atual: Refere dor retroesternal em aperto, sem relação clara com esforço, durando de 10 a 40 minutos, com irradiação ocasional para dorso. Nega dispneia, náuseas ou sudorese. Relata piora após refeições volumosas e ao deitar. Tomou omeprazol por conta própria com alívio parcial. Procurou UBS após episódio mais intenso ontem.
- Antecedentes pessoais: HAS há 12 anos, dislipidemia, ex-tabagista (parou há 5 anos, carga tabágica 30 maços-ano), apendicectomia aos 22 anos
- Medicações em uso: losartana 50 mg 2x/dia, sinvastatina 20 mg à noite, AAS 100 mg/dia
- Antecedentes familiares: pai com IAM aos 62 anos, mãe com DM2
- Hábitos: sedentário, alimentação rica em carboidratos, nega etilismo
- Exame físico relevante: PA 148x92 mmHg, FC 78 bpm, IMC 31. Ausculta cardíaca sem sopros. Pulmões limpos. Abdome com leve dor à palpação epigástrica. Sem edema de MMII.
- Exames complementares disponíveis: ECG de repouso com alterações inespecíficas de repolarização em parede inferior. Hemograma normal. Glicemia de jejum 118 mg/dL. Colesterol total 242 mg/dL, LDL 162 mg/dL, HDL 38 mg/dL.

COMANDO:
Elabore um diagnóstico diferencial estruturado para este caso, listando as hipóteses da mais provável à menos provável.

FORMATO DE RESPOSTA:
Para cada hipótese diagnóstica, forneça:
1. Nome da condição e CID-10
2. Probabilidade estimada (alta / moderada / baixa)
3. Achados do caso que FAVORECEM esta hipótese
4. Achados do caso que VÃO CONTRA esta hipótese
5. Próximo exame ou teste mais importante para confirmar/excluir
6. Sinal de alarme ("red flag") que, se presente, eleva a urgência

Ao final, apresente:
- Resumo da hipótese mais provável com justificativa
- Proposta de investigação sequencial (do mais simples/disponível ao mais complexo)
- Condições que exigem ação imediata ("não pode esperar")

RESTRIÇÕES:
- Considere a disponibilidade de exames no SUS e na rede privada brasileira
- Não sugira tratamento — foque apenas no diagnóstico diferencial
- Inclua pelo menos 5 hipóteses, mesmo que algumas sejam menos prováveis
- Cite se alguma hipótese exige notificação compulsória
```

---

## Dicas de uso

- **Seja específico nos achados negativos**: informar o que o paciente NÃO tem é tão importante quanto o que tem. Por exemplo, "nega febre, nega perda de peso" ajuda a IA a excluir hipóteses infecciosas e neoplásicas.
- **Inclua resultados de exames com valores numéricos**: em vez de "glicemia alterada", escreva "glicemia de jejum 118 mg/dL". Quanto mais preciso o input, melhor o output.
- **Use o template como checklist mental**: mesmo que você já tenha uma hipótese forte, o exercício de preencher todos os campos pode revelar dados que você não havia considerado.
- **Revise criticamente a resposta da IA**: o diagnóstico diferencial gerado é um ponto de partida para seu raciocínio, nunca uma conclusão definitiva. Confronte com sua experiência clínica e com as diretrizes vigentes.

---

## Variações possíveis

| Variação | O que mudar no template |
|---|---|
| **Caso pediátrico** | Altere a role para "pediatra" e adicione campos: idade gestacional ao nascer, vacinação, marcos do desenvolvimento |
| **Caso de urgência/emergência** | Adicione ao comando: "Priorize hipóteses que exigem intervenção nas próximas 2 horas" |
| **Segunda opinião** | Adicione ao contexto: "Hipótese inicial do médico assistente: [diagnóstico]. Questione essa hipótese e apresente alternativas" |
| **Foco em uma especialidade** | Altere a role e adicione: "Considere apenas diagnósticos dentro do escopo da [ESPECIALIDADE]" |
| **Medicina rural / cidade pequena** | Adicione às restrições: "Considere que o serviço dispõe apenas de: RX simples, ECG, hemograma, EAS, glicemia capilar. Hospital de referência a 120 km" |
