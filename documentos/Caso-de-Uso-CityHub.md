## **1. Casos de Uso**

### **UC01 - Cadastro de Usuário**

| **Campo**              | **Descrição**                                                                                       |
|------------------------|-----------------------------------------------------------------------------------------------------|
| **ID**                 | UC01                                                                                                 |
| **Ator**               | Cidadão, Funcionário, Administrador                                                                  |
| **Descrição**          | O sistema permite o cadastro de novos usuários.                                                     |
| **Fluxo Principal**    | 1. O usuário preenche seus dados no formulário de cadastro.<br>2. O sistema valida as informações e cria um novo usuário.<br>3. O sistema envia um e-mail de confirmação. |
| **Fluxos Alternativos**| A1. Se o usuário já estiver registrado, o sistema exibe uma mensagem de erro.                       |
| **Pré-Condições**      | O usuário não pode estar cadastrado previamente.                                                    |

---

### **UC02 - Autenticação de Usuário**

| **Campo**              | **Descrição**                                                                                       |
|------------------------|-----------------------------------------------------------------------------------------------------|
| **ID**                 | UC02                                                                                                 |
| **Ator**               | Cidadão, Funcionário, Administrador                                                                  |
| **Descrição**          | O sistema permite que o usuário realize login com a senha cadastrada.                             |
| **Fluxo Principal**    | 1. O usuário insere suas credenciais.<br>2. O sistema valida e autentica o usuário.<br>3. O sistema redireciona o usuário para o portal do cidadão. |
| **Fluxos Alternativos**| A1. Se as credenciais estiverem incorretas, o sistema solicita nova tentativa de login.            |
| **Pré-Condições**      | O usuário deve estar cadastrado no sistema.                                                         |

---

### **UC03 - Consultar Status de Requisição**

| **Campo**              | **Descrição**                                                                                       |
|------------------------|-----------------------------------------------------------------------------------------------------|
| **ID**                 | UC03                                                                                                 |
| **Ator**               | Cidadão, Funcionário, Administrador                                                                  |
| **Descrição**          | O usuário consulta o status de suas requisições através do portal do cidadão.                      |
| **Fluxo Principal**    | 1. O usuário acessa o portal do cidadão.<br>2. O sistema exibe uma lista das requisições do usuário.<br>3. O usuário seleciona a requisição desejada para consultar seu status. |
| **Fluxos Alternativos**| A1. Se o usuário não tiver requisições registradas, o sistema exibe uma mensagem informando a ausência de requisições. |
| **Pré-Condições**      | O usuário deve estar autenticado e possuir requisições registradas.                                 |

---

### **UC04 - Editar Requisição**

| **Campo**              | **Descrição**                                                                                       |
|------------------------|-----------------------------------------------------------------------------------------------------|
| **ID**                 | UC04                                                                                                 |
| **Ator**               | Funcionário, Administrador                                                                          |
| **Descrição**          | O funcionário ou administrador pode editar informações de uma requisição registrada.               |
| **Fluxo Principal**    | 1. O usuário seleciona uma requisição para editar.<br>2. O sistema exibe o formulário de edição.<br>3. O usuário modifica as informações necessárias.<br>4. O sistema valida e salva as alterações. |
| **Fluxos Alternativos**| A1. Se o usuário não tiver permissão para editar a requisição, o sistema exibe uma mensagem de erro. |
| **Pré-Condições**      | O usuário deve ser um funcionário ou administrador autenticado.                                     |

---

### **UC05 - Aprovar/Negar Requisição**

| **Campo**              | **Descrição**                                                                                       |
|------------------------|-----------------------------------------------------------------------------------------------------|
| **ID**                 | UC05                                                                                                 |
| **Ator**               | Administrador                                                                                        |
| **Descrição**          | O administrador aprova ou nega as requisições submetidas pelos cidadãos ou funcionários.            |
| **Fluxo Principal**    | 1. O administrador acessa o portal de gestão de requisições.<br>2. O sistema exibe uma lista de requisições pendentes.<br>3. O administrador seleciona uma requisição para aprovar ou negar.<br>4. O sistema registra a ação e altera o status da requisição. |
| **Fluxos Alternativos**| A1. Se o administrador não tiver permissão para aprovar/negá-la, o sistema exibe uma mensagem de erro. |
| **Pré-Condições**      | O usuário deve ser um administrador autenticado.                                                    |

---

### **UC06 - Excluir Requisição**

| **Campo**              | **Descrição**                                                                                       |
|------------------------|-----------------------------------------------------------------------------------------------------|
| **ID**                 | UC06                                                                                                 |
| **Ator**               | Funcionário, Administrador                                                                          |
| **Descrição**          | O sistema permite ao funcionário ou administrador excluir uma requisição registrada.               |
| **Fluxo Principal**    | 1. O usuário seleciona uma requisição para excluir.<br>2. O sistema exibe uma confirmação de exclusão.<br>3. O usuário confirma a exclusão.<br>4. O sistema exclui a requisição. |
| **Fluxos Alternativos**| A1. Se o usuário não tiver permissão para excluir a requisição, o sistema exibe uma mensagem de erro. |
| **Pré-Condições**      | O usuário deve ser um funcionário ou administrador autenticado.                                     |

---

### **UC07 - Autenticação via Google**

| **Campo**              | **Descrição**                                                                                       |
|------------------------|-----------------------------------------------------------------------------------------------------|
| **ID**                 | UC07                                                                                                 |
| **Ator**               | Cidadão, Funcionário, Administrador                                                                  |
| **Descrição**          | Permite que o usuário realize login no sistema utilizando sua conta Google.                        |
| **Fluxo Principal**    | 1. O usuário acessa a página de login do portal.<br>2. O sistema oferece a opção de autenticação via Google.<br>3. O usuário clica em "Login com Google".<br>4. O sistema redireciona o usuário para a tela de login do Google.<br>5. O usuário fornece suas credenciais do Google e concede permissão para o sistema acessar seu email.<br>6. O sistema valida a autenticação com o Google e recupera o email do usuário.<br>7. O sistema registra a autenticação e vincula o usuário ao sistema, verificando se o email já está cadastrado.<br>8. O sistema direciona o usuário para o portal do cidadão. |
| **Fluxos Alternativos**| A1. Se o email não estiver cadastrado, o sistema solicita que o usuário se registre, informando sua hierarquia.<br>A2. Se o token do Google expirar, o sistema solicita ao usuário que realize novamente o login. |
| **Pré-Condições**      | O usuário deve ter uma conta Google ativa.                                                          |

---

### **UC08 - Cadastro Interno para Requisição**

| **Campo**              | **Descrição**                                                                                       |
|------------------------|-----------------------------------------------------------------------------------------------------|
| **ID**                 | UC08                                                                                                 |
| **Ator**               | Cidadão, Funcionário, Administrador                                                                  |
| **Descrição**          | Permite que o usuário, após autenticação via Google, se cadastre no sistema interno e informe sua hierarquia (cidadão, funcionário ou administrador). |
| **Fluxo Principal**    | 1. O usuário, ao acessar o portal do cidadão, é redirecionado para a tela de cadastro interno.<br>2. O sistema solicita que o usuário informe sua hierarquia.<br>3. O usuário escolhe entre as opções: Cidadão, Funcionário ou Administrador.<br>4. O sistema registra as informações e cria o perfil interno do usuário.<br>5. O usuário passa a ter acesso completo para realizar requisições, dependendo de sua hierarquia. |
| **Fluxos Alternativos**| A1. Se o usuário não informar a hierarquia, o sistema exibe uma mensagem de erro e solicita o preenchimento. |
| **Pré-Condições**      | O usuário deve estar autenticado via Google.                                                        |

---

### **UC09 - Realização de Requisição**

| **Campo**              | **Descrição**                                                                                       |
|------------------------|-----------------------------------------------------------------------------------------------------|
| **ID**                 | UC09                                                                                                 |
| **Ator**               | Cidadão, Funcionário, Administrador                                                                  |
| **Descrição**          | Permite que o usuário registre uma nova requisição no sistema.                                      |
| **Fluxo Principal**    | 1. O usuário preenche os dados necessários para a requisição.<br>2. O sistema valida as informações e cria uma nova requisição.<br>3. O sistema gera um número de protocolo e atualiza o status da requisição. |
| **Fluxos Alternativos**| A1. Se algum dado obrigatório não for preenchido, o sistema solicita correção e exibe uma mensagem de erro. |
| **Pré-Condições**      | O usuário deve ter cadastro interno e permissão para realizar requisições.                         |

---
