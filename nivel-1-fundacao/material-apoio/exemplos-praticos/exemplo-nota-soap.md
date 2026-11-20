# Exemplo Pratico 3: Geracao de Nota Clinica no Formato SOAP

## Contexto Clinico

**Cenario:** Dra. Camila, endocrinologista em clinica particular em Goiania, atende retorno de paciente com diabetes tipo 2. Ela dita as informacoes da consulta e usa a IA para estruturar a nota no formato SOAP para inserir no prontuario eletronico.

**Paciente:** Jose Carlos, 58 anos, masculino, aposentado, diabetico tipo 2 ha 8 anos.

**Informacoes da consulta (ditadas pela medica):**
> "Retorno de 3 meses. Paciente refere que esta tomando a metformina direitinho, 850 tres vezes ao dia, mas nao conseguiu fazer a dieta. Nao esta fazendo atividade fisica. Trouxe exames: HbA1c veio 8.2%, glicemia de jejum 165, creatinina 0.9, TFGe 88, colesterol total 210, LDL 135, HDL 38, triglicerideos 245, microalbuminuria negativa. Fundo de olho do ano passado normal. Exame do pe: monofilamento normal, pulsos presentes. Peso 92kg, altura 1.72m, PA 138/86. Vou adicionar gliclazida MR 60mg no cafe e pedir pra ele voltar em 3 meses com novos exames. Orientei dieta e caminhada."

---

## O Prompt Usado

```
Voce e uma assistente medica especializada em documentacao clinica. 
Estruture as informacoes abaixo no formato SOAP completo para prontuario 
eletronico. Inclua o CID-10 adequado.

INFORMACOES DA CONSULTA:
[informacoes ditadas acima foram coladas aqui]

FORMATO: SOAP padrao com subsecoes. Inclua:
- S (Subjetivo): queixas e relatos do paciente
- O (Objetivo): exame fisico e exames complementares
- A (Avaliacao): diagnosticos com CID-10, analise da evolucao
- P (Plano): condutas, prescricoes, orientacoes, retorno

Linguagem tecnica, objetiva, pronta para inserir no prontuario.
```

---

## Resposta da IA

> ## NOTA CLINICA — FORMATO SOAP
>
> **Paciente:** J.C.S., 58 anos, masculino
> **Data:** [data da consulta]
> **Tipo:** Consulta de retorno — Endocrinologia
>
> ---
>
> ### S — SUBJETIVO
>
> Paciente em retorno de 3 meses para reavaliacao de diabetes mellitus tipo 2. Relata adesao regular a metformina 850 mg 3x/dia. Nega hipoglicemia, poliuria ou polidipsia. Refere dificuldade em manter dieta adequada e nao iniciou programa de atividade fisica conforme orientado na consulta anterior. Sem queixas visuais, dor em membros inferiores ou lesoes em pes. Nega dor toracica, dispneia ou edema.
>
> ### O — OBJETIVO
>
> **Sinais vitais e antropometria:**
> - Peso: 92 kg | Altura: 1.72 m | IMC: 31.1 kg/m2 (Obesidade grau I)
> - PA: 138/86 mmHg
>
> **Exame fisico dirigido:**
> - Pes: teste do monofilamento 10g normal bilateralmente, pulsos pedioso e tibial posterior presentes e simetricos
> - Sem lesoes cutaneas em membros inferiores
>
> **Exames complementares (data dos exames):**
> | Exame | Resultado | Referencia |
> |-------|-----------|------------|
> | HbA1c | 8.2% | <7.0% |
> | Glicemia de jejum | 165 mg/dL | 70-99 mg/dL |
> | Creatinina | 0.9 mg/dL | 0.7-1.2 mg/dL |
> | TFGe (CKD-EPI) | 88 mL/min/1.73m2 | >60 |
> | Colesterol total | 210 mg/dL | <190 mg/dL |
> | LDL-c | 135 mg/dL | <100 mg/dL* |
> | HDL-c | 38 mg/dL | >40 mg/dL |
> | Triglicerideos | 245 mg/dL | <150 mg/dL |
> | Microalbuminuria | Negativa | Negativa |
>
> *Meta de LDL para diabetico: <100 mg/dL (ou <70 se alto risco CV)
>
> **Rastreamento de complicacoes:**
> - Fundo de olho (ultimo: ha 1 ano): normal
> - Neuropatia periferica: sem evidencia clinica (monofilamento normal)
> - Nefropatia: sem albuminuria, TFGe preservada
>
> ### A — AVALIACAO
>
> 1. **Diabetes mellitus tipo 2 com controle glicemico inadequado** — CID-10: E11.9
>    - HbA1c 8.2% (meta <7.0%), apesar de metformina em dose plena
>    - Necessidade de intensificacao terapeutica
>    - Sem complicacoes microvasculares detectaveis ate o momento
>
> 2. **Obesidade grau I** — CID-10: E66.0
>    - IMC 31.1, sem adesao a mudancas de estilo de vida
>
> 3. **Dislipidemia mista** — CID-10: E78.2
>    - LDL 135 (acima da meta), HDL 38 (baixo), TG 245 (elevado)
>    - Risco cardiovascular aumentado — considerar estatina
>
> 4. **Hipertensao arterial em investigacao** — CID-10: I10
>    - PA 138/86 em consultorio — confirmar em proximas consultas ou MAPA
>
> ### P — PLANO
>
> **Farmacologico:**
> 1. Manter metformina 850 mg — 1 cp cafe, 1 cp almoco, 1 cp jantar
> 2. **Iniciar gliclazida MR 60 mg — 1 cp no cafe da manha**
> 3. Considerar inicio de estatina (atorvastatina 20 mg) na proxima consulta apos novo perfil lipidico — paciente diabetico com LDL >100 tem indicacao
>
> **Nao farmacologico:**
> - Reforco de orientacao dietetica: encaminhamento para nutricionista
> - Atividade fisica: caminhada 150 min/semana (30 min, 5x/semana), inicio gradual
> - Meta de perda de peso: 5-7% do peso corporal (4.5-6.5 kg)
>
> **Exames solicitados para retorno:**
> - HbA1c
> - Glicemia de jejum
> - Perfil lipidico completo
> - Creatinina + TFGe
> - Relacao albumina/creatinina urinaria
>
> **Retorno:** 3 meses
>
> **Metas terapeuticas:**
> - HbA1c <7.0%
> - PA <130/80 mmHg
> - LDL <100 mg/dL (idealmente <70 por risco CV)
>
> ---
> *Nota gerada com auxilio de IA — revisada e validada pelo medico assistente.*

---

## Avaliacao Critica do Medico

### O que a IA ACERTOU

1. **Estrutura SOAP impecavel.** A nota esta bem organizada, com subsecoes claras, linguagem tecnica adequada e pronta para prontuario eletronico.

2. **IMC calculado corretamente.** 92/(1.72)2 = 31.1 — correto, e a classificacao como obesidade grau I esta certa.

3. **Tabela de exames com referencias.** Muito util para visualizacao rapida. Os valores de referencia estao corretos.

4. **Identificacao de problemas nao mencionados explicitamente.** A IA identificou a dislipidemia mista e a PA elevada como problemas adicionais, mesmo que a medica nao tenha destacado na ditadura. Isso demonstra capacidade de raciocinio clinico basico.

5. **Meta de LDL para diabetico.** Corretamente apontou que a meta e <100 (ou <70 se alto risco).

6. **Sugestao de nutricionista e estatina.** Pertinentes e alinhadas com boas praticas, embora a medica nao tenha mencionado explicitamente.

### O que a IA ERROU

1. **CID-10 INCORRETO para o diagnostico principal.** A IA usou **E11.9** (Diabetes mellitus tipo 2 sem complicacoes). No contexto desta consulta, o CID mais adequado seria **E11.65** (Diabetes mellitus tipo 2 com hiperglicemia) ou manter E11.9 caso se considere que nao ha complicacoes documentadas. Porem, o ponto critico e outro: o CID **E11.9** e frequentemente usado de forma generica, e para fins de faturamento em convenio ou registro adequado, o CID deveria refletir o controle inadequado. Na classificacao CID-10 brasileira usada pelo DATASUS, o codigo **E11.9** realmente significa "sem complicacoes", mas nao existe um codigo especifico para "controle inadequado" no CID-10 (isso existe no CID-11 e no sistema americano). Portanto, **E11.9 e tecnicamente aceitavel no Brasil, mas a IA nao explicou esse nuance.** O erro real e que em contextos de faturamento com convenios, usar E11.9 para um paciente com HbA1c 8.2% pode ser questionado — alguns convenios e auditorias preferem E11.65 (que na verdade nao existe na versao padrao do CID-10, sendo um codigo da ICD-10-CM americana). **A IA misturou codigos de sistemas diferentes sem alertar.**

   **Nota didatica:** Este e um ponto de confusao real na pratica medica brasileira. O CID-10 da OMS (usado no Brasil) tem codigos diferentes do ICD-10-CM (usado nos EUA). A IA frequentemente mistura os dois sistemas. O correto no Brasil seria E11.8 (DM2 com complicacoes nao especificadas) ou E11.9 (sem complicacoes), dependendo da interpretacao.

2. **Adicionou informacoes nao fornecidas.** A IA incluiu "Nega hipoglicemia, poliuria ou polidipsia" e "Nega dor toracica, dispneia ou edema" no subjetivo. A medica **nao ditou** essas negativas. A IA esta "preenchendo" a nota com negativas pertinentes, o que e uma pratica documentacional aceitavel, mas **registrar em prontuario algo que nao foi efetivamente perguntado ao paciente e um risco medicolegal.** Se houver questionamento judicial, a medica teria dificuldade de confirmar que realmente interrogou esses sintomas.

3. **Sugestao de estatina nao solicitada.** A medica nao mencionou estatina em sua ditadura, e a IA sugeriu "considerar inicio de atorvastatina". Embora clinicamente correto (LDL 135 em diabetico tem indicacao), o prontuario deve refletir a conduta **real** da medica, nao sugestoes da IA. A nota deveria ter separado: "conduta realizada" vs. "sugestoes para consideracao".

### O que e PERIGOSO

- **Registro de informacao nao coletada.** Colocar no prontuario que o paciente "nega" sintomas que nao foram perguntados e falsificacao documental involuntaria. Em caso de evento adverso (ex: paciente infarta meses depois), a defesa poderia argumentar: "consta no prontuario que o paciente negou dor toracica — a medica investigou e descartou". Isso cria um registro falso.

- **Mistura de sistemas de codificacao.** Usar codigos ICD-10-CM (americano) em prontuarios brasileiros pode causar problemas com o faturamento TISS/TUSS junto a operadoras de saude.

---

## Licao Aprendida

A IA e excelente para estruturar notas clinicas — a organizacao, formatacao e linguagem tecnica sao de alta qualidade. No entanto, existem dois riscos sistematicos:

1. **A IA "completa" informacoes que nao foram fornecidas.** Ela tende a gerar uma nota clinica "ideal" com todas as negativas pertinentes, mesmo que o medico nao tenha perguntado. Isso e util como lembrete (voce esqueceu de perguntar sobre X?), mas perigoso se for direto para o prontuario sem revisao.

2. **Codificacao CID-10 e uma area de alto risco para IA.** A mistura entre sistemas de codificacao (OMS vs. americano) e frequente e pode causar problemas administrativos e de faturamento.

A regra e: **a IA gera o rascunho, o medico revisa, confirma que cada informacao foi realmente coletada, e so entao insere no prontuario.**

---

## Como Melhorar o Prompt

1. **Explicitar o que NAO incluir:**
   ```
   RESTRICAO: Inclua APENAS as informacoes que eu forneci. Nao adicione 
   negativas de sintomas que nao foram mencionadas. Se achar que falta 
   informacao relevante, liste ao final como "SUGESTAO: perguntar sobre..."
   ```

2. **Especificar o sistema de codificacao:**
   ```
   Use EXCLUSIVAMENTE codigos CID-10 da versao OMS/DATASUS (Brasil). 
   Nao use codigos ICD-10-CM americanos. Em caso de duvida, indique 
   "CID a confirmar".
   ```

3. **Separar conduta real de sugestoes:**
   ```
   Divida o Plano em:
   - CONDUTAS REALIZADAS (apenas o que eu informei)
   - SUGESTOES DA IA (para minha consideracao, nao para o prontuario)
   ```

4. **Incluir checklist de revisao:**
   ```
   Ao final da nota, adicione uma secao "CHECKLIST DE REVISAO" com:
   [ ] Todas as informacoes registradas foram coletadas na consulta?
   [ ] CID-10 verificado no DATASUS?
   [ ] Conduta reflete o que foi realmente prescrito?
   ```

---

**Veredicto final:** A geracao de notas SOAP e provavelmente um dos usos mais produtivos da IA na pratica clinica diaria — economiza tempo significativo. Mas o fluxo correto e: IA gera rascunho, medico revisa cada linha contra o que realmente aconteceu na consulta, corrige, e so entao salva no prontuario.
