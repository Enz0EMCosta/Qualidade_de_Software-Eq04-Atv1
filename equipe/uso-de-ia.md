# Declaração de Uso de IA Generativa (Enzo Emanuel Maia Costa)

| IA generativa | Finalidade | Prompt utilizado | Saída (resumo) |
|---|---|---|---|
| Claude | Gerar casos de teste | "Liste 12 casos de teste para avaliar a segurança do armazenamento de chaves de API e histórico de conversas em um cliente desktop de IA, incluindo cenários de dado sensível e indisponibilidade" | Retornou uma lista de casos de teste, incluindo cadastro sem chave (dado ausente), exposição da chave na interface (verificar mascaramento) e validação de formato de chave (entradas malformadas) |
| ChatGPT | Gerar casos de teste | Mesmo prompt acima | Retornou 12 casos focados em confidencialidade, proteção de credenciais, integridade e indisponibilidade, incluindo armazenamento da chave em repouso (texto puro vs. criptografada) e confiabilidade do armazenamento diante de falhas |
| Gemini | Estruturar requisitos de qualidade | "Sugira 10 requisitos de qualidade verificáveis para o gerenciamento de chaves de API" | Retornou 10 requisitos numerados, incluindo confidencialidade (chaves não devem ser armazenadas em texto puro), criptografia (chaves locais devem ser criptografadas) e controle de acesso |
| Copilot | Apoio na escrita/organização do relatório | "Revise este parágrafo sobre o arquivo readme.md do Cherry Studio, verifique erros de pontuação e duplicidade de palavras" | Revisou o arquivo conforme solicitado e corrigiu erros de gramática e coesão |
| Gemini | Auxílio e apoio à análise | "Explique em detalhes a licença de software do Cherry Studio (github.com/CherryHQ/cherry-studio), incluindo o modelo de licenciamento, restrições de uso comercial e se é permitido redistribuir versões modificadas." | Explicou que o Cherry Studio (Community Edition) é distribuído sob AGPL-3.0, descrevendo-a como uma das licenças mais rigorosas do ecossistema de software livre |

**O que foi aproveitado / corrigido / rejeitado:**

- *Aproveitado:* os casos de teste sugeridos por Claude e ChatGPT foram repassados como ponto de partida para a Seção 7 (Casos de Teste); os requisitos sugeridos pela Gemini serviram de base para a Seção 5 (Requisitos de Qualidade); a revisão do Copilot foi aplicada diretamente no README do repositório.
- *Corrigido:* a explicação da Gemini sobre a licença do Cherry Studio generalizou o AGPL-3.0 como "uma das licenças mais rigorosas do ecossistema de software livre", sem mencionar a particularidade específica do projeto: a existência de uma licença comercial adicional (Cherry Studio License Agreement) para empresas que desejam ficar isentas das exigências da AGPL-3.0. Essa lacuna foi identificada e corrigida manualmente pela equipe após conferência direta no repositório oficial.


**Verificações realizadas:** conferência manual da licença e da organização mantenedora diretamente no repositório oficial no GitHub, validação técnica dos casos de teste e requisitos sugeridos antes de repassá-los aos integrantes responsáveis pelas respectivas seções.

**Supervisão humana:** a IA generativa não foi utilizada como única autoridade de avaliação. Todas as sugestões produzidas pelas ferramentas de IA foram revisadas criticamente pela equipe antes de sua incorporação ao relatório final.
