
# Ficha Técnica do Projeto

**Aluno:** Enzo Emanuel Maia Costa (202300061901)

**Tarefa:** Analisar o repositório do Cherry Studio (README.md, arquivo de licença e página de releases no GitHub) para registrar a ficha técnica do projeto e delimitar o recorte de avaliação da equipe.

**Análise do artefato:**

O repositório do Cherry Studio é mantido pela organização CherryHQ, apresenta um README.md detalhado descrevendo a proposta da ferramenta: um cliente desktop multiplataforma (Windows, Mac e Linux) que unifica o acesso a diversos provedores de LLM — como OpenAI, Anthropic, Google Gemini, DeepSeek e Qwen, além de modelos locais via Ollama — em uma única interface de chat, com gerenciamento de assistentes personalizados, histórico de conversas e integrações via plugins e MCP.

A análise da licença revela um modelo híbrido: o projeto é distribuído sob AGPL-3.0, porém com termos comerciais adicionais (Cherry Studio License Agreement) que restringem a redistribuição de versões modificadas para fins comerciais sem autorização explícita da empresa mantenedora — particularidade que não fica evidente apenas pelo selo "open source" do repositório.

A leitura da documentação técnica mostrou ainda que o projeto não possui modelo de IA próprio, atuando como camada de orquestração sobre serviços de terceiros, o que torna o gerenciamento local de chaves de API e do histórico de conversas um ponto sensível do ponto de vista de segurança e privacidade.

**Dados registrados:**
- URL: https://github.com/CherryHQ/cherry-studio
- Organização responsável: CherryHQ
- Licença: AGPL-3.0 + termos comerciais adicionais (Cherry Studio License Agreement)
- Data de acesso: 13/09/2026
- Commit/tag/release avaliada: 

**Evidências:**

<img width="778" height="439" alt="image" src="https://github.com/user-attachments/assets/55585291-04f7-4936-8f87-e2e16cc5f821" />

<img width="1719" height="501" alt="image" src="https://github.com/user-attachments/assets/afb3b1e2-ec41-49ec-a2a6-533b803aa393" />
<img width="1896" height="706" alt="image" src="https://github.com/user-attachments/assets/a441edc4-e72b-4e5f-9c26-404bbd636e45" />

Este commit realiza uma alteração simples na interface do componente de seleção de modelos (`ModelSelector`).

* **O que mudou:** No arquivo `src/renderer/components/ModelSelector/ModelSelector.tsx`, o espaçamento horizontal entre as tags de filtro (*tag-chips*) foi aumentado de `gap-1` (4 pixels) para `gap-1.5` (6 pixels).
* **Objetivo:** Dar um respiro visual adequado entre os chips de filtro quando vários estão selecionados, melhorando o layout e a legibilidade sem alterar o comportamento de rolagem horizontal existente.
* **Contexto técnico:** O commit também serviu para rebasear uma Pull Request anterior (#18593) que estava em conflito devido a commits não relacionados que haviam vazado, limpando o histórico para manter apenas a modificação necessária de 1 linha.

