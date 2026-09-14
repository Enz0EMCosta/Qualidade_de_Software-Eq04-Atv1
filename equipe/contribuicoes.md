# 📌 Divisão de Tarefas e Contribuições — Trabalho de Qualidade de Software (AV1)

> Este documento detalha a atribuição de responsabilidades, Seções do Relatório Técnico, escopo de apresentação nos slides/vídeo e manutenção do repositório para cada integrante da equipe.

---

## 📊 Visão Geral da Divisão

| Integrante | Seções do Relatório | Responsabilidade Principal | Papel no Vídeo / Slides |
| :--- | :--- | :--- | :--- |
| **Enzo** | Seções 1 e 10 | Recorte do Projeto & Governança de IA | Abertura, Introdução e Transparência de IA |
| **Thayla** | Seção 4 | Partes Interessadas & Contexto de Uso | Stakeholders e Impacto dos Riscos |
| **Douglas** | Seção 5 | Requisitos de Qualidade (RQ-01 a RQ-10) | Requisitos Críticos e Critérios de Aceitação |
| **Adam** | Seção 6 | Aplicação da Norma ISO/IEC 25010:2023 | Mapeamento da Norma ISO 25010 e Riscos |
| **[Nome do Integrante 5]** | Seção 7 | Casos de Teste (CT-01 a CT-12) & Evidências | Demonstração Prática de Testes e Logs |
| **Vinícius** | Seção 8 | Variabilidade, Não-Determinismo e Confabulação | Análise Prática de Variabilidade na IA |
| **Raphael** | Seção 9 + Git | Achados, Plano de Melhoria & Repositório | Achados e Gestão das Entregas do Git |

---

## 👤 Detalhamento por Integrante

### 1. Enzo
* **Papel:** Líder de Contexto e Governança de IA

#### 📄 Relatório Técnico
* **Seção 1 — Ficha Inicial e Recorte do Projeto:**
  * Descrever o repositório escolhido no GitHub, organização responsável e licença de software.
  * Registrar o *hash* do commit, *tag* ou *release* exata avaliada.
  * Definir a finalidade da ferramenta e delimitar o recorte específico (*ex: pipeline RAG, geração de SQL, logs, etc.*).
* **Seção 10 — Uso Crítico de IA Generativa:**
  * Montar a tabela declarando as IAs usadas pela equipe (ChatGPT, Claude, Gemini, etc.).
  * Listar até 5 prompts principais utilizados durante a pesquisa/escrita.
  * Registrar o que foi aproveitado, corrigido ou rejeitado (validação humana).

#### 📹 Vídeo e Slides
* Realizar a **abertura** e introdução da equipe.
* Apresentar o repositório selecionado e explicar o recorte delimitado.
* Explicar brevemente a transparência e governança no uso de IA generativa pela equipe.

---

### 2. Thayla
* **Papel:** Analista de Stakeholders e Impacto de Negócio

#### 📄 Relatório Técnico
* **Seção 4 — Partes Interessadas e Contexto de Uso:**
  * Mapear 4 partes interessadas (*ex: Usuário Final, Desenvolvedor, Auditor de Compliance, Gestor de TI*).
  * Detalhar para cada uma: objetivo, expectativa, possíveis danos de falhas, evidência desejada e responsabilidades.
  * Descrever o contexto de uso: nível de supervisão humana necessária, decisões apoiadas pela IA, limites de erros aceitáveis vs. inaceitáveis e impactos de respostas incorretas.

#### 📹 Vídeo e Slides
* Apresentar os stakeholders afetados.
* Explicar o contexto de uso real da ferramenta e os riscos/prejuízos em caso de falha da IA.

---

### 3. Douglas
* **Papel:** Engenheiro de Requisitos de Qualidade

#### 📄 Relatório Técnico
* **Seção 5 — Requisitos de Qualidade (RQ):**
  * Criar tabela com **no mínimo 10 Requisitos de Qualidade** verificáveis (`RQ-01` a `RQ-10`).
  * Cobrir categorias como: Rastreabilidade, Confiabilidade, Privacidade, Segurança, Desempenho, Usabilidade e Robustez.
  * Preencher para cada requisito: Descrição, Categoria, Prioridade (Baixa/Média/Alta), Critério de Aceitação e Evidência Esperada.

#### 📹 Vídeo e Slides
* Explicar os principais Requisitos de Qualidade especificados para a validação do sistema.
* Destacar os critérios de aceitação críticos definidos para garantir a qualidade.

---

### 4. Adam
* **Papel:** Especialista em Normas e Governança (ISO/IEC 25010)

#### 📄 Relatório Técnico
* **Seção 6 — Aplicação da Norma ISO/IEC 25010:2023:**
  * Mapear **no mínimo 6 características** da norma (*ex: Adequação Funcional, Confiabilidade, Segurança, Eficiência de Desempenho, Capacidade de Interação, Manutenibilidade*).
  * Para cada característica, detalhar: Pertinência para o sistema, Risco mapeado, Requisito associado, Método de avaliação, Evidência e Limitação da análise.

#### 📹 Vídeo e Slides
* Apresentar a estrutura da norma ISO 25010 aplicada ao contexto de software com IA.
* Explicar as características priorizadas e os riscos avaliados.

---

### 5. [Nome do Integrante 5]
* **Papel:** Analista de Testes e Garantia de Qualidade (QA)

#### 📄 Relatório Técnico
* **Seção 7 — Casos de Teste (CT) e Execução:**
  * Elaborar e executar **no mínimo 12 Casos de Teste** (`CT-01` a `CT-12`).
  * Cobrir cenários: Caso feliz, ambiguidade, falta de dados, fora do domínio, tentativa de *hallucination* (fontes inventadas), entradas muito curtas/longas, vazamento de dados sensíveis e indisponibilidade.
  * Preencher tabela contendo: Entrada, Condição, Esperado, Resultado Obtido, Nota (0, 1 ou 2) e Status.
  * Organizar e salvar todos os *prints* e *logs* na pasta `/evidencias`.

#### 📹 Vídeo e Slides
* Demonstrar a execução prática dos testes.
* Exibir *prints* e evidências destacando os pontos de sucesso e falhas da aplicação.

---

### 6. Vinícius
* **Papel:** Pesquisador de Robustez e Comportamento da IA

#### 📄 Relatório Técnico
* **Seção 8 — Análise de Variabilidade e Confabulação:**
  * Selecionar **5 prompts específicos** e executá-los em **3 repetições idênticas** (15 execuções no total).
  * Registrar para cada tentativa: Data/hora, parâmetros (*ex: temperatura, modelo*), resposta gerada e divergências.
  * Analisar a equivalência semântica, mudanças em fatos/fontes e se a variabilidade afeta a confiabilidade do sistema.

#### 📹 Vídeo e Slides
* Explicar como a IA se comporta em relação ao não-determinismo.
* Exibir exemplos práticos de respostas que variaram, destacando alucinações/confabulações identificadas.

---

### 7. Raphael
* **Papel:** Engenheiro de Melhoria Contínua e Maintainer do Repositório

#### 📄 Relatório Técnico
* **Seção 9 — Achados e Plano de Melhoria:**
  * Classificar **no mínimo 5 Achados** (bugs, falhas de segurança ou inconsistências) por gravidade (Baixa, Média, Alta, Crítica).
  * Estruturar o Plano de Melhoria: Ação recomendada, Responsável, Prioridade, Indicador de sucesso, Risco residual e Critério de conclusão.
* **Manutenção e Gestão do Repositório:**
  * Atualizar o `README.md` principal do GitHub com o resumo do projeto e link do vídeo.
  * Criar e preencher o arquivo `VIDEO.md` (URL do vídeo, data de gravação e identificação dos participantes).

#### 📹 Vídeo e Slides
* Apresentar os principais achados e o plano de ação/melhoria proposto.
* Garantir a entrega e integridade dos artefatos do repositório.

---

## 📅 Checklist de Entregáveis Gerais

- [ ] Pasta `/evidencias` criada e populada com logs e prints (Integrante 5).
- [ ] Relatório Técnico final revisado e consolidado.
- [ ] Slides da apresentação finalizados.
- [ ] Vídeo gravado e hospedado (Link no `VIDEO.md`).
- [ ] `README.md` atualizado com o link do vídeo e resumo do trabalho (Raphael).
- [ ] `VIDEO.md` criado no repositório (Raphael).
