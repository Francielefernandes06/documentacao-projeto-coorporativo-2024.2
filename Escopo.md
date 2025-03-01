*Edilson Gomes*  
*Franciele Fernandes*
---

### Escopo do Sistema Protocolar CityHub

**Objetivo:** 
Desenvolver um sistema protocolar que centralize a criação, o acompanhamento e a comunicação de requisições entre cidadãos e os departamentos municipais, promovendo transparência e eficiência no atendimento.

---

## 1. **O que o sistema CityHub vai fazer**

- ### **Criação e Registro de Protocolos**
  - Permitir que os cidadãos e os funcionários municipais registrem requisições de forma organizada.
  - Disponibilizar um identificador único para cada protocolo gerado.
  - Campos para registro de protocolo:
  
    - Título da requisição (obrigatório, texto de até 100 caracteres)
  - Descrição (texto livre para detalhamento da solicitação, até 500 caracteres)
  - Categoria (ex.: manutenção de vias, iluminação pública, coleta de lixo)
  - Data de abertura (gerada automaticamente)
  - Departamento responsável (seleção obrigatória com lista predefinida de departamentos)
  - Anexos (opcional, permite upload de arquivos PDF, imagens, etc.).
- ### **Gestão e Distribuição Interna de Requisições**
  - As requisições serão criadas por um departamento responsável.
  - Permitir atualizações de requisições, quando necessário.
  - Disponibilizar notificações internas para os responsáveis das requisições.
  - **Campos de atualização:**
    - **Status da requisição** (em análise, em execução, finalizado, cancelado)
    - **Responsável pelo atendimento** (seleção obrigatória de usuário do sistema)
    - **Comentários internos** (campo texto livre para anotações do departamento)
    - **Data de última atualização** (gerada automaticamente)
  - Disponibilizar **notificações internas** para os responsáveis quando uma requisição for atribuída ou atualizada.
- ### **Área do Cidadão**
  - Acompanhar o status das requisições em tempo real.
  - Notificar atualizações e mudanças de status das requisições de forma automática.
  - Disponibilizar caixa de comentários para a melhoria das requisições e serviços.
  - **Campos na área do cidadão:**
    - **Resumo da requisição** (título, status, última atualização)
    - **Detalhes** (descrição completa, categoria, anexos)
    - **Linha do tempo** (histórico de mudanças de status com data/hora)
    - **Comentários do cidadão** (campo aberto para feedback, limitado a 300 caracteres).
- ### **Controle de Status e Relatórios**
  - Permitir que o, departamento responsável das requisições, atualize o status dos protocolos (ex.: em análise, em execução, finalizado).
  - **Campos visíveis na tabela:**
    - Identificador único (número do protocolo)
    - Título
    - Status atual
    - Departamento responsável
    - Data de abertura
    - Última atualização.
  - Exportar **relatórios de requisições** em formato **PDF ou CSV** para análise interna.
- ### **Autenticação e Permissões**
  - Autenticação via google para evitar dados desnecessários.
  - Definir **privilégios de acesso** conforme hierarquia de usuários:
    - **Cidadão:** Criação e acompanhamento de protocolos próprios.
    - **Funcionário:** Visualização e gerenciamento de protocolos atribuídos ao seu departamento.
    - **Administrador:** Gerenciamento total do sistema, incluindo usuários e permissões
- ### **Notificações e Alertas**
  - Enviar notificações para a "Área do cidadão" sobre alterações nos status dos seus protocolos.
  - Disponibilizar **alertas internos** para os departamentos sobre:
    - Protocolos **prioritários** (sinalizados pelo administrador ou usuário)
    - Protocolos **atrasados** (baseados no tempo desde a criação ou no SLA configurado).

## 2. **O que o sistema CityHub não vai fazer**

- **Gestão Avançada de Processos**
  - Integração com sistemas de workflow para definir fluxos complexos de requisições.
  - Implementação de automação de processos para tarefas repetitivas, reduzindo o tempo de resposta.

- **Análise e Transparência Pública**
  - Desenvolver painéis com KPIs sobre o atendimento das requisições para auditorias e transparência.
  - Disponibilizar um histórico público das ações executadas por departamento, mantendo a privacidade de dados pessoais.

- **Integrações Externas**
  - Fornecer API pública para integração com outras plataformas de atendimento municipal.
  - Suporte para integração com sistemas de terceiros para notificações e atualizações automáticas.

### Conclusão

O *CityHub* é um sistema corporativo projetado para centralizar e gerenciar protocolos e requisições entre departamentos municipais, garantindo segurança, eficiência e controle no fluxo de informações, com acesso hierárquico e ferramentas de análise para otimizar o atendimento ao cidadão.
