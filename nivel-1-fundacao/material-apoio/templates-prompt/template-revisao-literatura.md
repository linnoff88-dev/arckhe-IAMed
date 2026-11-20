# Template: Revisao Rapida de Literatura (Pergunta Clinica PICO)

## Quando usar

Use este template quando tiver uma duvida clinica e precisar de orientacao para buscar evidencias de forma estruturada. A IA ajuda a formular a pergunta PICO, montar a estrategia de busca e interpretar o que a literatura diz. Ideal para duvidas que surgem no consultorio, preparacao de protocolos ou atualizacao rapida.

**Importante**: a IA nao substitui a busca real no PubMed/MEDLINE. Ela ajuda a estruturar sua pergunta e pode resumir o que sabe ate sua data de corte, mas voce deve validar as informacoes nas fontes primarias.

---

## Template (copie e cole)

```
Voce e um medico pesquisador com experiencia em medicina baseada em evidencias e revisao sistematica.

Ajude-me a estruturar uma revisao rapida de literatura sobre a pergunta clinica abaixo.

PERGUNTA CLINICA (como surgiu na pratica):
[DESCREVA A SITUACAO CLINICA QUE GEROU A DUVIDA — EX.: "TENHO UM PACIENTE COM IC E FEVE PRESERVADA, OUVI FALAR QUE SGLT2I PODE AJUDAR, MAS NAO SEI SE A EVIDENCIA E FORTE"]

ETAPA 1 — FORMULE A PERGUNTA PICO:
A partir da minha pergunta, estruture:
- P (Populacao): Quem sao os pacientes?
- I (Intervencao): Qual a intervencao ou exposicao em questao?
- C (Comparacao): Qual o comparador?
- O (Outcome/Desfecho): Qual o desfecho mais relevante?

ETAPA 2 — ESTRATEGIA DE BUSCA:
Monte uma estrategia de busca para PubMed/MEDLINE usando:
- Termos MeSH e palavras-chave em ingles
- Operadores booleanos (AND, OR)
- Filtros recomendados (tipo de estudo, data, idioma)
- Formate como uma string pronta para colar no PubMed

ETAPA 3 — PANORAMA DA EVIDENCIA:
Com base no seu conhecimento, apresente:
- Os 3-5 estudos mais importantes sobre esta pergunta (nome do estudo, revista, ano, achado principal)
- A revisao sistematica ou meta-analise mais recente, se existir
- O que dizem as principais diretrizes (brasileiras e internacionais)
- Nivel de evidencia geral (forte/moderada/fraca/insuficiente)
- Lacunas na evidencia (o que ainda nao sabemos)

ETAPA 4 — SINTESE PARA A PRATICA:
- Responda a pergunta clinica em 1 paragrafo objetivo
- Indique o grau de confianca na resposta
- Sugira se vale a pena aprofundar a busca ou se a evidencia ja e suficiente para tomar decisao

RESTRICOES:
- Distinga claramente entre o que e evidencia robusta e o que e opiniao de especialista
- Se nao tiver certeza sobre um estudo especifico, diga "verifique no PubMed" em vez de inventar detalhes
- Considere a realidade brasileira (disponibilidade no SUS, custo, diretrizes da SBC/SBD/etc.)
- Cite se ha estudos brasileiros relevantes sobre o tema
```

---

## Exemplo preenchido

```
Voce e um medico pesquisador com experiencia em medicina baseada em evidencias e revisao sistematica.

Ajude-me a estruturar uma revisao rapida de literatura sobre a pergunta clinica abaixo.

PERGUNTA CLINICA (como surgiu na pratica):
Tenho acompanhado pacientes com insuficiencia cardiaca com fracao de ejecao preservada (ICFEp) e li que os inibidores de SGLT2 podem ter beneficio nesse grupo. Quero saber se a evidencia ja e forte o suficiente para eu prescrever empagliflozina ou dapagliflozina para esses pacientes, ou se ainda e considerado off-label/experimental.

ETAPA 1 — FORMULE A PERGUNTA PICO:
A partir da minha pergunta, estruture:
- P (Populacao): Quem sao os pacientes?
- I (Intervencao): Qual a intervencao ou exposicao em questao?
- C (Comparacao): Qual o comparador?
- O (Outcome/Desfecho): Qual o desfecho mais relevante?

ETAPA 2 — ESTRATEGIA DE BUSCA:
Monte uma estrategia de busca para PubMed/MEDLINE usando:
- Termos MeSH e palavras-chave em ingles
- Operadores booleanos (AND, OR)
- Filtros recomendados (tipo de estudo, data, idioma)
- Formate como uma string pronta para colar no PubMed

ETAPA 3 — PANORAMA DA EVIDENCIA:
Com base no seu conhecimento, apresente:
- Os 3-5 estudos mais importantes sobre esta pergunta
- A revisao sistematica ou meta-analise mais recente, se existir
- O que dizem as principais diretrizes
- Nivel de evidencia geral
- Lacunas na evidencia

ETAPA 4 — SINTESE PARA A PRATICA:
- Responda a pergunta clinica em 1 paragrafo objetivo
- Indique o grau de confianca na resposta
- Sugira se vale a pena aprofundar a busca ou se a evidencia ja e suficiente para tomar decisao

RESTRICOES:
- Distinga claramente entre o que e evidencia robusta e o que e opiniao de especialista
- Se nao tiver certeza sobre um estudo especifico, diga "verifique no PubMed" em vez de inventar detalhes
- Considere a realidade brasileira (disponibilidade no SUS, custo, diretrizes da SBC/SBD/etc.)
- Cite se ha estudos brasileiros relevantes sobre o tema
```

---

## Dicas de uso

- **Comece pela pergunta bruta**: nao se preocupe em formular o PICO perfeitamente. Descreva a duvida como ela surgiu na pratica e deixe a IA estruturar. Depois voce refina.
- **Copie a estrategia de busca no PubMed de verdade**: a IA monta a string de busca, mas voce deve executar no PubMed (pubmed.ncbi.nlm.nih.gov) para obter os artigos reais e atualizados.
- **Verifique os estudos citados**: a IA pode "confundir" detalhes de estudos ou citar artigos que nao existem. Sempre confirme titulo, autores e ano no PubMed ou Google Scholar.
- **Use para protocolos institucionais**: quando estiver montando um protocolo clinico para seu servico, rode o template para cada pergunta-chave do protocolo.
- **Atualize periodicamente**: a evidencia muda. Um tema que voce revisou ha 1 ano pode ter novos ECRs publicados. Rode o template novamente com a restricao "considere apenas estudos publicados apos [DATA]".

---

## Variacoes possiveis

| Variacao | O que mudar no template |
|---|---|
| **Pergunta de diagnostico** | Altere o PICO para: P = populacao com suspeita de X, I = teste diagnostico, C = padrao-ouro, O = sensibilidade/especificidade/LR. Adicione pedido de calculo de probabilidade pos-teste |
| **Pergunta de prognostico** | Altere: I = fator prognostico, C = ausencia do fator, O = desfecho a longo prazo. Peca estudos de coorte em vez de ECRs |
| **Pergunta de etiologia/dano** | Altere: I = exposicao, C = nao-exposicao, O = desfecho adverso. Peca estudos de coorte e caso-controle |
| **Busca para guideline/protocolo** | Adicione: "Alem do PubMed, sugira busca em: Cochrane Library, NICE, UpToDate, Dynamed, diretrizes brasileiras (PCDT, SBC, SBD)" |
| **Comparacao entre dois tratamentos** | Altere a pergunta para comparar duas intervencoes e peca: "Existe estudo head-to-head? Se nao, ha meta-analise em rede (network meta-analysis)?" |
