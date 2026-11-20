# Guia Pratico: Anonimizacao de Dados do Paciente

**Objetivo:** Ensinar como remover dados identificaveis do paciente ANTES de inserir qualquer informacao clinica em ferramentas de IA.
**Regra de ouro:** Na duvida, remova. E mais seguro anonimizar demais do que de menos.

---

## Por Que Anonimizar?

- A LGPD classifica dados de saude como **dados sensiveis** — exigem protecao redobrada.
- Ferramentas de IA externas (ChatGPT, Claude, Gemini, etc.) nao sao sistemas de saude certificados.
- Mesmo com politicas de privacidade favoraveis, dados identificaveis nao devem ser inseridos em plataformas de terceiros.
- A Resolucao CFM 2.454/2026 reforça a responsabilidade do medico sobre a protecao dos dados do paciente.

---

## O Que REMOVER (Sempre)

Estes dados devem ser **removidos ou substituidos** antes de inserir em qualquer ferramenta de IA:

| Dado | Risco | Como Substituir |
|---|---|---|
| **Nome completo** | Identificacao direta | "Paciente" ou "Sr(a). X" |
| **CPF** | Identificacao direta | Remover completamente |
| **RG** | Identificacao direta | Remover completamente |
| **Data de nascimento completa** | Identificacao indireta | Usar apenas a idade: "45 anos" |
| **Endereco** | Identificacao indireta | Remover ou usar "zona urbana/rural" |
| **Telefone** | Identificacao direta | Remover completamente |
| **E-mail** | Identificacao direta | Remover completamente |
| **Nome de familiares** | Identificacao indireta | "Mae do paciente", "Conjugue" |
| **Local de trabalho** | Identificacao indireta | Usar apenas a profissao: "trabalhador rural" |
| **Numero de prontuario** | Identificacao direta | Remover completamente |
| **Plano de saude e carteirinha** | Identificacao indireta | Remover ou usar "conveniado" |
| **Fotos com rosto visivel** | Identificacao direta | Nao inserir em ferramentas de IA |
| **Nome da instituicao** | Identificacao indireta | "Hospital de referencia" |
| **Datas especificas de internacao** | Identificacao indireta | "Internado ha 3 dias" |

---

## O Que PODE Ficar (Geralmente Seguro)

Estes dados clinicos geralmente podem ser mantidos, pois sao necessarios para o raciocinio clinico e nao identificam o paciente isoladamente:

| Dado | Exemplo |
|---|---|
| **Idade** | "45 anos" |
| **Sexo/genero** | "Masculino" |
| **Comorbidades** | "HAS, DM2, dislipidemia" |
| **Medicacoes em uso** (sem dosagem unica identificavel) | "Metformina, losartana" |
| **Sinais e sintomas** | "Dor toracica, dispneia aos esforcos" |
| **Resultados de exames** (sem identificacao) | "HbA1c 8,2%, Cr 1,5" |
| **Historia da doenca atual** (anonimizada) | "Paciente, 45 anos, masculino, com queixa de..." |
| **Antecedentes** (genericos) | "Tabagista 20 macos-ano, ex-etilista" |
| **Hipoteses diagnosticas** | "Sindrome coronariana aguda" |

---

## Exemplos Praticos: Antes e Depois

### Exemplo 1: Consulta ambulatorial

**ANTES (NAO insira isso na IA):**
```
Joao Carlos da Silva, CPF 123.456.789-00, nascido em 15/03/1980,
morador da Rua das Flores, 123, Belo Horizonte. Paciente do
Dr. Roberto Almeida, Hospital Santa Casa. Internado em 05/04/2026.
Queixa de dor toracica ha 2 dias. HAS, DM2. Usa metformina 850mg
e losartana 50mg. ECG com supra de ST em parede anterior.
```

**DEPOIS (versao anonimizada — pode inserir):**
```
Paciente masculino, 45 anos. Queixa de dor toracica ha 2 dias.
Comorbidades: HAS, DM2. Uso de metformina e losartana.
ECG com supra de ST em parede anterior. Internado ha 7 dias
em hospital de referencia.
```

### Exemplo 2: Pedido de diagnostico diferencial

**ANTES (NAO insira isso):**
```
Maria Aparecida Santos, 68 anos, de Campinas-SP, paciente da
Unimed, prontuario 2024-5678. Filha relata que Dona Maria
comecou com confusao mental ha 3 dias. Na 2,5 mg/dL.
```

**DEPOIS (versao anonimizada):**
```
Paciente feminina, 68 anos. Familiar relata inicio de confusao
mental ha 3 dias. Laboratorio: Na 125 mEq/L. Solicito
diagnostico diferencial para hiponatremia com alteracao
do nivel de consciencia.
```

### Exemplo 3: Resumo para discussao de caso

**ANTES (NAO insira isso):**
```
Pedro, 12 anos, filho de Ana e Carlos Oliveira, estudante do
Colegio Santo Agostinho, encaminhado pelo Dr. Marcos da UBS
Vila Nova em 10/04/2026.
```

**DEPOIS (versao anonimizada):**
```
Paciente masculino, 12 anos, encaminhado de unidade basica de
saude para investigacao de [motivo].
```

---

## Checklist Rapido de Anonimizacao

Antes de colar o texto na ferramenta de IA, verifique:

- [ ] Removi todos os nomes (paciente, familiares, profissionais, instituicoes)
- [ ] Removi CPF, RG e numero de prontuario
- [ ] Substituí data de nascimento por idade
- [ ] Removi endereco e telefone
- [ ] Removi datas especificas (substituí por intervalos: "ha 3 dias")
- [ ] Removi nome do convênio e numero de carteirinha
- [ ] Reli o texto completo buscando qualquer dado que possa identificar o paciente

---

## Fluxo Recomendado

```
TEXTO ORIGINAL DO PRONTUARIO
          |
          v
   [Anonimizar com este guia]
          |
          v
   [Reler e verificar]
          |
          v
   TEXTO ANONIMIZADO --> Pode inserir na ferramenta de IA
```

---

## Dicas Importantes

1. **Crie o habito.** Com pratica, a anonimizacao leva menos de 1 minuto.
2. **Use um editor de texto intermediario.** Nao copie direto do prontuario para a IA. Cole num bloco de notas, anonimize, depois cole na ferramenta.
3. **Cuidado com dados indiretos.** Combinacoes raras (doenca rara + idade + cidade pequena) podem identificar um paciente mesmo sem nome.
4. **Imagens clinicas:** Pode usar fotos de lesoes, exames de imagem, etc., desde que nao contenham nome, rosto, ou dados identificaveis visiveis.
5. **Na duvida, nao inclua.** Se um dado nao e necessario para a pergunta que voce esta fazendo a IA, nao inclua.

---

*Material educacional do curso IAMed - Nivel 1: Fundacao.*
