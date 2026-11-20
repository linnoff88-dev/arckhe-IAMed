# Glossario de IA para Medicos

**40+ termos de inteligencia artificial traduzidos para a linguagem medica.**
**Formato:** Termo tecnico -- Traducao medica -- Explicacao pratica.

---

## Conceitos Fundamentais

**1. Artificial Intelligence (AI) / Inteligencia Artificial (IA)**
Traducao medica: Sistemas computacionais que simulam raciocinio.
Programas de computador capazes de realizar tarefas que normalmente exigiriam inteligencia humana, como reconhecer padroes, interpretar texto ou tomar decisoes com base em dados.

**2. Machine Learning (ML) / Aprendizado de Maquina**
Traducao medica: Aprendizado por experiencia (como residencia, mas para computadores).
Subcampo da IA em que o sistema aprende padroes a partir de dados, sem ser explicitamente programado para cada situacao. Quanto mais dados ve, melhor fica — similar a um residente ganhando experiencia.

**3. Deep Learning / Aprendizado Profundo**
Traducao medica: Reconhecimento avancado de padroes.
Tipo de aprendizado de maquina que usa "redes neurais" com muitas camadas para identificar padroes complexos. E a tecnologia por tras do reconhecimento de imagens em radiologia e dermatologia.

**4. Neural Network / Rede Neural**
Traducao medica: Circuito de processamento inspirado no cerebro.
Estrutura computacional vagamente inspirada em neuronios biologicos. Recebe informacoes, processa em camadas e gera uma saida. Nao pensa como um cerebro — apenas usa uma arquitetura matematica similar.

**5. Large Language Model (LLM) / Modelo de Linguagem de Grande Porte**
Traducao medica: O "cerebro" por tras do ChatGPT, Claude e similares.
Modelo de IA treinado em enormes volumes de texto para entender e gerar linguagem humana. E o motor que faz assistentes de IA conversarem de forma coerente.

**6. Algorithm / Algoritmo**
Traducao medica: Protocolo clinico, mas para computadores.
Conjunto de instrucoes passo a passo que o computador segue para resolver um problema. Assim como um protocolo de sepse guia a conduta, um algoritmo guia o processamento de dados.

---

## Geracao de Texto e Respostas

**7. Hallucination / Alucinacao**
Traducao medica: Invencao de informacao com confianca.
Quando a IA gera informacoes falsas, mas apresenta com tom confiante e convincente. Analogo a um residente que afirma algo que nao esta na literatura, mas fala com tanta seguranca que parece verdade.

**8. Prompt / Prompt (Comando)**
Traducao medica: A "anamnese" que voce faz a IA.
O texto que voce escreve para pedir algo a IA. Assim como uma boa anamnese leva a um bom diagnostico, um bom prompt leva a uma boa resposta.

**9. Prompt Engineering / Engenharia de Prompt**
Traducao medica: A arte de fazer as perguntas certas a IA.
Tecnica de estruturar perguntas e instrucoes para obter as melhores respostas possiveis da IA. E aprender a "fazer anamnese" de forma eficiente com a maquina.

**10. Context Window / Janela de Contexto**
Traducao medica: "Memoria de trabalho" da IA.
Quantidade de texto que a IA consegue considerar de uma so vez. Como a memoria de trabalho humana e limitada, a da IA tambem tem um teto. Modelos mais avancados tem janelas maiores.

**11. Token / Token**
Traducao medica: "Silaba" computacional.
Unidade basica de texto que a IA processa. Uma palavra pode ter 1 a 4 tokens. Importante porque a janela de contexto e medida em tokens, e muitas vezes o custo tambem.

**12. Temperature / Temperatura**
Traducao medica: "Nivel de criatividade" da resposta.
Parametro que controla o grau de aleatoriedade na resposta da IA. Temperatura baixa = respostas mais previsiveis e conservadoras. Temperatura alta = respostas mais criativas e variadas.

**13. Fine-tuning / Ajuste Fino**
Traducao medica: "Especializacao" do modelo (como uma residencia medica).
Processo de treinar um modelo de IA geral com dados especificos de um dominio para que ele se torne especialista. Um LLM generico fine-tuned com literatura medica responde melhor a perguntas clinicas.

**14. RAG (Retrieval-Augmented Generation) / Geracao Aumentada por Recuperacao**
Traducao medica: IA que "consulta o livro" antes de responder.
Tecnica em que a IA busca informacoes em uma base de dados especifica antes de gerar a resposta, em vez de confiar apenas no que "memorizou" durante o treinamento. Reduz alucinacoes.

---

## Dados e Treinamento

**15. Training Data / Dados de Treinamento**
Traducao medica: Os "livros-texto" da IA.
Conjunto de dados usado para ensinar o modelo. A qualidade e diversidade desses dados determinam o conhecimento e os vieses da IA — assim como a formacao de um medico depende da qualidade dos seus livros e preceptores.

**16. Bias / Vies**
Traducao medica: Vies diagnostico, mas do algoritmo.
Tendencias sistematicas nas respostas da IA causadas por desequilibrios nos dados de treinamento. Se a IA foi treinada com mais dados de pacientes brancos, pode ter desempenho inferior em outras populacoes.

**17. Overfitting / Sobreajuste**
Traducao medica: "Decorar a prova em vez de aprender a materia."
Quando o modelo aprende tao bem os dados de treinamento que perde a capacidade de generalizar para casos novos. Como um residente que decora casos especificos mas nao entende o raciocinio por tras.

**18. Ground Truth / Verdade de Referencia**
Traducao medica: Padrao-ouro.
A resposta correta contra a qual o modelo e avaliado. Em medicina, e o diagnostico confirmado (biopsia, cultura, etc.) usado para medir a acuracia do modelo.

**19. Annotation / Anotacao**
Traducao medica: Laudo feito por especialista para ensinar a IA.
Processo de rotular dados manualmente (ex: marcar tumores em imagens) para que a IA aprenda o que e correto. A qualidade da IA depende da qualidade dessas anotacoes.

**20. Synthetic Data / Dados Sinteticos**
Traducao medica: Casos clinicos fictícios, mas realistas.
Dados gerados artificialmente que imitam dados reais, usados quando dados reais sao escassos ou sensiveis. Util para treinar modelos sem expor dados de pacientes.

---

## Avaliacao de Desempenho

**21. Accuracy / Acuracia**
Traducao medica: Taxa de acerto geral.
Proporcao de respostas corretas entre todas as respostas. Cuidado: em condicoes raras, alta acuracia pode ser enganosa (como um teste que diz "nao tem cancer" para todos e acerta 99% das vezes).

**22. Sensitivity / Sensibilidade**
Traducao medica: Igual em medicina — taxa de verdadeiros positivos.
Capacidade do modelo de identificar corretamente os casos positivos. Alta sensibilidade = poucos falsos negativos.

**23. Specificity / Especificidade**
Traducao medica: Igual em medicina — taxa de verdadeiros negativos.
Capacidade do modelo de identificar corretamente os casos negativos. Alta especificidade = poucos falsos positivos.

**24. AUC-ROC / Area Sob a Curva ROC**
Traducao medica: Medida global de desempenho diagnostico.
Metrica que resume a capacidade discriminativa do modelo. Varia de 0,5 (aleatorio) a 1,0 (perfeito). Interpretacao similar a usada em estudos diagnosticos na medicina.

**25. Benchmark / Benchmark (Referencia)**
Traducao medica: "Prova de residencia" para modelos de IA.
Conjunto padronizado de testes usado para comparar o desempenho de diferentes modelos. O USMLE, por exemplo, e usado como benchmark medico para LLMs.

---

## Tipos de IA em Saude

**26. NLP (Natural Language Processing) / Processamento de Linguagem Natural**
Traducao medica: IA que le e entende texto.
Ramo da IA dedicado a interpretar linguagem humana. E o que permite que a IA leia um artigo, resuma um prontuario ou entenda sua pergunta.

**27. Computer Vision / Visao Computacional**
Traducao medica: IA que interpreta imagens.
Capacidade da IA de analisar imagens — radiografias, lâminas de patologia, lesoes de pele. Base da IA em radiologia e dermatologia.

**28. Clinical Decision Support System (CDSS) / Sistema de Apoio a Decisao Clinica**
Traducao medica: Consultor digital integrado ao prontuario.
Software que analisa dados do paciente e sugere alertas, diagnosticos ou condutas ao medico. Exemplo: alerta de interacao medicamentosa no sistema de prescricao.

**29. SaMD (Software as a Medical Device) / Software como Dispositivo Medico**
Traducao medica: Software que funciona como equipamento medico.
Software que tem funcao medica propria (diagnostico, monitoramento) e precisa de aprovacao regulatoria (ANVISA, FDA). Diferente de um app de agenda, um SaMD pode interpretar um ECG.

**30. Digital Twin / Gemeo Digital**
Traducao medica: Modelo virtual do paciente.
Representacao computacional de um paciente ou orgao que permite simular tratamentos e prever respostas antes de aplica-los no mundo real.

---

## Seguranca e Etica

**31. Explainability / Explicabilidade**
Traducao medica: "Me explique o raciocinio" — o modelo mostra como chegou aquela resposta.
Capacidade de um modelo de IA mostrar por que tomou determinada decisao. Essencial em medicina, onde "confie em mim" nao e aceitavel.

**32. Black Box / Caixa-Preta**
Traducao medica: Modelo que da o resultado mas nao explica como.
IA cujo processo decisorio nao e acessivel ou compreensivel. Problema serio em saude, pois o medico precisa entender o raciocinio para avaliar a sugestao.

**33. Adversarial Attack / Ataque Adversarial**
Traducao medica: "Enganar" a IA com dados manipulados.
Manipulacao sutil dos dados de entrada para fazer a IA errar. Exemplo: alterar minimamente uma imagem radiologica para que a IA mude o diagnostico.

**34. Data Drift / Deriva de Dados**
Traducao medica: Quando o perfil dos pacientes muda e o modelo nao acompanha.
Fenomeno em que os dados do mundo real se tornam diferentes dos dados de treinamento ao longo do tempo, degradando o desempenho do modelo. Como um protocolo que fica desatualizado.

**35. Federated Learning / Aprendizado Federado**
Traducao medica: Treinamento colaborativo sem compartilhar dados.
Tecnica em que varios hospitais treinam um modelo juntos sem que os dados de pacientes saiam de cada instituicao. Os dados ficam locais; apenas o aprendizado e compartilhado.

---

## Termos do Dia a Dia com IA

**36. API (Application Programming Interface)**
Traducao medica: "Tomada" para conectar sistemas.
Interface que permite que diferentes softwares se comuniquem. E o que permite, por exemplo, integrar uma IA ao prontuario eletronico.

**37. Cloud / Nuvem**
Traducao medica: Computador remoto.
Servidores externos onde dados sao armazenados e processados. Quando voce usa ChatGPT, a conversa e processada em servidores na nuvem, nao no seu computador.

**38. On-premise / Local**
Traducao medica: No seu proprio servidor/hospital.
Quando o software roda nos servidores da propria instituicao, sem enviar dados para fora. Maior controle, mas maior custo e complexidade.

**39. Open Source / Codigo Aberto**
Traducao medica: "Receita aberta" — qualquer um pode ver, usar e modificar.
Software cujo codigo e publico e pode ser modificado por qualquer pessoa. Modelos de IA open source (como LLaMA) podem ser rodados localmente para maior privacidade.

**40. Chatbot**
Traducao medica: Assistente virtual de conversa.
Interface de conversa com IA. ChatGPT e Claude sao chatbots. O termo nao define a inteligencia do sistema — ha chatbots simples (baseados em regras) e avancados (baseados em LLMs).

**41. Multimodal**
Traducao medica: IA que "ve, le e ouve" ao mesmo tempo.
Modelo capaz de processar diferentes tipos de dados (texto, imagem, audio) simultaneamente. Relevante em medicina porque o diagnostico muitas vezes combina historia, exames de imagem e laboratorio.

**42. Zero-shot / Few-shot**
Traducao medica: Responder sem ver exemplos / com poucos exemplos.
Capacidade da IA de realizar uma tarefa sem exemplos previos (zero-shot) ou com apenas alguns exemplos (few-shot). Como pedir a um especialista para opinar sobre um tema que ele nunca viu versus dar-lhe 2-3 casos de referencia.

**43. Inference / Inferencia**
Traducao medica: O momento em que a IA "da o resultado."
Processo de usar um modelo ja treinado para gerar respostas ou predicoes a partir de novos dados. O treinamento e a formacao; a inferencia e o atendimento.

**44. Embedding / Embedding (Representacao Vetorial)**
Traducao medica: Como a IA "entende" o significado das palavras.
Representacao numerica de texto que captura seu significado. Permite que a IA entenda que "infarto" e "IAM" sao conceitos proximos, mesmo sendo palavras diferentes.

---

## Referencia Rapida

| Se voce ouvir... | Pense em... |
|---|---|
| "O modelo alucinou" | A IA inventou informacao |
| "Janela de contexto grande" | A IA consegue ler textos longos |
| "Modelo fine-tuned para medicina" | IA especializada em saude |
| "RAG" | IA que consulta fontes antes de responder |
| "Vies do modelo" | Tendencia sistematica que pode prejudicar grupos |
| "Caixa-preta" | Nao da para saber como a IA decidiu |
| "On-premise" | Roda no servidor do hospital, dados nao saem |
| "SaMD" | Software que precisa de aprovacao regulatoria |

---

*Material educacional do curso IAMed - Nivel 1: Fundacao.*
