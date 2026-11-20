# Template: Resumo de Artigo Científico em Formato PICO

## Quando usar

Use este template quando precisar extrair rapidamente as informações essenciais de um artigo científico e organizá-las no formato PICO (Paciente/População, Intervenção, Comparação, Outcome/Desfecho). Ideal para journal clubs, atualização rápida, preparação de aulas ou para decidir se vale a pena ler o artigo completo.

---

## Template (copie e cole)

```
Você é um epidemiologista clínico experiente em leitura crítica de evidências.

Analise o artigo abaixo e forneça um resumo estruturado.

ARTIGO:
[COLE AQUI O ABSTRACT COMPLETO OU O TEXTO DO ARTIGO]

Referência completa: [AUTORES, TÍTULO, REVISTA, ANO, DOI]

FORMATO DO RESUMO:

1. PICO DO ESTUDO
   - P (População): Quem foi estudado? Critérios de inclusão/exclusão principais.
   - I (Intervenção): Qual a intervenção ou exposição avaliada?
   - C (Comparação): Qual o grupo controle ou comparador?
   - O (Outcome/Desfecho): Qual o desfecho primário? E os secundários?

2. DESENHO DO ESTUDO
   - Tipo de estudo (ECR, coorte, caso-controle, transversal, revisão sistemática, etc.)
   - Nível de evidência (Oxford/GRADE)
   - Tempo de seguimento
   - Tamanho da amostra e poder estatístico (se informado)

3. RESULTADOS PRINCIPAIS
   - Desfecho primário: resultado com IC 95% e valor de p
   - NNT ou NNH (calcule se não estiver explícito e os dados permitirem)
   - Desfechos secundários relevantes
   - Análises de subgrupo importantes

4. PONTOS FORTES E LIMITAÇÕES
   - Liste 3 pontos fortes do estudo
   - Liste 3 limitações
   - Avalie risco de viés (seleção, aferição, confusão, atrito)

5. APLICABILIDADE NO BRASIL
   - Esta evidência se aplica à população brasileira? Por quê?
   - Considere acesso pelo SUS e pela rede privada
   - Há alguma diretriz brasileira (SBC, SBD, SBMT, etc.) que já incorporou esta evidência?

6. CONCLUSÃO EM 1 PARÁGRAFO
   - Resumo objetivo do que o estudo muda (ou não) na prática clínica

7. PÉROLA CLÍNICA
   - Uma frase que resuma o achado principal de forma memorável
```

---

## Exemplo preenchido

```
Você é um epidemiologista clínico experiente em leitura crítica de evidências.

Analise o artigo abaixo e forneça um resumo estruturado.

ARTIGO:
Background: Sodium-glucose cotransporter 2 (SGLT2) inhibitors reduce the risk of hospitalization for heart failure in patients with heart failure and a reduced ejection fraction, but their effects in patients with heart failure and a mildly reduced or preserved ejection fraction are less certain.
Methods: In this double-blind trial, we randomly assigned 5988 patients with heart failure and a left ventricular ejection fraction of more than 40% to receive empagliflozin (10 mg once daily) or placebo, in addition to usual therapy. The primary outcome was a composite of cardiovascular death or hospitalization for heart failure.
Results: Over a median of 26.2 months, a primary outcome event occurred in 415 of 2997 patients (13.8%) in the empagliflozin group and in 511 of 2991 patients (17.1%) in the placebo group (hazard ratio, 0.79; 95% CI, 0.69 to 0.90; P<0.001). This result was mainly driven by a reduction in hospitalization for heart failure. The effect was consistent regardless of the presence or absence of diabetes. Adverse events related to the trial regimen did not differ meaningfully between the two groups.
Conclusions: Empagliflozin reduced the combined risk of cardiovascular death or hospitalization for heart failure in patients with heart failure and a mildly reduced or preserved ejection fraction, regardless of the presence or absence of diabetes.

Referência completa: Anker SD, Butler J, Filippatos G, et al. Empagliflozin in Heart Failure with a Preserved Ejection Fraction. N Engl J Med. 2021;385(16):1451-1461. doi:10.1056/NEJMoa2107038 (EMPEROR-Preserved)

FORMATO DO RESUMO:

1. PICO DO ESTUDO
   - P (População): Quem foi estudado? Critérios de inclusão/exclusão principais.
   - I (Intervenção): Qual a intervenção ou exposição avaliada?
   - C (Comparação): Qual o grupo controle ou comparador?
   - O (Outcome/Desfecho): Qual o desfecho primário? E os secundários?

2. DESENHO DO ESTUDO
   - Tipo de estudo (ECR, coorte, caso-controle, transversal, revisão sistemática, etc.)
   - Nível de evidência (Oxford/GRADE)
   - Tempo de seguimento
   - Tamanho da amostra e poder estatístico (se informado)

3. RESULTADOS PRINCIPAIS
   - Desfecho primário: resultado com IC 95% e valor de p
   - NNT ou NNH (calcule se não estiver explícito e os dados permitirem)
   - Desfechos secundários relevantes
   - Análises de subgrupo importantes

4. PONTOS FORTES E LIMITAÇÕES
   - Liste 3 pontos fortes do estudo
   - Liste 3 limitações
   - Avalie risco de viés (seleção, aferição, confusão, atrito)

5. APLICABILIDADE NO BRASIL
   - Esta evidência se aplica à população brasileira? Por quê?
   - Considere acesso pelo SUS e pela rede privada
   - Há alguma diretriz brasileira (SBC, SBD, SBMT, etc.) que já incorporou esta evidência?

6. CONCLUSÃO EM 1 PARÁGRAFO
   - Resumo objetivo do que o estudo muda (ou não) na prática clínica

7. PÉROLA CLÍNICA
   - Uma frase que resuma o achado principal de forma memorável
```

---

## Dicas de uso

- **Cole o abstract completo**, não apenas o título. Se possível, cole também a seção de métodos e resultados do artigo inteiro para uma análise mais profunda.
- **Peça para a IA calcular o NNT**: se o artigo não traz o NNT explícito, os dados de redução absoluta de risco geralmente permitem o cálculo. No exemplo acima: RAR = 17,1% - 13,8% = 3,3%, logo NNT = 1/0,033 = ~30.
- **Use para preparar journal club**: após obter o resumo, peça à IA para gerar 5 perguntas de discussão sobre o artigo.
- **Compare com diretrizes brasileiras**: a seção de aplicabilidade é essencial. A IA pode não ter informações atualizadas sobre incorporação no SUS via CONITEC, então valide esse ponto.
- **Artigos em português também funcionam**: se o artigo for de um periódico brasileiro (como Arquivos Brasileiros de Cardiologia), cole o texto em português mesmo.

---

## Variações possíveis

| Variação | O que mudar no template |
|---|---|
| **Revisão sistemática/meta-análise** | Adicione ao formato: "Avalie heterogeneidade (I2), risco de viés de publicação e qualidade metodológica via AMSTAR-2" |
| **Artigo de diagnóstico** | Substitua PICO por: "População testada, Teste índice, Padrão-ouro, Sensibilidade/Especificidade/LR+/LR-" |
| **Comparação de dois artigos** | Cole os dois abstracts e adicione: "Compare os dois estudos lado a lado em uma tabela, destacando diferenças de população, intervenção, resultados e limitações" |
| **Resumo para pacientes** | Adicione ao final: "Agora reescreva a conclusão em linguagem acessível para um paciente leigo com ensino fundamental" |
| **Foco em custo-efetividade** | Adicione: "Analise se o artigo traz dados de custo-efetividade. Se não trouxer, estime o impacto econômico considerando o preço do medicamento no Brasil (Tabela CMED)" |
