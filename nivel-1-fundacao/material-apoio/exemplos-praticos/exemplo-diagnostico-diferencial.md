# Exemplo Pratico 1: Diagnostico Diferencial com Framework RCCFR

## Contexto Clinico

**Cenario:** Ambulatorio de clinica medica em hospital universitario de Belo Horizonte. Medica generalista atende paciente sem neurologista disponivel no momento.

**Paciente:** Maria Aparecida, 45 anos, sexo feminino, parda, professora do ensino fundamental.

**Queixa principal:** "Dor de cabeca forte e perdi a visao do olho direito por uns minutos."

**Historia da doenca atual:**
- Cefaleia hemicraniana esquerda, pulsatil, intensidade 8/10, iniciada ha 3 dias
- Episodio de perda visual monocular direita (amaurose fugaz) ha 2 dias, duracao de aproximadamente 5 minutos, com recuperacao completa
- Segundo episodio de turvacao visual hoje pela manha, duracao de 2-3 minutos
- Nauseas eventuais, sem vomitos
- Nega febre, trauma, uso de drogas ilicitas

**Antecedentes:**
- Enxaqueca com aura visual desde os 20 anos (diagnosticada, sem acompanhamento regular)
- Uso de anticoncepcional oral combinado (etinilestradiol + levonorgestrel) ha 15 anos
- Tabagista — 10 macos/ano
- IMC 28
- Sem historia familiar de AVC ou doencas autoimunes

**Exame fisico:**
- PA 148/92 mmHg, FC 78 bpm, temperatura 36.5C
- Exame neurologico: sem deficits focais no momento da consulta
- Fundoscopia: dificil visualizacao, sem papiledema evidente
- Ausculta de carotidas: sopro cervical a direita

---

## O Prompt Usado (Framework RCCFR)

```
ROLE: Voce e um neurologista clinico com experiencia em cefaleias e doencas cerebrovasculares, atuando em hospital universitario brasileiro.

CONTEXTO: Paciente feminina, 45 anos, apresentando cefaleia hemicraniana esquerda pulsatil (8/10) ha 3 dias associada a dois episodios de amaurose fugaz monocular direita (5 min e 2-3 min, com recuperacao completa). Antecedentes: enxaqueca com aura desde os 20 anos, uso de ACO combinado ha 15 anos, tabagismo 10 macos/ano, IMC 28. Exame: PA 148/92, sopro carotideo a direita, sem deficits focais atuais, fundoscopia sem papiledema evidente.

COMANDO: Liste os 5 diagnosticos diferenciais mais provaveis em ordem de probabilidade, com justificativa clinica para cada um. Para cada diagnostico, indique: (a) exames complementares prioritarios, (b) conduta inicial, (c) criterio de urgencia (emergencia, urgencia ou ambulatorial).

FORMATO: Tabela com colunas: Diagnostico | Probabilidade estimada | Justificativa | Exames prioritarios | Conduta inicial | Urgencia

RESTRICAO: Base suas recomendacoes nas diretrizes brasileiras (quando disponiveis) e internacionais atualizadas. Nao invente referencias. Se nao tiver certeza de uma dosagem, diga explicitamente.
```

---

## Resposta da IA

> **Diagnostico Diferencial — Cefaleia + Amaurose Fugaz em Mulher de 45 Anos**
>
> | # | Diagnostico | Probabilidade | Justificativa | Exames Prioritarios | Conduta Inicial | Urgencia |
> |---|-------------|---------------|---------------|---------------------|-----------------|----------|
> | 1 | Doenca ateromatosa carotidea com AIT (ataque isquemico transitorio) | Alta | Amaurose fugaz monocular e o sintoma classico de AIT no territorio da arteria oftalmica/carotida interna. Sopro carotideo a direita corrobora. Fatores de risco: tabagismo, HAS, ACO. | Doppler de carotidas e vertebrais, angiotomografia cervical e craniana, hemograma, perfil lipidico, glicemia, ECG | AAS 300 mg dose de ataque seguido de 100 mg/dia. Estatina de alta potencia (atorvastatina 80 mg/dia). Anti-hipertensivo. Suspender ACO combinado. | EMERGENCIA |
> | 2 | Enxaqueca com aura prolongada / aura retiniana | Moderada-alta | Historia previa de enxaqueca com aura. Cefaleia pulsatil hemicraniana e compativel. Porem, amaurose fugaz monocular nao e apresentacao tipica de aura — a aura visual classica e binocular (cortical). | RM de cranio com angioressonancia | Analgesia para crise (sumatriptano 50 mg VO). Profilaxia se recorrente. Suspender ACO combinado (enxaqueca com aura e contraindicacao). | URGENCIA |
> | 3 | Disseccao de arteria carotida interna | Moderada | Pode causar cefaleia ipsilateral + sintomas isquemicos no territorio carotideo. Embora mais comum em jovens e apos trauma, pode ocorrer espontaneamente. | Angiotomografia ou angioressonancia cervical (protocolo para disseccao com cortes axiais em T1 com supressao de gordura) | Anticoagulacao com heparina seguida de varfarina (alvo INR 2-3) por 3-6 meses. Alternativa: AAS em casos leves. **Dose de heparina: bolus 80 UI/kg seguido de infusao 18 UI/kg/h.** | EMERGENCIA |
> | 4 | Arterite de celulas gigantes (arterite temporal) | Baixa-moderada | Idade de 45 anos esta abaixo da faixa tipica (>50 anos), mas nao exclui. Cefaleia nova + sintomas visuais devem levantar suspeita. | VHS, PCR, hemograma (anemia, trombocitose), biopsia de arteria temporal se marcadores inflamatorios elevados | Se alta suspeita: **prednisona 1 mg/kg/dia (60-80 mg/dia) iniciada empiricamente antes da biopsia** para evitar perda visual definitiva. | EMERGENCIA |
> | 5 | Sindrome antifosfolipide | Baixa | Mulher em idade fertil com eventos isquemicos recorrentes. ACO e um fator que potencializa o risco trombotico nessa sindrome. | Anticorpo anticardiolipina (IgG e IgM), anticoagulante lupico, anti-beta2 glicoproteina I. Repetir em 12 semanas para confirmacao. | Anticoagulacao se confirmada. Suspender ACO. | URGENCIA |
>
> **Observacoes adicionais:**
> - A suspensao do anticoncepcional oral combinado e imperativa independentemente do diagnostico final — a paciente apresenta multiplos fatores de risco cardiovascular (tabagismo, HAS, enxaqueca com aura, >35 anos).
> - Recomendo internacao hospitalar para investigacao de AIT conforme escore ABCD2 (provavel >= 4 pontos neste caso).
> - De acordo com o guideline da American Heart Association 2019 para manejo de AIT, pacientes com ABCD2 >= 4 devem ser investigados em regime de urgencia nas primeiras 24 horas.
> - Considerar ecocardiograma transtoracico e Holter 24h para excluir fonte cardioembolica.

---

## Avaliacao Critica do Medico

### O que a IA ACERTOU

1. **Priorizacao diagnostica correta.** Colocar AIT por doenca carotidea como primeira hipotese e adequado. Amaurose fugaz monocular com sopro carotideo ipsilateral e um quadro classico que nao pode ser ignorado.

2. **Suspensao do ACO.** A IA identificou corretamente que o anticoncepcional combinado deve ser suspenso independentemente do diagnostico — isso esta alinhado com os criterios de elegibilidade da OMS para contraceptivos.

3. **Consideracao de disseccao carotidea.** Boa lembranca — embora menos provavel sem historia de trauma, a disseccao espontanea e um diagnostico que nao pode ser esquecido nessa faixa etaria.

4. **Diferenciacao aura vs. amaurose.** A IA acertou ao pontuar que aura visual tipica de enxaqueca e binocular (cortical), e amaurose fugaz monocular sugere patologia retiniana/vascular, nao cortical.

5. **Recomendacao de internacao com escore ABCD2.** Pertinente e bem fundamentada.

### O que a IA ERROU

1. **Dosagem de AAS no AIT.** A IA recomendou "AAS 300 mg dose de ataque seguido de 100 mg/dia". Na verdade, a dose de ataque recomendada pela diretriz brasileira de AVC (Academia Brasileira de Neurologia, 2023) e pela AHA/ASA e de **160-325 mg**, e a dose de manutencao mais utilizada no Brasil e **100 mg/dia** (aceitavel) ou **81-325 mg/dia** (AHA). O valor de 300 mg esta dentro da faixa, mas a IA apresentou como se fosse a dose exata recomendada, sem mencionar a faixa. **Isso poderia induzir a um falso senso de precisao.**

2. **Guideline citado esta incompleto/impreciso.** A IA mencionou "guideline da American Heart Association 2019 para manejo de AIT". O documento mais relevante e o "2021 Guideline for the Prevention of Stroke in Patients With Stroke and Transient Ischemic Attack" (AHA/ASA 2021, Kleindorfer et al.). O de 2019 existe (manejo de AVC agudo), mas nao e especifico para AIT. **A IA misturou documentos.**

3. **Dose de heparina na disseccao.** A IA citou "bolus 80 UI/kg seguido de infusao 18 UI/kg/h". Essa e a dose padrao de heparina para TEV/SCA, mas na disseccao carotidea a decisao de anticoagular versus antiagregar e controversa, e a IA apresentou a anticoagulacao como se fosse conduta padrao. As diretrizes mais recentes (CADISS trial, Lancet Neurology 2015) mostraram equivalencia entre anticoagulacao e antiagregacao. **A IA nao mencionou essa controversia.**

4. **Arterite temporal — idade.** A IA corretamente notou que 45 anos esta abaixo da faixa tipica, mas ainda assim colocou como "baixa-moderada". Na pratica, arterite de celulas gigantes em menores de 50 anos e rara (prevalencia <2% dos casos). A probabilidade deveria ser classificada como "baixa" ou "muito baixa", nao "baixa-moderada".

### O que e PERIGOSO

- **Sugerir sumatriptano** na segunda hipotese e potencialmente perigoso neste contexto. Se o quadro real for AIT ou disseccao carotidea, triptanos sao contraindicados (vasoconstricao). A IA deveria ter colocado um alerta explicito: "NAO administrar triptanos ate excluir causa vascular."
- A dose de prednisona para arterite temporal (1 mg/kg/dia) esta correta, mas iniciar corticoide empiricamente em uma paciente de 45 anos sem VHS/PCR elevados seria questionavel. A IA deveria ter condicionado melhor: "solicitar VHS e PCR de urgencia; iniciar corticoide se marcadores elevados ou perda visual em andamento."

---

## Licao Aprendida

A IA demonstrou um raciocinio clinico estruturado e abrangente — o diagnostico diferencial esta bem construido e seria util como ponto de partida. No entanto, ela apresentou informacoes imprecisas com tom de certeza (dosagens, guidelines), o que e o tipo de erro mais perigoso: **parece confiavel mas contem imprecisoes que so um medico atento detectaria.**

O maior risco nao foi o que a IA disse de errado — foi o que ela **deixou de alertar** (contraindicacao de triptano com suspeita vascular ativa).

---

## Como Melhorar o Prompt

1. **Adicionar restricao de seguranca explicita:**
   ```
   RESTRICAO ADICIONAL: Para cada hipotese, liste explicitamente 
   contraindicacoes da conduta proposta caso outra hipotese do diferencial 
   seja o diagnostico real.
   ```

2. **Pedir intervalos ao inves de valores fixos:**
   ```
   Para dosagens, indique a FAIXA terapeutica recomendada (minimo-maximo) 
   e a fonte especifica (nome do guideline, ano, organizacao).
   ```

3. **Solicitar grau de certeza da IA:**
   ```
   Para cada recomendacao de conduta, classifique seu nivel de confianca 
   como ALTO, MEDIO ou BAIXO, e justifique.
   ```

4. **Pedir verificacao cruzada:**
   ```
   Ao final, revise sua propria resposta: alguma conduta sugerida para 
   uma hipotese seria perigosa se outra hipotese for verdadeira?
   ```

---

**Veredicto final:** A IA foi util como ferramenta de brainstorming diagnostico e organizacao do raciocinio. Mas **nao substitui a avaliacao clinica integrada** — neste caso, o sopro carotideo + amaurose fugaz monocular exigia encaminhamento emergencial para neurologia vascular, e nenhum prompt de IA muda isso.
