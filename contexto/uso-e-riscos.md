# Contexto de Uso e Riscos Identificados

**Aluno:** Enzo Emanuel Maia Costa (202300061901)

**Recorte avaliado:** gerenciamento de chaves de API, histórico de conversas, UX e segurança.

**Armazenamento de credenciais:**

A documentação oficial de configuração de provedores confirma que um mesmo provedor pode ter múltiplas chaves de API cadastradas, usadas em esquema de rotação sequencial. No entanto, a documentação pública não detalha se essas chaves são armazenadas com criptografia em repouso ou apenas em arquivo de configuração local em texto plano — trata-se de uma lacuna de documentação que a equipe recomenda verificar empiricamente (print de evidência a ser anexado por quem executar os testes práticos de segurança).

É importante também destacar que o projeto não possui modelo de IA próprio, atuando como camada de orquestração sobre serviços de terceiros — o que reforça o gerenciamento local de chaves de API e do histórico de conversas como ponto sensível do ponto de vista de segurança e privacidade.

**Resultados:**

A partir da ficha técnica levantada, a equipe delimitou como recorte de avaliação o gerenciamento de chaves de API, o histórico de conversas, a experiência do usuário (UX) e a segurança da aplicação — não sendo avaliada a qualidade das respostas geradas pelos modelos conectados. Essa delimitação se justifica pela natureza do Cherry Studio como orquestrador de LLMs de terceiros: o maior risco identificado não está na geração de conteúdo, mas em como a ferramenta armazena e protege dados sensíveis do usuário no dispositivo local, sem um console de administração centralizado.
