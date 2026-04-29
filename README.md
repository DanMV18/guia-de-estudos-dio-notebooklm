# Engenharia de Prompts e Contexto: Um Estudo com NotebookLM 🚀

Este repositório documenta um ciclo de estudos avançado sobre **Engenharia de Prompt e Otimização de Instruções**, utilizando o **NotebookLM** como ferramenta de síntese, análise e geração de insights. O foco principal é transcender o "vibe coding" e aplicar princípios de arquitetura de contexto para maximizar o desempenho de Modelos de Linguagem em Larga Escala (LLMs).

## 🎯 Contexto e Objetivos

O avanço da Inteligência Artificial Generativa transformou a interação com modelos em uma disciplina técnica. Este caderno temático foi criado para explorar como a estruturação de contextos e o refinamento algorítmico de instruções podem reduzir alucinações e aumentar a precisão em tarefas complexas.

**Objetivos de Estudo:**
* Compreender as diferenças entre técnicas de *Zero-shot*, *Few-shot* e *Chain-of-Thought* (CoT).
* Explorar a transição da Engenharia de Prompt para a **Engenharia de Contexto**.
* Validar métodos de otimização automatizada e avaliação de métricas (CMS, MSS, IOMS).
* Desenvolver um workflow de estudo eficiente utilizando a base de conhecimento do NotebookLM.

## 📚 Curadoria de Fontes

Para alimentar este estudo, foram selecionadas as seguintes fontes de alta relevância técnica:

1.  **Tratado sobre Engenharia de Prompt:** Arquiteturas de Instrução e Ciência da Contextualização (Guia Operacional).
2.  **Self-Consistency - Prompt Engineering Guide:** Documentação detalhada sobre caminhos de raciocínio diversos.
3.  **Prompt engineering | OpenAI API:** Melhores práticas oficiais da OpenAI para modelos de raciocínio.
4.  **Effective context engineering for AI agents - Anthropic:** Artigo sobre a gestão de recursos finitos de contexto.
5.  **DSPy Prompt Optimization:** Guia sobre a separação sistemática entre estrutura de programa e parâmetros de LLM.

## 🧪 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Nesta seção, documento o raciocínio por trás das interações e as dificuldades encontradas.

### Pergunta Estratégica 01: Comparação de Técnicas
**Prompt:** *"Com base nos documentos, explique a diferença fundamental entre Chain-of-Thought e Self-Consistency. Em quais cenários a Self-Consistency falha em comparação com CoT linear?"*

* **Resposta obtida:** A IA identificou corretamente que a Self-Consistency melhora o CoT ao amostrar múltiplos caminhos de raciocínio, mas inicialmente não detalhou o custo de tokens.
* **Ajuste (Troubleshooting):** Tive que iterar o prompt adicionando uma restrição: *"Inclua uma análise sobre o consumo de tokens e latência com base nos dados do Reddit e arXiv"*.
* **Lição aprendida:** Modelos tendem a focar na precisão qualitativa; restrições quantitativas precisam ser explicitadas.

### Pergunta Estratégica 02: Métricas de Avaliação
**Prompt:** *"Crie uma tabela comparativa entre as 5 métricas de relevância citadas pela Latitude.so (CMS, MSS, IOMS, CFR, PCI)."*

* **Dificuldade:** O NotebookLM inicialmente confundiu MSS com CMS por serem nomes similares.
* **Solução:** Refinei o contexto apontando o parágrafo específico do documento "Top 5 Metrics for Evaluating Prompt Relevance" para forçar a extração exata das definições.

## 📖 Miniguia de Estudo (Entrega Final)

### Resumo Estruturado
A engenharia de prompt moderna evoluiu de simples frases para **Pipelines de Otimização**. Técnicas como o **DSPy** permitem que os prompts sejam tratados como código, onde a estrutura é constante, mas as instruções são otimizadas automaticamente com base em métricas de sucesso, eliminando o erro humano do "tentativa e erro".

### Glossário de Conceitos Chave
* **Context Engineering:** Otimização da utilidade dos tokens disponíveis em um contexto limitado.
* **Hallucination (Alucinação):** Geração de informações factualmente incorretas, mitigada por técnicas de aterramento (Grounding).
* **Few-shot Prompting:** Fornecer exemplos de entrada/saída para condicionar o modelo a um padrão específico.
* **Prompt Drift:** Mudança no comportamento de um prompt devido a atualizações no modelo subjacente.

### 🛠️ Prompts Reutilizáveis
* **Para Revisão:** *"Aja como um especialista em IA. Resuma os conceitos de [Tema] focando em aplicações de produção e liste 3 possíveis falhas de segurança (adversarial prompting) relacionadas."*
* **Para Estruturação:** *"Transforme o texto técnico fornecido em um guia passo-a-passo no formato Markdown, destacando os termos técnicos em negrito e criando um glossário ao final."*
