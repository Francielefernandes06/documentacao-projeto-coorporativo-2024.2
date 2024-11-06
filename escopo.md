**EDILSON GOMES**

**FRANCIELE FERNANDES**



## **Escopo do Projeto: Sistema de Gerenciamento de Prefeitura**

**Objetivo do Projeto**

Desenvolver um sistema integrado para gerenciar as atividades, dados e serviços oferecidos pela prefeitura, centralizando informações e otimizando a administração de serviços públicos. O sistema permitirá uma comunicação mais eficaz entre os departamentos e melhorará a eficiência na gestão de processos internos e atendimento ao cidadão.

**Premissas do Projeto** 

\- O sistema será acessível para diferentes tipos de usuários com permissões específicas: cidadão, servidor, gestor e administrador.

\- Será desenvolvido utilizando uma arquitetura moderna, modular e escalável, com Angular para o frontend, Symfony para o backend e PostgreSQL para o banco de dados.

\- A segurança e a proteção de dados pessoais são fundamentais, respeitando as regulamentações da LGPD.

 

**Funcionalidades Principais**

- **Autenticação e Autorização**
  - Login seguro integrado ao sistema da Prefeitura, com autenticação baseada em níveis de usuário (ex: cidadão, servidor, gestor, administrador).
  - Gerenciamento de permissões baseado em funções para acesso a módulos específicos.

- **Gestão de Usuários**
  - Cadastro e atualização de perfis de cidadãos e servidores.
  - Visualização e edição de informações pessoais (limita-se ao perfil do cidadão, quando aplicável).
  - Gerenciamento de permissões e acesso por nível hierárquico.

- **Gestão de Serviços Públicos**
  - Cadastro e gerenciamento de serviços públicos disponíveis, como emissão de documentos, atendimento médico, manutenção de infraestrutura.
  - Solicitações de serviço pelos cidadãos, incluindo o acompanhamento do status do atendimento.
  - Feedback de usuários sobre os serviços prestados e registros históricos de atendimentos.

- **Gestão de Recursos Humanos**
  - Registro e atualização de dados dos servidores públicos, incluindo cargo, setor e qualificações.
  - Controle de escalas de trabalho, horários, férias e licenças.
  -  Avaliações de desempenho e registro de treinamentos e formações dos servidores.

- **Gestão de Processos Administrativos**
  - Gerenciamento de processos administrativos, como solicitações de licenças de construção, alvarás e certidões.
  - Acompanhamento de tramitação de documentos e atualizações de status dos processos.
  - Notificações automáticas sobre prazos e vencimentos de documentos.

- **Gestão Financeira**
  - Controle de arrecadação de impostos municipais e taxas, com emissão de boletos e relatórios.
  - Gerenciamento de orçamento e despesas dos departamentos, com relatórios financeiros periódicos.
  - Monitoramento de contratos e fornecedores com controle de pagamentos e vencimentos.

- **Portal do Cidadão**
  - Interface pública para que cidadãos possam acessar informações de serviços e fazer solicitações online.
  - Emissão de boletos para pagamento de tributos e taxas municipais.
  - Consulta a status de solicitações e visualização de documentos públicos relevantes.

- **Gestão de Patrimônio e Infraestrutura**
  - Cadastro e monitoramento de bens patrimoniais, incluindo manutenção de prédios públicos e equipamentos.
  - Controle de inventário de equipamentos e mobiliário, com histórico de uso e manutenção.
  - Planejamento e controle de obras públicas e manutenção de infraestrutura urbana.

- **Relatórios e Análises**
  - Geração de relatórios sobre o desempenho de cada departamento, demandas de serviços e satisfação dos cidadãos.
  - Painel com indicadores de desempenho (KPIs) para apoio na tomada de decisão.
  - Análise de dados históricos para previsão de demandas futuras.

- **Integrações Externas**
  - Integração com outros sistemas governamentais e bases de dados estaduais ou federais, quando aplicável.
  - API pública para acesso controlado a dados relevantes para outras plataformas e aplicações.

**Requisitos Técnicos**

- **Frontend:** Angular para construção da interface, responsiva e acessível.
- **Backend:** Symfony, com APIs RESTful para comunicação com o frontend.
- **Banco de Dados:** PostgreSQL para armazenamento dos dados, garantindo segurança e integridade.
- **Hospedagem e Infraestrutura:** Nuvem (Azure) com balanceamento de carga via HAproxy para escalabilidade e alta disponibilidade.
- **Segurança:** Autenticação via token (JWT) e criptografia de dados sensíveis; compliance com LGPD.

 

**Cronograma Resumido**

1. **Planejamento e Análise de Requisitos:** 1 mês
2. **Design e Arquitetura do Sistema:** 1 mês
3. **Desenvolvimento de Funcionalidades Base:** 3 meses
4. **Integração e Testes:** 2 meses
5. **Lançamento e Treinamento de Usuários:** 1 mês
6. **Manutenção e Suporte:** Contínuo pós-lançamento

**Orçamento Estimado**

O orçamento incluirá:

\- Recursos para desenvolvimento (equipe de desenvolvimento e infraestrutura).

\- Ferramentas de monitoramento e segurança.

\- Custos de hospedagem e manutenção na nuvem.

 

**Riscos e Mitigações**

- **Risco:** Mudança de escopo durante o desenvolvimento.
- **Mitigação:** Reuniões periódicas com stakeholders para alinhamento.

**Conclusão**

Este escopo fornece uma visão clara e detalhada das expectativas para **o sistema de gerenciamento da prefeitura**. Com isso, a equipe poderá se guiar ao longo do desenvolvimento para garantir a entrega de um produto de alta qualidade e que atenda às necessidades dos cidadãos e gestores. 