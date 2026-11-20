# Template: Nota Clínica SOAP

## Quando usar

Use este template para transformar suas anotações livres de consulta em uma nota clínica estruturada no formato SOAP (Subjetivo, Objetivo, Avaliação, Plano). Ideal para otimizar a documentação em prontuário eletrônico, economizando tempo sem perder qualidade.

---

## Template (copie e cole)

```
Você é um médico [ESPECIALIDADE] experiente em documentação clínica no Brasil.

A partir das informações abaixo, gere uma nota clínica completa no formato SOAP para registro em prontuário eletrônico.

INFORMAÇÕES DA CONSULTA (anotações livres):
[COLE AQUI SUAS ANOTAÇÕES, RASCUNHOS, ÁUDIO TRANSCRITO OU INFORMAÇÕES SOLTAS DA CONSULTA — NÃO PRECISA ESTAR ORGANIZADO]

DADOS ADICIONAIS:
- Data da consulta: [DATA]
- Tipo de consulta: [PRIMEIRA VEZ / RETORNO / URGÊNCIA]
- Tempo de consulta: [DURAÇÃO APROXIMADA]
- CID principal (se já definido): [CID-10]

FORMATO DA NOTA SOAP:

S (Subjetivo):
- Queixa principal com duração
- HDA em ordem cronológica, usando as palavras do paciente quando relevante
- Revisão de sistemas pertinente
- Medicações em uso (nome, dose, posologia, adesão)
- Alergias

O (Objetivo):
- Sinais vitais (incluir todos que foram aferidos)
- Exame físico dirigido (achados positivos e negativos pertinentes)
- Resultados de exames trazidos nesta consulta

A (Avaliação):
- Diagnóstico principal com CID-10
- Diagnósticos secundários/comorbidades com CID-10
- Raciocínio clínico breve (por que este diagnóstico e não outro)
- Classificação de risco ou estadiamento, quando aplicável

P (Plano):
- Prescrições (medicamento, dose, via, posologia, duração)
- Exames solicitados com justificativa breve
- Encaminhamentos
- Orientações dadas ao paciente
- Retorno: quando e com o quê

RESTRIÇÕES:
- Use terminologia médica adequada, mas mantenha clareza
- Não invente dados que não foram fornecidos — se faltar informação, escreva "[dado não informado]"
- Siga as convenções brasileiras de documentação clínica
- Inclua CID-10 para todos os diagnósticos
```

---

## Exemplo preenchido

```
Você é um médico clínico geral / médico de família experiente em documentação clínica no Brasil.

A partir das informações abaixo, gere uma nota clínica completa no formato SOAP para registro em prontuário eletrônico.

INFORMAÇÕES DA CONSULTA (anotações livres):
Dona Maria, 63 anos, retorno de DM2 e HAS. Trouxe exames. Tá tomando metformina 850 2x mas diz que às vezes esquece a da noite. Glifage. Losartana 50 2x. Diz que tá tudo bem, sem queixas novas. Perguntei sobre os pés, diz que às vezes formiga um pouco à noite mas passa. Nega feridas. Visão ok, fez oftalmo mês passado, tudo normal. Peso 78kg (tava 80 na última, emagreceu 2kg com caminhada). Altura 1,58. PA 138x88. Glicemia jejum 142, HbA1c 7,8 (era 8,2 há 6 meses). Creatinina 0,9. Microalbuminúria 45 mg/L. Colesterol total 210, LDL 138, HDL 42, TG 180. Pés: sensibilidade com monofilamento preservada, pulsos presentes. Vou aumentar metformina pra 1000 2x e adicionar empagliflozina 25mg pela microalbuminúria. Manter losartana. Orientei dieta, exercício. Pedido novo HbA1c em 3 meses. Retorno em 3 meses.

DADOS ADICIONAIS:
- Data da consulta: 10/04/2026
- Tipo de consulta: retorno
- Tempo de consulta: 20 minutos
- CID principal: E11 (DM2)

FORMATO DA NOTA SOAP:

S (Subjetivo):
- Queixa principal com duração
- HDA em ordem cronológica, usando as palavras do paciente quando relevante
- Revisão de sistemas pertinente
- Medicações em uso (nome, dose, posologia, adesão)
- Alergias

O (Objetivo):
- Sinais vitais (incluir todos que foram aferidos)
- Exame físico dirigido (achados positivos e negativos pertinentes)
- Resultados de exames trazidos nesta consulta

A (Avaliação):
- Diagnóstico principal com CID-10
- Diagnósticos secundários/comorbidades com CID-10
- Raciocínio clínico breve
- Classificação de risco ou estadiamento, quando aplicável

P (Plano):
- Prescrições (medicamento, dose, via, posologia, duração)
- Exames solicitados com justificativa breve
- Encaminhamentos
- Orientações dadas ao paciente
- Retorno: quando e com o quê

RESTRIÇÕES:
- Use terminologia médica adequada, mas mantenha clareza
- Não invente dados que não foram fornecidos — se faltar informação, escreva "[dado não informado]"
- Siga as convenções brasileiras de documentação clínica
- Inclua CID-10 para todos os diagnósticos
```

---

## Dicas de uso

- **Não se preocupe em organizar antes de colar**: o template foi feito para aceitar anotações bagunçadas. Quanto mais informação bruta você fornecer, melhor a nota gerada.
- **Revise sempre o output**: a IA pode interpretar dados ambíguos de forma incorreta. Confira especialmente doses de medicamentos e valores de exames.
- **Use com transcrição de áudio**: se você grava a consulta (com consentimento do paciente), cole a transcrição diretamente no campo de anotações livres.
- **Adapte para seu prontuário**: se o sistema do seu serviço exige campos específicos (ex.: classificação de risco de Framingham, escore FINDRISC), adicione nas restrições.

---

## Variações possíveis

| Variação | O que mudar no template |
|---|---|
| **Consulta de pronto-socorro** | Adicione campos: classificação de risco (Manchester/ESI), hora de chegada, tempo porta-médico, desfecho (alta/internação/observação) |
| **Consulta pediátrica** | Adicione: idade em meses, peso/estatura com percentil, vacinação em dia (sim/não), marcos do desenvolvimento, alimentação |
| **Nota de internação** | Altere para formato de evolução diária: subjetivo da manhã, exame físico do dia, balanço hídrico, ajustes de prescrição, pendências |
| **Telemedicina** | Adicione: "Nota de teleconsulta conforme Resolução CFM 2.314/2022. Plataforma utilizada: [nome]. Paciente conectado de: [local]. Termo de consentimento: obtido" |
| **Nota bilíngue (para convênio internacional)** | Adicione: "Após a nota em português, gere uma versão resumida em inglês para envio ao seguro saúde internacional" |
