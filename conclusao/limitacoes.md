# Limitações

Esta avaliação está sujeita às seguintes limitações e premissas:

- **Recorte não avalia qualidade de resposta.** Conforme delimitado em contexto/ficha-tecnica.md, a equipe optou por avaliar gerenciamento de chaves de API, histórico de conversas, UX e segurança da aplicação. A qualidade do conteúdo gerado pelos modelos de LLM conectados não foi objeto desta análise.

- **Testes executados em um único provedor.** Os casos de teste e a análise de variabilidade foram executados conectando o Cherry Studio ao modelo gemini-flash-lite-latest via API key gratuita. O comportamento pode variar com outros provedores suportados pela ferramenta (OpenAI, Anthropic, DeepSeek, Qwen, modelos locais via Ollama).

- **Amostra limitada na análise de variabilidade.** Foram executados 5 prompts em 3 repetições cada (15 execuções no total). Esse volume permite identificar padrões gerais de variação textual, mas não é estatisticamente suficiente para generalizar a taxa de confabulação do modelo.

- **AC-03 não foi verificado empiricamente.** A lacuna sobre criptografia de chaves de API é uma lacuna de documentação identificada, não uma falha confirmada por teste prático. A equipe recomendou, mas não executou, a inspeção direta dos arquivos de configuração local.

- **Análise da ISO/IEC 25010:2023 baseada em documentação pública.** Conforme registrado na coluna "Limitação da Análise" de qualidade/modelo-iso25010.md, a avaliação não incluiu auditoria integral do código-fonte do repositório, apenas inspeção de documentação, README e comportamento observável na interface.

- **Ambiente de teste não replicado em múltiplas máquinas.** Os testes de desempenho e consumo de recursos foram realizados no ambiente de uma única máquina, sem variação de hardware entre os avaliadores.