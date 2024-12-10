*Edilson Gomes*  
*Franciele Fernandes*

**Sistema de protocolo para prefeituras \- CityHub**

**Objetivo:** Desenvolver um sistema protocolar que centralize a criação, o acompanhamento e a comunicação de requisições entre cidadãos e os departamentos municipais, promovendo transparência e eficiência no atendimento.

**Diagrama Caso de Uso**  
![][image1]

**Planejamento de Teste de Cenário**

#### **1\. Teste de Cenário: Cadastrar Requisição (Funcionário)**

**Pré-condições:**  
Usuário logado como funcionário.  
Campos obrigatórios disponíveis na interface.  
**Ações do Usuário:**  
Acessar o formulário de cadastro de requisição.  
Preencher os campos obrigatórios corretamente.  
Submeter o formulário.  
**Resultado Esperado:**  
Requisição salva com sucesso no banco de dados.  
Mensagem de sucesso exibida ao usuário.  
Registro disponível na lista de requisições.  
**Tipos de Teste:**  
Teste funcional.  
Teste de validação de campos.  
Teste de integração com o banco de dados.

#### **2\. Teste de Cenário: Atualizar Requisição (Funcionário)**

**Pré-condições:**  
Usuário logado como funcionário.  
Requisição existente no sistema.  
**Ações do Usuário:**  
Selecionar uma requisição existente.  
Alterar os campos permitidos.  
Salvar as alterações.  
**Resultado Esperado:**  
Alterações salvas com sucesso no banco de dados.  
Histórico atualizado com o comentário e data.  
Mensagem de sucesso exibida.  
**Tipos de Teste**:  
Teste funcional.  
Teste de fluxo de dados.  
Teste de UI/UX.

#### **3\. Teste de Cenário: Cadastrar Funcionário (Administrador)**

**Pré-condições:**  
Usuário logado como administrador com permissões adequadas.  
Dados do novo funcionário disponíveis.  
**Ações do Usuário:**  
Acessar a funcionalidade de cadastro de funcionário.  
Preencher os dados obrigatórios (e.g., conta Google, hierarquia).  
Submeter o formulário.  
**Resultado Esperado:**  
Novo funcionário registrado no sistema.  
Dados corretamente armazenados e exibidos.  
Mensagem de sucesso exibida.  
**Tipos de Teste:**  
Teste funcional.  
Teste de validação de permissões.  
Teste de validação de dados.

#### **4\. Teste de Cenário: Comentar Requisição (Cidadão/Funcionário)**

**Pré-condições:**  
Requisição existente no sistema.  
Usuário logado como cidadão ou funcionário.  
**Ações do Usuário:**  
Selecionar a requisição desejada.  
Inserir comentário na caixa de texto.  
Submeter o comentário.  
**Resultado Esperado:**  
Comentário vinculado à requisição com sucesso.  
Registro visível no histórico da requisição.  
Mensagem de sucesso exibida.  
**Tipos de Teste:**  
Teste funcional.  
Teste de validação de campos.  
Teste de integração com banco de dados.

#### **5\. Teste de Cenário: Consultar Requisição (Cidadão/Funcionário)**

**Pré-condições:**  
Requisição existente com protocolo válido.  
**Ações do Usuário:**  
Inserir o protocolo no campo de busca.  
Confirmar a busca.  
**Resultado Esperado:**  
**Se protocolo válido:**  
Status e detalhes da requisição exibidos.  
**Se protocolo inválido:**  
**Mensagem de erro:** "Protocolo não encontrado".  
**Tipos de Teste:**  
Teste funcional.  
Teste de fluxo alternativo (erro).  
Teste de integração.

### **Cenários de Teste**

#### **1\. Cadastrar Requisição (Funcionário)**

| CT | Entrada | Critérios | Resultado Esperado |
| :---- | :---- | :---- | :---- |
| CT-001 | Dados válidos: descrição, data, usuário, departamento, prioridade e status preenchidos. | Todos os campos obrigatórios devem estar preenchidos corretamente. | Requisição salva no banco de dados; mensagem de sucesso exibida. |
| CT-002 | Dados inválidos: campo obrigatório vazio ou dados em formato incorreto (ex.: data inválida). | Sistema deve validar os dados e impedir submissão com erro; exibir mensagem clara ao usuário. | Requisição não salva; mensagem de erro exibida informando campos que precisam ser corrigidos. |

#### **2\. Atualizar Requisição (Funcionário)**

| CT | Entrada | Critérios | Resultado Esperado |
| :---- | :---- | :---- | :---- |
| CT-003 | Selecionar requisição válida e editar campos permitidos com dados corretos. | Sistema deve permitir edição apenas de campos permitidos; dados devem ser válidos. | Alterações salvas no banco de dados; histórico atualizado; mensagem de sucesso exibida. |
| CT-004 | Selecionar requisição inválida ou tentar editar campos não permitidos. | Sistema deve bloquear edições de campos não autorizados ou alterações em requisições inexistentes. | Alterações não realizadas; mensagem de erro exibida informando motivo da falha. |

#### **3\. Cadastrar Funcionário (Adminstrador)**

| CT | Entrada | Critérios | Resultado Esperado |
| :---- | :---- | :---- | :---- |
| CT-005 | Dados válidos: conta Google, hierarquia, status e privilégio inseridos corretamente. | Todos os campos obrigatórios devem estar preenchidos corretamente; dados devem ser únicos no sistema. | Novo funcionário registrado no banco de dados; mensagem de sucesso exibida. |
| CT-006 | Dados inválidos: conta Google já existente ou hierarquia inválida. | Sistema deve validar unicidade de conta Google e integridade dos dados hierárquicos. | Cadastro não realizado; mensagem de erro exibida com descrição clara do problema. |

#### **4\. Comentar Requisição (Cidadão/Funcionário)**

| CT | Entrada | Critérios | Resultado Esperado |
| :---- | :---- | :---- | :---- |
| CT-007 | Comentário válido inserido na requisição existente. | Sistema deve aceitar comentários apenas em requisições existentes; texto deve ser não vazio. | Comentário salvo no banco de dados e vinculado à requisição; mensagem de sucesso exibida. |
| CT-008 | Comentário inválido: requisição inexistente ou texto vazio. | Sistema deve impedir envio de comentários inválidos. | Comentário não salvo; mensagem de erro exibida com informações sobre a falha. |

#### **5\. Consultar Requisição (Cidadão/Funcionário)**

| CT | Entrada | Critérios | Resultado Esperado |
| :---- | :---- | :---- | :---- |
| CT-009 | Protocolo válido inserido no campo de busca. | Sistema deve validar o protocolo e exibir os detalhes apenas se for válido. | Detalhes e status da requisição exibidos corretamente. |
| CT-010 | Protocolo inválido ou inexistente inserido no campo de busca. | Sistema deve identificar protocolo inválido e exibir mensagem clara. | Mensagem de erro exibida: "Protocolo não encontrado". |

**Casos de testes das três principais funcionalidades do sistema**

### **Caso de Teste: Cadastrar Requisição \- CT-001**

| Dados de Entrada | Ações Executadas | Resultado Esperado | Resultado Obtido |
| :---- | :---- | :---- | :---- |
| \- Descrição: "Conserto de iluminação pública". \- Usuário: "admin123". \- Departamento: "Infraestrutura". \- Prioridade: "Alta". \- Status: "Em andamento". | 1\. O administrador acessa o sistema. 2\. Seleciona a opção "Cadastrar Requisição". 3\. Preenche os campos obrigatórios com os dados fornecidos. 4\. Clica no botão "Salvar". | Requisição salva no banco de dados. Mensagem de sucesso: "Requisição cadastrada com sucesso". Data de criação gerada automaticamente. | \[A preencher após execução\] |

### **Caso de Teste: Cadastrar Funcionário \- CT-005**

| Dados de Entrada | Ações Executadas | Resultado Esperado | Resultado Obtido |
| :---- | :---- | :---- | :---- |
| \- Conta Google: "funcionario@gmail.com". \- Hierarquia: "Funcionário". \- Status: "Ativo". \- Privilégio: "Consulta". | 1\. O administrador acessa o sistema. 2\. Seleciona a opção "Cadastrar Funcionário". 3\. Preenche os campos obrigatórios com os dados fornecidos. 4\. Clica no botão "Salvar". | Funcionário cadastrado no banco de dados com os níveis de privilégio correspondentes. Mensagem de sucesso: "Funcionário cadastrado com sucesso". | \[A preencher após execução\] |

### **Caso de Teste: Cadastrar Funcionário \- CT-006 (conta existente)**

| Dados de Entrada | Ações Executadas | Resultado Esperado | Resultado Obtido |
| :---- | :---- | :---- | :---- |
| \- Conta Google: "existente@gmail.com". \- Hierarquia: "Administrador". \- Status: "Ativo". \- Privilégio: "Total". | 1\. O administrador acessa o sistema. 2\. Seleciona a opção "Cadastrar Funcionário". 3\. Insere uma conta Google já cadastrada. 4\. Clica no botão "Salvar". | Cadastro não realizado. Mensagem de erro: "Conta Google já existente no sistema". | \[A preencher após execução\] |

### **Caso de Teste: Consultar Requisição \- CT-009**

| Dados de Entrada | Ações Executadas | Resultado Esperado | Resultado Obtido |
| :---- | :---- | :---- | :---- |
| \- Protocolo: "REQ123456". | 1\. O usuário acessa a página "Área do Cidadão". 2\. Insere o protocolo válido "REQ123456" no campo de busca. 3\. Clica no botão "Consultar". | O sistema exibe os detalhes e o status da requisição correspondente ao protocolo "REQ123456". | \[A preencher após execução\] |

### **Caso de Teste: Consultar Requisição \- CT-010 (requisição inexistente)**

| Dados de Entrada | Ações Executadas | Resultado Esperado | Resultado Obtido |
| :---- | :---- | :---- | :---- |
| \- Protocolo: "REQINVALIDO". | 1\. O usuário acessa a página "Área do Cidadão". 2\. Insere o protocolo inválido "REQINVALIDO" no campo de busca. 3\. Clica no botão "Consultar". | O sistema exibe a mensagem de erro: "Protocolo não encontrado". | \[A preencher após execução\] |

[image1]: <data:image/png;base64,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>