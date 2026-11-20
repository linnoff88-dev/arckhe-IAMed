# Exemplo Pratico 5: Deteccao de Alucinacao em Referencias Bibliograficas

## Contexto Clinico

**Cenario:** Dra. Fernanda, dermatologista em Recife, esta escrevendo um artigo de revisao sobre inteligencia artificial aplicada a dermatoscopia. Ela precisa de referencias recentes para fundamentar a introducao e decide pedir sugestoes a IA como ponto de partida para a busca bibliografica.

**Objetivo:** Obter 5 referencias relevantes sobre IA em dermatoscopia para depois verificar e incluir no artigo.

---

## O Prompt Usado

```
Voce e um pesquisador em dermatologia digital. Liste 5 artigos 
cientificos publicados entre 2019 e 2024 sobre o uso de inteligencia 
artificial (deep learning) em dermatoscopia para diagnostico de lesoes 
melanociticas. 

Para cada artigo, forneca:
- Autores (primeiro autor et al.)
- Titulo completo
- Journal
- Ano
- DOI (se disponivel)
- Achado principal (1-2 frases)

Priorize artigos de alto impacto (Nature, NEJM, Lancet, JAMA, 
ou journals especializados como JAAD, BJD).
```

---

## Resposta da IA

> **5 Artigos sobre IA em Dermatoscopia (2019-2024)**
>
> ---
>
> **1.** Esteva A, Kuprel B, Novoa RA, et al. "Dermatologist-level classification of skin cancer with deep neural networks." *Nature*. 2017;542(7639):115-118. DOI: 10.1038/nature21056
>
> *Achado principal:* Demonstrou que uma rede neural convolucional (CNN) treinada com 129.450 imagens clinicas alcancou desempenho comparavel ao de 21 dermatologistas na classificacao de lesoes cutaneas, incluindo carcinomas e melanomas.
>
> **Nota:** Este artigo e de 2017, fora do periodo solicitado, mas e considerado o estudo seminal da area e referencia obrigatoria.
>
> ---
>
> **2.** Haenssle HA, Fink C, Schneiderbauer R, et al. "Man against machine: diagnostic performance of a deep learning convolutional neural network for dermoscopic melanoma recognition in comparison to 58 dermatologists." *Annals of Oncology*. 2018;29(8):1836-1842. DOI: 10.1093/annonc/mdy166
>
> *Achado principal:* CNN superou a maioria dos 58 dermatologistas na classificacao dermatoscopica de melanoma vs. nevo, com sensibilidade de 95% vs. 86.6% e especificidade de 82.5% vs. 71.3%.
>
> **Nota:** Tambem ligeiramente fora do periodo (2018), mas altamente relevante.
>
> ---
>
> **3.** Tschandl P, Rosendahl C, Kittler H. "The HAM10000 dataset, a large collection of multi-source dermatoscopic images of common pigmented skin lesions." *Scientific Data*. 2018;5:180161. DOI: 10.1038/sdata.2018.161
>
> *Achado principal:* Apresentou o dataset HAM10000 com 10.015 imagens dermatoscopicas de 7 categorias diagnosticas, tornando-se um dos benchmarks mais utilizados para treinamento e avaliacao de modelos de IA em dermatologia.
>
> ---
>
> **4.** Silva RMV, Nascimento TL, Costa FBR, et al. "Deep learning-based dermoscopic analysis outperforms Brazilian dermatologists in melanoma detection: a multicenter prospective study." *Journal of the American Academy of Dermatology*. 2023;88(4):892-899. DOI: 10.1016/j.jaad.2022.11.034
>
> *Achado principal:* Estudo multicentrico brasileiro envolvendo 12 centros e 142 dermatologistas demonstrou que o modelo de deep learning teve acuracia diagnostica 12% superior a media dos dermatologistas na deteccao precoce de melanoma em populacao com fototipos III-V.
>
> ---
>
> **5.** Rotemberg V, Kurtansky N, Bressler-Grinberg S, et al. "A patient-centric dataset of images and metadata for identifying melanomas using clinical context." *Scientific Data*. 2021;8:34. DOI: 10.1038/s41597-021-00815-z
>
> *Achado principal:* Apresentou o dataset SLICE-3D com mais de 33.000 imagens dermatoscopicas contextualizadas com metadados clinicos, avancando a pesquisa em IA ao incorporar informacoes como localizacao da lesao e idade do paciente no modelo diagnostico.
>
> ---

---

## O Processo de Verificacao da Medica (Passo a Passo)

Dra. Fernanda, sabendo que a IA pode alucinar referencias, decidiu verificar **cada artigo** antes de incluir no manuscrito. Aqui esta o processo que ela seguiu:

### Passo 1: Verificacao por DOI

Para cada artigo, ela acessou **doi.org** e inseriu o DOI fornecido.

| # | DOI fornecido | Resultado |
|---|---------------|-----------|
| 1 | 10.1038/nature21056 | ENCONTRADO — artigo real de Esteva et al., Nature 2017. Dados corretos. |
| 2 | 10.1093/annonc/mdy166 | ENCONTRADO — artigo real de Haenssle et al., Annals of Oncology 2018. Dados corretos. |
| 3 | 10.1038/sdata.2018.161 | ENCONTRADO — artigo real de Tschandl et al., Scientific Data 2018. Dados corretos. |
| 4 | 10.1016/j.jaad.2022.11.034 | NAO ENCONTRADO — DOI nao resolve para nenhum artigo. **Alerta vermelho.** |
| 5 | 10.1038/s41597-021-00815-z | ENCONTRADO — artigo real de Rotemberg et al., Scientific Data 2021. Titulo e dados corretos. |

**Resultado parcial:** 1 artigo com DOI invalido (artigo 4). Necessita investigacao adicional.

### Passo 2: Busca no PubMed para o artigo suspeito (4)

Dra. Fernanda buscou no PubMed:
- Busca: `"Silva RMV" AND "dermoscopic" AND JAAD`
- Resultado: **0 artigos encontrados**

Busca alternativa:
- `"deep learning" AND "Brazilian dermatologists" AND "melanoma" AND JAAD`
- Resultado: **0 artigos encontrados**

Busca por titulo exato:
- `"Deep learning-based dermoscopic analysis outperforms Brazilian dermatologists"`
- Resultado: **0 artigos encontrados**

**Conclusao:** O artigo 4 e **completamente fabricado pela IA.** Os autores (Silva RMV, Nascimento TL, Costa FBR) nao possuem essa publicacao. O JAAD volume 88, edicao 4 existe, mas nao contem esse artigo. A IA criou um artigo ficticio com:
- Autores com nomes brasileiros plausiveis
- Journal real e prestigiado (JAAD)
- DOI com formato valido mas inexistente
- Achado principal plausivel e detalhado (12 centros, 142 dermatologistas, fototipos III-V)
- Ate incluiu um resultado especifico ("12% superior") para parecer mais convincente

### Passo 3: Verificacao cruzada dos artigos "reais"

Mesmo para os 4 artigos com DOI valido, Dra. Fernanda verificou os detalhes:

**Artigo 1 (Esteva et al.):**
- Autores: correto
- Titulo: correto
- Journal/ano: correto (Nature 2017)
- Achado: essencialmente correto, mas o numero de imagens no artigo original e **129.450 imagens clinicas** — correto
- Numero de dermatologistas: o artigo menciona **21 dermatologistas** — correto
- **Porem:** a IA incluiu este artigo mesmo sendo de 2017 (fora do periodo 2019-2024 solicitado)

**Artigo 2 (Haenssle et al.):**
- Autores: correto
- Titulo: correto
- Journal/ano: correto (Annals of Oncology 2018)
- Sensibilidade/especificidade reportadas: **a conferir no texto original** — os numeros 95% vs 86.6% sao aproximados mas podem nao ser os valores exatos reportados no abstract. A IA pode ter arredondado ou confundido metricas de diferentes analises do estudo
- **Porem:** tambem fora do periodo solicitado (2018)

**Artigo 3 (Tschandl et al.):**
- Dados corretos
- **Porem:** 2018, fora do periodo

**Artigo 5 (Rotemberg et al.):**
- Autores e titulo: corretos
- O dataset e real (ISIC challenge)
- O numero de 33.000 imagens e o nome SLICE-3D precisam ser confirmados — o artigo real descreve o dataset do ISIC 2020 challenge, mas o nome "SLICE-3D" e os detalhes exatos podem variar

### Passo 4: Tabela resumo final

| # | Artigo | Status | Detalhes corretos? | Periodo correto? |
|---|--------|--------|-------------------|-----------------|
| 1 | Esteva et al., Nature 2017 | REAL | Sim | NAO (2017) |
| 2 | Haenssle et al., Ann Oncol 2018 | REAL | Parcialmente (numeros a conferir) | NAO (2018) |
| 3 | Tschandl et al., Sci Data 2018 | REAL | Sim | NAO (2018) |
| 4 | Silva et al., JAAD 2023 | **FABRICADO** | N/A | N/A |
| 5 | Rotemberg et al., Sci Data 2021 | REAL | Parcialmente (detalhes a conferir) | Sim |

**Resumo:** De 5 artigos, 1 e completamente fabricado (20%), 3 sao reais mas fora do periodo solicitado, e apenas 1 atende aos criterios do pedido.

---

## Avaliacao Critica da Medica

### Padroes observados na alucinacao

1. **A IA fabricou o artigo mais "conveniente".** O artigo inventado (4) era o unico com autores brasileiros, estudo multicentrico brasileiro e publicacao em 2023 — exatamente o tipo de referencia que seria mais util para a Dra. Fernanda. A IA parece ter "preenchido uma lacuna" ao perceber que nao tinha referencias brasileiras recentes.

2. **Nivel de detalhe da fabricacao e assustador.** A IA nao inventou apenas titulo e autores — criou um estudo completo com 12 centros, 142 dermatologistas, resultado especifico (12% superior) e ate mencionou fototipos III-V (relevante para populacao brasileira). Quanto mais detalhado, mais convincente — e mais perigoso.

3. **DOI com formato valido.** O DOI fabricado (10.1016/j.jaad.2022.11.034) segue o formato correto do JAAD (prefixo Elsevier 10.1016, path do JAAD). Isso poderia enganar uma verificacao superficial que olha apenas o formato.

4. **Artigos reais usados como "ancora de credibilidade".** Ao misturar 4 artigos reais com 1 fabricado, a IA criou um cenario onde a maioria das referencias e verificavel, o que pode levar o usuario a assumir que todas sao corretas apos verificar 2-3.

### O que tornaria a alucinacao INDETECTAVEL para um leitor desatento

- O artigo inventado cita um journal real (JAAD) com volume e paginas plausiveis
- Os autores tem nomes brasileiros comuns
- O achado e clinicamente coerente e relevante
- Se alguem nao verificar o DOI ou buscar no PubMed, nao teria como saber que e falso

---

## Licao Aprendida

### Regra de ouro para referencias bibliograficas

**NUNCA cite uma referencia fornecida pela IA sem verificacao independente.** O fluxo correto e:

1. **Verificar o DOI** em doi.org — se nao resolver, o artigo provavelmente nao existe
2. **Buscar no PubMed** pelo titulo exato entre aspas
3. **Conferir autores, journal, volume e paginas** no registro encontrado
4. **Verificar os numeros citados** (resultados, metricas) contra o abstract ou texto original
5. **So entao incluir** no seu manuscrito

### Por que a IA alucina referencias?

A IA nao tem acesso a bases de dados bibliograficos em tempo real. Ela gera referencias com base em padroes estatisticos — sabe que "Esteva" publica sobre IA em dermatologia na Nature, que o JAAD publica estudos de dermatoscopia, e que DOIs da Elsevier tem determinado formato. Quando nao "lembra" de um artigo real que atenda ao pedido, ela **sintetiza um artigo plausivel** combinando esses padroes. Nao e mentira intencional — e o modelo tentando ser util preenchendo lacunas com conteudo estatisticamente provavel.

---

## Como Melhorar o Prompt

1. **Pedir honestidade explicita sobre incerteza:**
   ```
   RESTRICAO: Se voce nao tem certeza ABSOLUTA de que um artigo existe, 
   NAO o inclua. Prefiro receber 2 artigos reais do que 5 com fabricados 
   misturados. Para cada artigo, classifique: CERTEZA ALTA / CERTEZA MEDIA / 
   INCERTO.
   ```

2. **Usar a IA para sugerir TERMOS DE BUSCA, nao artigos:**
   ```
   Em vez de me dar artigos, sugira 5 estrategias de busca para PubMed 
   (combinacoes de MeSH terms e palavras-chave) para eu encontrar artigos 
   sobre IA em dermatoscopia publicados entre 2019-2024.
   ```
   Essa abordagem e muito mais segura — a IA e boa em construir queries de busca.

3. **Pedir apenas artigos "classicos" amplamente conhecidos:**
   ```
   Liste apenas artigos considerados marcos (landmark studies) na area 
   de IA em dermatologia — aqueles com mais de 500 citacoes. Esses tem 
   maior probabilidade de a IA "lembrar" corretamente.
   ```

4. **Usar ferramentas com acesso a bases de dados:**
   Em vez de pedir referencias diretamente a IA generativa, usar ferramentas como:
   - PubMed diretamente (busca manual)
   - Semantic Scholar (busca com IA mas baseada em dados reais)
   - Connected Papers (para encontrar artigos relacionados a um artigo seminal real)
   - Perplexity ou outras IAs com acesso a internet em tempo real

---

## Checklist de Verificacao de Referencias (para imprimir e usar)

```
VERIFICACAO DE REFERENCIA FORNECIDA POR IA

[ ] 1. DOI verificado em doi.org — resolve para o artigo correto?
[ ] 2. Busca no PubMed por titulo exato — artigo encontrado?
[ ] 3. Autores conferem com o registro do PubMed/journal?
[ ] 4. Journal, volume, paginas e ano conferem?
[ ] 5. O achado principal descrito confere com o abstract?
[ ] 6. Numeros especificos (n, HR, IC, p-valor) conferem com o texto?

Se QUALQUER item falhar: DESCARTAR a referencia e buscar manualmente.
```

---

**Veredicto final:** A IA e a PIOR ferramenta possivel para fornecer referencias bibliograficas diretamente. Use-a para construir estrategias de busca, identificar temas e organizar a revisao de literatura — mas NUNCA para gerar a lista de referencias em si. Cada referencia em um artigo cientifico precisa ser rastreavel ate a fonte primaria, e a IA nao oferece essa garantia.
