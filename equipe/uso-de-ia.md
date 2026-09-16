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


# Declaração de Uso de IA Generativa — (Thayla Almeida Figueiredo)

## Stakeholders e Contexto de Uso

| IA generativa | Finalidade  | Prompt utilizado  | Saída (resumo) |
| ---| --- | --- |--- |
| **ChatGPT**   | Identificar as principais partes interessadas do Cherry Studio | "Identifique partes interessadas para uma análise de qualidade e segurança do Cherry Studio e, para cada uma, informe objetivo, expectativa, possíveis danos de falhas, evidências desejadas e responsabilidades." | Identificou como principais stakeholders o usuário final, desenvolvedor, auditor de segurança e gestor de TI, detalhando as responsabilidades e os impactos de possíveis falhas para cada um. |
| **Claude**    | Analisar o contexto real de utilização da ferramenta | "Descreva o contexto de uso de um aplicativo desktop que permite utilizar diferentes provedores de LLM em uma única interface. Considere supervisão humana, tipos de decisões apoiadas e consequências de erros." | Destacou que o Cherry Studio atua como intermediário entre o usuário e diferentes modelos de IA. Também indicou que o nível de supervisão deve variar de acordo com o risco da tarefa realizada. |
| **Gemini**    | Identificar riscos de respostas incorretas da IA | "Quais riscos podem ocorrer quando respostas geradas por uma IA estão incorretas? Considere usos em programação, pesquisas, ambiente corporativo, finanças, saúde e segurança." | Apontou riscos diferentes conforme o contexto, desde retrabalho em tarefas simples até vulnerabilidades, prejuízos financeiros, exposição de informações e danos graves em situações de alto risco.|
| **Copilot**   | Organizar e resumir o conteúdo para apresentação | "Resuma uma análise de stakeholders e contexto de uso do Cherry Studio em tópicos curtos para uma apresentação acadêmica." | Organizou o conteúdo em tópicos sobre stakeholders, funcionamento da ferramenta, supervisão humana e riscos de falhas da IA. |

**O que foi aproveitado / corrigido / rejeitado:**

* *Aproveitado:* a identificação de quatro stakeholders, suas responsabilidades e expectativas, além da classificação dos riscos de acordo com o contexto de utilização da ferramenta.
* *Corrigido:* algumas respostas foram simplificadas e adaptadas para evitar informações genéricas e deixar o conteúdo mais objetivo. Também foi reforçado que o Cherry Studio apenas fornece uma interface para diferentes modelos de IA e que as respostas geradas devem ser verificadas pelo usuário.
* *Rejeitado:* foram descartadas informações que não estavam diretamente relacionadas à avaliação de qualidade, segurança, confiabilidade e contexto de uso do Cherry Studio.

**Verificações realizadas:** as informações sugeridas pelas IAs foram comparadas com o contexto de funcionamento do Cherry Studio e revisadas manualmente. Os riscos foram analisados considerando o possível impacto de respostas incorretas em diferentes situações de uso.

**Supervisão humana:** as ferramentas de IA generativa foram utilizadas apenas como apoio à pesquisa, organização e elaboração do conteúdo. As respostas não foram consideradas como fonte única de informação, sendo revisadas e adaptadas manualmente antes de sua utilização no trabalho.

# Declaração de Uso de IA Generativa — (Douglas de Oliveira Déda)

## Casos de Teste - IA através do Cherry Studio

| IA generativa | Finalidade  | Prompt utilizado  | Saída (resumo) |
| ---| --- | --- |--- |
| **Claude**   | Gerar prompts para cada caso de teste | "Estamos fazendo uma atividade da materia de Qualidade de Software do curso de Sistemas de Informações. Precisamos analisar a qualidade de uma IA e para isso precisamos analisar os temas que estão na imagem (ambiguidade, falta de informação, etc...). Preciso que vc crie um documento com 3 prompts diferentes para analisar cada um dos tópicos solicitados." | Criou um documento robusto não só com os prompts mas uma formatação para avaliação de cada um deles, inclusive exemplificando as saídas esperadas. |


**O que foi aproveitado / corrigido / rejeitado:**

* *Aproveitado:* Toda a estrutura do documento foi usado para registrar os testes. Além disso, a maioria dos prompts também foram aprovados para usar no teste e eram coerentes com a proposta, com exceção de um que fugia um pouco da temática.
* *Corrigido:* Prompts de enviesamento estavam muito centrados em tópicos sensíveis como discriminação, xenofobia, etc... Não era o foco da avaliação.
* *Rejeitado:* Nada foi 100% descartado.

**Verificações realizadas:** Todos os prompts gerados foram validados se de fato falavam sobre o caso de teste em questão.

**Supervisão humana:** as ferramentas de IA generativa foram utilizadas apenas como apoio à pesquisa, organização e elaboração do conteúdo. As respostas não foram consideradas como fonte única de informação, sendo revisadas e adaptadas manualmente antes de sua utilização no trabalho.


# Declaração de Uso de IA Generativa (Vinícius Morais Souza)
| IA generativa | Finalidade | Prompt utilizado | Saída (resumo) |
|---|---|---|---|
| **ChatGPT** | Gerar casos de teste | "“Me gere 5 prompts de teste adequados, para testar a variabilidade e não determinismo de uma IA generativa” | “Resultados apresentados na Tabela de Registro de Prompt e Saída” |


# Declaração de Uso de IA Generativa (Rafael Souza Prata)
| IA generativa | Finalidade | Prompt utilizado | Saída (resumo) |
|---|---|---|---|
| **ChatGPT** | Com base exclusivamente nos dados e informações fornecidos sobre o Cherry Studio, gere 10 requisitos de qualidade (requisitos não funcionais) relacionados ao sistema. Para cada requisito, descreva de forma clara, objetiva e verificável a característica de qualidade que deve ser atendida, informe a respectiva área do requisito, como segurança, confiabilidade, desempenho, usabilidade, disponibilidade, manutenibilidade, compatibilidade, portabilidade, escalabilidade ou privacidade, e estabeleça critérios de aceitação objetivos que permitam verificar se o requisito foi atendido. Os requisitos devem ser específicos para o Cherry Studio, evitando características genéricas aplicáveis a qualquer sistema, e devem ser testáveis e mensuráveis sempre que possível. Evite critérios vagos, como “o sistema deve ser rápido” ou “o sistema deve ser seguro”, utilizando métricas ou condições concretas para validar cada requisito. Distribua os 10 requisitos entre diferentes áreas de qualidade e, ao final, apresente uma breve justificativa sobre a relevância de cada requisito para o Cherry Studio.” | “Resultados apresentados na Tabela de Inserida no Arquivo do trabalho” |
