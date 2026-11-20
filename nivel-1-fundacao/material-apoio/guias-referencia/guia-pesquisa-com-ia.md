# Guia Pratico: Pesquisa Cientifica Acelerada com IA

**Objetivo:** Aprender um fluxo de trabalho pratico para encontrar, avaliar e sintetizar evidencia cientifica usando ferramentas de IA.
**Tempo estimado:** 20-30 minutos para aprender o fluxo; depois, 10-15 minutos por pesquisa.

---

## O Stack de Pesquisa

Cada ferramenta tem um papel especifico no fluxo:

| Etapa | Ferramenta | Papel |
|---|---|---|
| 1. Pergunta | Claude ou ChatGPT | Refinar a pergunta clinica (formato PICO) |
| 2. Busca | Elicit + Consensus | Encontrar artigos relevantes |
| 3. Contexto | Semantic Scholar | Mapear conexoes e artigos influentes |
| 4. Validacao | scite | Verificar como a evidencia e citada |
| 5. Sintese | Claude | Resumir e integrar os achados |

---

## Passo a Passo

### Passo 1: Refinar a Pergunta Clinica

**Ferramenta:** Claude ou ChatGPT

Antes de buscar, transforme sua duvida em uma pergunta estruturada. Use o formato PICO.

**Prompt sugerido:**

```
Sou medico [sua especialidade]. Tenho a seguinte duvida clinica:
[descreva sua duvida em linguagem natural]

Por favor, ajude-me a estruturar isso no formato PICO:
- P (Populacao):
- I (Intervencao):
- C (Comparacao):
- O (Outcome/Desfecho):

Tambem sugira 3 termos de busca em ingles para PubMed/Elicit.
```

**Exemplo de resultado:**

```
P: Adultos com diabetes tipo 2
I: Uso de inibidores SGLT2
C: Metformina isolada
O: Reducao de eventos cardiovasculares

Termos sugeridos:
1. "SGLT2 inhibitors cardiovascular outcomes type 2 diabetes"
2. "empagliflozin vs metformin cardiovascular"
3. "dapagliflozin heart failure diabetes"
```

---

### Passo 2: Busca de Artigos

**Ferramenta:** Elicit

1. Acesse https://elicit.com
2. Cole sua pergunta em linguagem natural (em ingles, para melhores resultados):
   - Exemplo: "Do SGLT2 inhibitors reduce cardiovascular events in type 2 diabetes compared to metformin alone?"
3. O Elicit retorna uma tabela com artigos relevantes, incluindo:
   - Titulo e autores
   - Resumo dos achados principais
   - Metodologia (RCT, meta-analise, coorte, etc.)
   - Tamanho da amostra
4. **Filtre** por tipo de estudo (priorize meta-analises e RCTs)
5. **Exporte** os 5-10 artigos mais relevantes

**Ferramenta complementar:** Consensus

1. Acesse https://consensus.app
2. Faca a mesma pergunta
3. O Consensus mostra um "medidor de consenso" — qual a tendencia geral da literatura
4. Compare os resultados com o que o Elicit encontrou

> Dica: Consensus e melhor para perguntas do tipo "sim ou nao". Elicit e melhor para perguntas exploratórias.

---

### Passo 3: Mapear o Contexto

**Ferramenta:** Semantic Scholar

1. Acesse https://semanticscholar.org
2. Busque os artigos-chave que voce encontrou no Passo 2
3. Para cada artigo importante, observe:
   - **Highly Influential Citations:** quais artigos foram mais impactados por este
   - **References:** quais sao as fontes fundamentais
   - **TLDR:** resumo de uma frase gerado por IA
4. Identifique os "artigos ancora" — aqueles mais citados e influentes no tema

> Dica: Se um artigo tem muitas "highly influential citations", provavelmente e um estudo fundamental no tema.

---

### Passo 4: Validar a Evidencia

**Ferramenta:** scite

1. Acesse https://scite.ai
2. Busque os artigos-chave do seu tema
3. Para cada artigo, o scite mostra:
   - **Supporting citations:** citacoes que apoiam os achados
   - **Contrasting citations:** citacoes que contradizem ou questionam
   - **Mentioning citations:** citacoes neutras
4. **Atencao especial** aos artigos com muitas citacoes contrastantes — pode indicar evidencia controversa

**Pergunte-se:**
- Os achados principais sao mais apoiados ou contestados pela literatura subsequente?
- Houve estudos mais recentes que mudaram o consenso?

---

### Passo 5: Sintetizar com IA

**Ferramenta:** Claude

Agora que voce tem os artigos-chave, use Claude para criar uma sintese.

**Prompt sugerido:**

```
Sou medico [especialidade] e fiz uma revisao rapida sobre [tema].
Encontrei os seguintes artigos-chave:

1. [Titulo do artigo 1] - [achado principal]
2. [Titulo do artigo 2] - [achado principal]
3. [Titulo do artigo 3] - [achado principal]
[...]

Com base nesses achados, por favor:
1. Faca uma sintese de 1 paragrafo sobre o estado atual da evidencia
2. Identifique pontos de consenso e controversia
3. Sugira a implicacao pratica para minha conduta clinica
4. Aponte limitacoes e lacunas que encontrou

Importante: se algo nao esta claro nos dados que forneci, diga explicitamente
em vez de preencher com suposicoes.
```

---

## Fluxo Visual Resumido

```
DUVIDA CLINICA
     |
     v
[Claude] --> Pergunta PICO + termos de busca
     |
     v
[Elicit + Consensus] --> Artigos relevantes + tendencia da literatura
     |
     v
[Semantic Scholar] --> Artigos ancora + conexoes
     |
     v
[scite] --> Validacao: a evidencia e apoiada ou contestada?
     |
     v
[Claude] --> Sintese final com implicacao pratica
     |
     v
DECISAO CLINICA INFORMADA (sua, nao da IA)
```

---

## Erros Comuns a Evitar

1. **Aceitar o primeiro resultado sem verificar.** Sempre cruze informacoes entre pelo menos 2 ferramentas.
2. **Pesquisar apenas em portugues.** A maioria da literatura cientifica de alto impacto esta em ingles.
3. **Ignorar a data de publicacao.** Evidencias mudam. Priorize estudos dos ultimos 5 anos, a menos que busque artigos seminais.
4. **Confiar em resumos da IA sem ler o artigo original.** Para decisoes clinicas importantes, leia pelo menos o abstract e os metodos dos estudos-chave.
5. **Nao considerar o nivel de evidencia.** Uma meta-analise de RCTs tem mais peso que um relato de caso, independentemente do que a IA destaque.

---

## Modelo de Registro de Pesquisa

Use este modelo para documentar suas pesquisas rapidas:

```
Data: ___/___/______
Pergunta clinica: _________________________________
Formato PICO: P:___ I:___ C:___ O:___
Ferramentas usadas: ______________________________
Artigos-chave encontrados (3-5):
1. _______________________________________________
2. _______________________________________________
3. _______________________________________________
Sintese: _________________________________________
Implicacao para conduta: __________________________
Limitacoes: ______________________________________
```

---

*Material educacional do curso IAMed - Nivel 1: Fundacao.*
