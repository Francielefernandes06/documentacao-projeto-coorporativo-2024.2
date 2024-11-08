#### EDILSON GOMES
#### FRANCIELE FERNANDES
# Planejamento do Projeto: Sistema de Gerenciamento de Prefeitura (Método Ágil - Scrum)
# CityHub

**Objetivo**: Entregar o sistema de forma incremental e interativo, priorizando as funcionalidades de maior valor para a prefeitura e seus cidadãos, com feedback constante dos stakeholders.

---

## Estrutura da Equipe

- **Product Owner (PO):** Representante da prefeitura, responsável por priorizar as funcionalidades, definir requisitos e manter o backlog atualizado.
- **Scrum Master:** Responsável por facilitar o processo ágil e remover impedimentos.
- **Time de Desenvolvimento:** Engenheiros de frontend (Angular), backend (Symfony), especialistas em banco de dados (PostgreSQL) e QA.
- **Stakeholders:** Usuários finais (gestores da prefeitura, cidadãos) que darão feedback nas revisões.

---

## Planejamento Inicial

### Kickoff do Projeto
- Onboarding inicial para alinhar expectativas e objetivos do projeto.
- Definição de funcionalidades principais, papéis e responsabilidades.
- Criação do roadmap macro com as funcionalidades mais importantes.

### Backlog do Produto
- Estruturar o backlog com base nos módulos principais: Autenticação, Gestão de Usuários, Gestão de Serviços, Portal do Cidadão, etc.
- Criar **épicos** (grandes funcionalidades) e **histórias de usuário** (descrições das funcionalidades específicas) para cada módulo.

---

## Ciclos de Sprints

O projeto será desenvolvido em **sprints de duas semanas** (ajustável), com cada sprint entregando funcionalidades prontas para uso ou teste.

### Estrutura de cada sprint:

- **Planejamento da Sprint:**  
  - O PO define as histórias de usuário prioritárias para a sprint, e a equipe estima o esforço necessário.
  - As histórias são quebradas em tarefas menores, com uma definição clara do que é “Pronto” (Definition of Done).

- **Desenvolvimento e Testes:**  
  - Durante as duas semanas, a equipe trabalha nas histórias, realizando testes contínuos.
  - O QA realiza testes manuais e automatizados para validar as funcionalidades desenvolvidas.

- **Reuniões Diárias (Daily Stand-up):**  
  - Reuniões curtas para discutir o progresso, o que foi feito, o que será feito e possíveis bloqueios.

- **Revisão da Sprint:**  
  - Apresentação das funcionalidades desenvolvidas para o PO e stakeholders.
  - Coleta de feedback para ajustes e melhorias.

- **Retrospectiva:**  
  - Análise do que funcionou bem e do que pode ser melhorado.
  - Ajustes no processo, se necessário, para a próxima sprint.

---

## Roadmap das Sprints

O desenvolvimento será realizado em **sprints de duas semanas** para garantir entregas contínuas e feedback constante dos stakeholders. Cada sprint terá entregas incrementais para atender ao escopo do projeto de forma gradual.

---

## **Sprint 1: MVP - Autenticação e Gestão de Usuários (2 semanas)**

### Objetivo:
Estabelecer a infraestrutura básica para autenticação de usuários e o controle de acesso ao sistema.

- **Funcionalidades:**
  - Implementação do sistema de login e controle de acesso.
  - Gerenciamento de permissões para diferentes tipos de usuários (cidadão, servidor e administrador).
  - Cadastro inicial de usuários e suas permissões.

- **Critérios de Conclusão:**
  - Usuários conseguem fazer login e acessar o sistema com permissões específicas.
  - Testes unitários para autenticação e autorização.

---

## **Sprint 2: Portal do Cidadão - Módulo Inicial (2 semanas)**

### Objetivo:
Criar a interface inicial para o Portal do Cidadão, onde cidadãos podem acessar informações e realizar solicitações.

- **Funcionalidades:**
  - Interface pública do portal com acesso básico a informações de serviços.
  - Visualização de informações pessoais e atualização de perfil para o cidadão.

- **Critérios de Conclusão:**
  - Portal acessível e funcionando com uma estrutura básica de navegação.
  - Testes de usabilidade e acessibilidade da interface.

---

## **Sprint 3: Gestão de Processos Administrativos - Fase 1 (2 semanas)**

### Objetivo:
Iniciar o módulo de Gestão de Processos Administrativos com cadastro e acompanhamento de processos.

- **Funcionalidades:**
  - Cadastro de processos administrativos como licenças e alvarás.
  - Estrutura para acompanhar a tramitação de processos e atualizações de status.

- **Critérios de Conclusão:**
  - Processos podem ser cadastrados e acompanhados no sistema.
  - Notificações automáticas de status de processos para os usuários.

---

## **Sprint 4: Integrações Externas - Fase Inicial (2 semanas)**

### Objetivo:
Configurar APIs e integração básica com sistemas externos para coleta e envio de dados.

- **Funcionalidades:**
  - Criação de APIs para comunicação com outros sistemas.
  - Configuração inicial para troca de dados externos (por exemplo, sistema de tributos).

- **Critérios de Conclusão:**
  - API funcionando com endpoints principais para dados externos.
  - Documentação das APIs para futuras integrações.

---

## **Sprint 5: Relatórios e Análises - Fase Inicial (2 semanas)**

### Objetivo:
Implementar relatórios básicos e painéis de indicadores para análise inicial de dados.

- **Funcionalidades:**
  - Geração de relatórios simples para acompanhamento de processos e dados de usuários.
  - Implementação de painel básico com KPIs de desempenho dos serviços.

- **Critérios de Conclusão:**
  - Relatórios gerados e exportáveis para análise.
  - Indicadores de desempenho disponíveis no painel de gestão.

---

## **Sprint 6: Portal do Cidadão - Funcionalidades Avançadas (2 semanas)**

### Objetivo:
Expandir as funcionalidades do Portal do Cidadão, adicionando novos recursos.

- **Funcionalidades:**
  - Implementação de consultas avançadas e emissão de boletos para tributos.
  - Inclusão de funcionalidades para acompanhar status de processos.

- **Critérios de Conclusão:**
  - Portal atualizado com funcionalidades avançadas.
  - Testes de usabilidade para novos recursos.

---

## **Sprint 7: Gestão de Serviços Públicos - Fase 1 (2 semanas)**

### Objetivo:
Desenvolver o módulo de Gestão de Serviços Públicos para cadastro e solicitação de serviços pela população.

- **Funcionalidades:**
  - Cadastro de serviços públicos e criação de fluxo de solicitação de serviços.
  - Registro de feedback dos cidadãos sobre os serviços.

- **Critérios de Conclusão:**
  - Cadastro de serviços e possibilidade de solicitação online.
  - Funcionalidade de feedback ativa e operacional.

---

## **Sprint 8: Gestão Financeira - Fase Inicial (2 semanas)**

### Objetivo:
Iniciar o módulo financeiro com funcionalidades básicas para controle de tributos.

- **Funcionalidades:**
  - Implementação do controle de arrecadação de impostos e taxas.
  - Emissão de boletos e relatórios financeiros iniciais.

- **Critérios de Conclusão:**
  - Módulo financeiro ativo com funcionalidades básicas.
  - Testes de emissão e validação de boletos.

---

## **Sprint 9: Gestão de Recursos Humanos - Fase 1 (2 semanas)**

### Objetivo:
Criar o módulo de RH com foco na gestão de dados dos servidores.

- **Funcionalidades:**
  - Cadastro e atualização de dados de servidores (cargos, qualificações, etc.).
  - Controle de escalas e férias dos servidores.

- **Critérios de Conclusão:**
  - Módulo de RH ativo com funcionalidades básicas.
  - Testes para validação dos dados dos servidores.

---

## **Sprint 10: Feedback e Ajustes Gerais (2 semanas)**

### Objetivo:
Realizar ajustes, melhorias e correções com base no feedback obtido ao longo do projeto.

- **Funcionalidades:**
  - Revisão de feedback dos stakeholders e ajustes de funcionalidades.
  - Correções de bugs identificados durante o uso inicial do sistema.

- **Critérios de Conclusão:**
  - Sistema ajustado e refinado com base no feedback.
  - Documentação atualizada e preparativos para a próxima fase.

---

## Reuniões de Revisão e Feedback

Para cada ciclo de sprints (2 a 3 sprints), faça uma reunião de revisão com os stakeholders para validar o progresso geral e ajustar o backlog de acordo com as novas necessidades ou mudanças de prioridade.

---

## Ferramentas Recomendadas

- **Gestão do Projeto:** O acompanhamento do progresso será realizada através do **GitHub Projetos**, por meio de issues e cards.
- **Controle de Código:** Git, utilizando GitHub, GitHub Actions (CI/CD).
- **Comunicação:** Discord para comunicação rápida e integração de atualizações.
- **Documentação:** Repositório no GitHub para manter uma documentação centralizada.

---

## Benefícios do Planejamento Ágil

- **Flexibilidade:** Capacidade de ajustar o projeto a novas necessidades.
- **Feedback Contínuo:** Validação das entregas com o PO e stakeholders, garantindo que o sistema atenda às expectativas.
- **Entrega Incremental:** Lançamento de funcionalidades em fases, possibilitando o uso gradual do sistema.
