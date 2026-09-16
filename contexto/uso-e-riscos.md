# Contexto de Uso e Riscos Identificados

**Aluno:** Enzo Emanuel Maia Costa (202300061901)

**Recorte avaliado:** gerenciamento de chaves de API, histórico de conversas, UX e segurança.

**Armazenamento de credenciais:**

A documentação oficial de configuração de provedores confirma que um mesmo provedor pode ter múltiplas chaves de API cadastradas, usadas em esquema de rotação sequencial. No entanto, a documentação pública não detalha se essas chaves são armazenadas com criptografia em repouso ou apenas em arquivo de configuração local em texto plano — trata-se de uma lacuna de documentação que a equipe recomenda verificar empiricamente (print de evidência a ser anexado por quem executar os testes práticos de segurança).

É importante também destacar que o projeto não possui modelo de IA próprio, atuando como camada de orquestração sobre serviços de terceiros — o que reforça o gerenciamento local de chaves de API e do histórico de conversas como ponto sensível do ponto de vista de segurança e privacidade.

**Resultados:**

A partir da ficha técnica levantada, a equipe delimitou como recorte de avaliação o gerenciamento de chaves de API, o histórico de conversas, a experiência do usuário (UX) e a segurança da aplicação — não sendo avaliada a qualidade das respostas geradas pelos modelos conectados. Essa delimitação se justifica pela natureza do Cherry Studio como orquestrador de LLMs de terceiros: o maior risco identificado não está na geração de conteúdo, mas em como a ferramenta armazena e protege dados sensíveis do usuário no dispositivo local, sem um console de administração centralizado.


# Contexto de Uso - Thayla Almeida Figueiredo

O Cherry Studio permite ao usuário acessar diferentes provedores de inteligência artificial em uma única interface. A ferramenta pode ser utilizada para pesquisas, criação de textos, programação, análise de informações e outras atividades que utilizem modelos de IA.

### Nível de Supervisão Humana

A necessidade de supervisão depende do risco da atividade:

- **Baixo risco:** tarefas como brainstorming, geração de ideias e criação de textos simples podem ter menor nível de supervisão.
- **Médio risco:** programação, trabalhos acadêmicos e análise de informações exigem revisão do usuário.
- **Alto risco:** atividades relacionadas à saúde, finanças, questões jurídicas, segurança e informações confidenciais exigem supervisão humana especializada.

### Decisões Apoiadas pela IA

A IA pode auxiliar o usuário em:

- Análise de informações;
- Pesquisas;
- Programação;
- Criação e revisão de documentos;
- Comparação de alternativas;
- Planejamento e geração de ideias.

A IA deve atuar como ferramenta de apoio, enquanto a decisão final permanece sob responsabilidade humana.

### Erros Aceitáveis

São considerados aceitáveis erros de baixo impacto que possam ser identificados e corrigidos pelo usuário, como:

- Pequenas falhas de escrita;
- Sugestões inadequadas em brainstorming;
- Respostas incompletas;
- Informações incorretas em tarefas simples, desde que sejam revisadas antes da utilização.

### Erros Inaceitáveis

São considerados inaceitáveis erros ou falhas que possam causar impactos significativos, como:

- Vazamento de dados pessoais ou corporativos;
- Exposição de chaves de API ou credenciais;
- Perda ou corrupção de informações;
- Acesso não autorizado;
- Execução de ações perigosas sem autorização;
- Utilização de informações incorretas em decisões de alto impacto.

### Impactos de Respostas Incorretas

O impacto de uma resposta incorreta depende da finalidade do uso:

- **Tarefas simples:** podem causar retrabalho.
- **Programação:** podem gerar bugs e vulnerabilidades.
- **Ambiente acadêmico:** podem resultar em informações incorretas no trabalho.
- **Ambiente corporativo:** podem levar a decisões ou procedimentos inadequados.
- **Finanças:** podem causar prejuízos financeiros.
- **Saúde e segurança:** podem causar danos significativos.
