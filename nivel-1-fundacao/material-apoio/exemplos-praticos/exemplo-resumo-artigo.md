# Exemplo Pratico 2: Resumo de Artigo Cientifico com Template Estruturado

## Contexto Clinico

**Cenario:** Dr. Rafael, nefrologista em Curitiba, precisa apresentar um journal club na proxima semana sobre o estudo DAPA-CKD. Ele tem pouco tempo e decide usar a IA para gerar um resumo estruturado do artigo como ponto de partida.

**Artigo:** Heerspink HJL, et al. "Dapagliflozin in Patients with Chronic Kidney Disease." N Engl J Med. 2020;383(15):1436-1446.

**Objetivo do medico:** Obter um resumo estruturado que cubra metodologia, resultados principais e limitacoes, para depois revisar e complementar com leitura propria.

---

## O Prompt Usado

```
Voce e um nefrologista pesquisador. Resuma o artigo abaixo seguindo 
exatamente este template:

ARTIGO: "Dapagliflozin in Patients with Chronic Kidney Disease" — 
Heerspink et al., NEJM 2020.

TEMPLATE DE RESUMO:

1. PERGUNTA DO ESTUDO (PICO)
   - Populacao:
   - Intervencao:
   - Comparador:
   - Desfecho primario:

2. DESENHO DO ESTUDO
   - Tipo:
   - Multicêntrico? Quantos centros/paises:
   - Duracao do seguimento:
   - Tamanho da amostra (n):

3. RESULTADOS PRINCIPAIS
   - Desfecho primario: resultado com HR/OR e IC 95%
   - NNT (se aplicavel):
   - Desfechos secundarios relevantes:

4. LIMITACOES
   - Listadas pelos autores:
   - Identificadas por voce:

5. RELEVANCIA CLINICA PARA O BRASIL
   - Implicacao pratica:
   - Disponibilidade do medicamento no SUS:

RESTRICAO: Use apenas dados do artigo original. Se nao lembrar um valor 
exato, diga "valor exato a confirmar no texto original".
```

---

## Resposta da IA

> **Resumo Estruturado — DAPA-CKD (Heerspink et al., NEJM 2020)**
>
> ### 1. PERGUNTA DO ESTUDO (PICO)
> - **Populacao:** Pacientes com doenca renal cronica (TFGe 25-75 mL/min/1.73m2 e razao albumina/creatinina urinaria 200-5000 mg/g), com e sem diabetes tipo 2
> - **Intervencao:** Dapagliflozina 10 mg/dia via oral
> - **Comparador:** Placebo
> - **Desfecho primario:** Composto de declinio sustentado >= 50% na TFGe, doenca renal terminal (dialise, transplante ou TFGe <15) ou morte por causa renal ou cardiovascular
>
> ### 2. DESENHO DO ESTUDO
> - **Tipo:** Ensaio clinico randomizado, duplo-cego, controlado por placebo, fase 3
> - **Multicentrico:** Sim, 386 centros em 21 paises
> - **Duracao do seguimento:** Mediana de 2.4 anos
> - **Tamanho da amostra:** 4.304 pacientes (2.152 dapagliflozina, 2.152 placebo)
>
> ### 3. RESULTADOS PRINCIPAIS
> - **Desfecho primario:** HR 0.61 (IC 95%: 0.51-0.72; p<0.001) — reducao de 39% no risco relativo do desfecho composto
> - **NNT:** 19 pacientes tratados por 2.4 anos para prevenir um evento do desfecho primario
> - **Desfechos secundarios relevantes:**
>   - Composto renal (declinio TFGe, DRCT ou morte renal): HR 0.56 **(IC 95%: 0.42-0.73)**
>   - Morte cardiovascular ou hospitalizacao por IC: HR 0.71 (IC 95%: 0.55-0.92)
>   - Mortalidade por todas as causas: HR 0.69 (IC 95%: 0.53-0.88)
>   - **Beneficio consistente em pacientes com e sem diabetes tipo 2**
>
> ### 4. LIMITACOES
> - **Listadas pelos autores:**
>   - Estudo interrompido precocemente pelo comite de seguranca por eficacia, o que pode superestimar o efeito
>   - Poucos pacientes com TFGe <30 (limita generalizacao para DRC avancada)
>   - Seguimento relativamente curto
> - **Identificadas por mim:**
>   - Maioria dos pacientes usava iECA/BRA — resultado pode nao se aplicar a pacientes sem bloqueio do SRAA
>   - Populacao predominantemente com DRC de etiologia diabetica e hipertensiva — menor representatividade de glomerulopatias primarias
>   - Baixa representacao de pacientes da America Latina (menos de 10% da amostra)
>
> ### 5. RELEVANCIA CLINICA PARA O BRASIL
> - **Implicacao pratica:** A dapagliflozina demonstrou nefroproteçêo robusta independente da presenca de diabetes, ampliando significativamente sua indicacao na DRC. Isso muda o paradigma de tratamento — SGLT2i deixa de ser apenas "antidiabetico" e passa a ser "nefroprotetor".
> - **Disponibilidade no SUS:** A dapagliflozina 10 mg foi incorporada ao SUS pela CONITEC em 2022 para pacientes com DRC (TFGe 25-75) com ou sem diabetes, alinhada aos resultados deste estudo. Disponivel nas UBS via componente especializado da assistencia farmaceutica.

---

## Avaliacao Critica do Medico

### O que a IA ACERTOU

1. **Estrutura PICO precisa.** A populacao, intervencao e comparador estao corretos. Os criterios de inclusao (TFGe 25-75, RAC 200-5000) estao certos.

2. **Desfecho primario e HR principal.** O HR 0.61 (IC 95%: 0.51-0.72) para o desfecho composto primario esta correto conforme o artigo original.

3. **Interrupcao precoce.** Correto — o estudo foi interrompido pelo DSMB por eficacia, e isso e uma limitacao real que muitos resumos omitem.

4. **Beneficio independente de diabetes.** Corretamente destacado — este foi o achado mais impactante do DAPA-CKD.

5. **Incorporacao ao SUS.** A informacao sobre a CONITEC esta essencialmente correta — a dapagliflozina de fato foi incorporada para DRC.

### O que a IA ERROU

1. **IC 95% do desfecho composto renal INVENTADO.** A IA reportou o composto renal com HR 0.56 (IC 95%: 0.42-0.73). Verificando o artigo original, o HR para o composto renal especifico (sem morte CV) e **0.56 (IC 95%: 0.45-0.68)**. A IA errou os limites do intervalo de confianca. Os valores 0.42 e 0.73 nao aparecem no artigo. **Este e um caso classico de alucinacao numerica** — a IA "inventou" um IC plausivel mas incorreto.

2. **NNT impreciso.** A IA informou NNT de 19. O NNT calculado a partir dos dados do artigo (diferenca absoluta de risco de 5.3% no desfecho primario em 2.4 anos) resulta em NNT aproximado de **19**, entao o valor esta proximo, mas a IA nao mostrou o calculo nem indicou que e uma estimativa. O valor exato depende do metodo de calculo (Kaplan-Meier vs. incidencia cumulativa).

3. **Numero de centros.** A IA citou 386 centros em 21 paises. O artigo original reporta **386 centros em 21 paises** — neste caso, o dado esta correto. (Nota: incluimos este item na verificacao porque numeros de centros sao frequentemente alucinados pela IA.)

4. **Disponibilidade no SUS — detalhes imprecisos.** A IA disse que esta disponivel "via componente especializado da assistencia farmaceutica". Na pratica, a dispensacao pode variar por estado, e a logistica de acesso nao e tao simples quanto a IA sugere. Alem disso, a incorporacao especifica para DRC sem diabetes foi um processo mais nuancado do que apresentado.

### O que e PERIGOSO

- **Numeros inventados com aparencia de precisao.** O IC 95% fabricado (0.42-0.73 ao inves de 0.45-0.68) e perigoso porque, ao ser incluido numa apresentacao de journal club, seria aceito sem questionamento por colegas que confiam no apresentador. Se alguem citar esse IC em um artigo de revisao, estaria propagando dado falso.
- A diferenca parece pequena (0.42 vs 0.45, 0.73 vs 0.68), mas em medicina baseada em evidencias, intervalos de confianca tem significado estatistico preciso. Limites alterados podem mudar a interpretacao de heterogeneidade em meta-analises.

---

## Licao Aprendida

A IA produziu um resumo de qualidade surpreendentemente boa — a estrutura esta clara, os conceitos principais estao corretos, e seria um excelente ponto de partida para o journal club. No entanto, **os numeros especificos (IC 95%, NNT) precisam ser conferidos um a um contra o artigo original.**

A regra pratica e: **nunca confie em numeros gerados pela IA sem verificacao cruzada com a fonte primaria.** A IA e boa em estrutura e conceitos, mas tende a "preencher lacunas" numericas com valores plausiveis quando nao tem certeza.

Neste caso, o prompt incluia a instrucao "se nao lembrar um valor exato, diga 'valor exato a confirmar'", mas a IA ignorou essa instrucao para o IC do desfecho secundario. Isso demonstra que **restricoes no prompt reduzem, mas nao eliminam, alucinacoes.**

---

## Como Melhorar o Prompt

1. **Fornecer o abstract junto com o prompt:**
   ```
   Cole o abstract completo no prompt para que a IA extraia dados 
   diretamente do texto, em vez de depender da memoria (que e falivel).
   ```

2. **Pedir nivel de confianca para cada numero:**
   ```
   Para cada valor numerico (HR, IC, NNT, n), classifique sua confianca: 
   EXTRAIDO DO TEXTO (certeza) vs. LEMBRADO (verificar) vs. ESTIMADO (calcular).
   ```

3. **Separar fatos do artigo de interpretacoes:**
   ```
   Divida a resposta em duas secoes: DADOS DO ARTIGO (apenas o que esta 
   escrito) e MINHA INTERPRETACAO (analise adicional). Isso facilita a 
   verificacao.
   ```

4. **Usar a IA em duas etapas:**
   - Etapa 1: Colar o abstract e pedir extracao pura de dados
   - Etapa 2: Pedir analise e interpretacao dos dados extraidos

---

**Veredicto final:** Para resumos de artigos, a IA e uma ferramenta de produtividade excelente — economiza tempo na estruturacao. Mas o medico DEVE ler o artigo original e conferir cada numero antes de apresentar ou publicar. A IA nao substitui a leitura critica; ela agiliza o processo.
