### Caso de Uso: Cadastrar Requisição

| **ID**              | RF01                                                                                          |
|----------------------|-----------------------------------------------------------------------------------------------|
| **Nome**            | Cadastrar requisição                                                                          |
| **Ator**            | Administrador                                                                                 |
| **Fluxo Principal** | 1. O administrador acessa o sistema e escolhe a opção de cadastrar requisição.                |
|                      | 2. O administrador preenche os campos obrigatórios: descrição, dataCriação, usuário,          |
|                      |    departamento, prioridade, e statusProcesso.                                               |
|                      | 3. O sistema valida as informações fornecidas.                                               |
|                      | 4. O sistema salva a requisição no banco de dados e retorna uma mensagem de sucesso.         |
| **Fluxo Alternativo**| 1a. Caso algum campo obrigatório não seja preenchido ou inválido:                             |
|                      | - O sistema exibe uma mensagem de erro, informando os campos que precisam ser corrigidos.     |
| **Critérios**        | - Todos os campos obrigatórios devem ser preenchidos corretamente.                            |
|                      | - A data de criação deve ser gerada automaticamente no momento do cadastro.                  |

---

### Caso de Uso: Consultar Requisição

| **ID**              | RF02                                                                                          |
|----------------------|-----------------------------------------------------------------------------------------------|
| **Nome**            | Consultar requisição                                                                          |
| **Ator**            | Cidadão, Funcionário                                                                          |
| **Fluxo Principal** | 1. O usuário acessa a página *Área do Cidadão*.                                               |
|                      | 2. O usuário insere o protocolo da requisição no campo de busca.                              |
|                      | 3. O sistema valida o protocolo inserido.                                                    |
|                      | 4. O sistema exibe o status e os detalhes da requisição correspondente.                      |
| **Fluxo Alternativo**| 1a. Caso o protocolo seja inválido ou não exista:                                             |
|                      | - O sistema exibe uma mensagem informando que nenhuma requisição foi encontrada.             |
| **Critérios**        | - O usuário deve inserir um protocolo válido.                                                |

---

### Caso de Uso: Atualizar Requisição

| **ID**              | RF03                                                                                          |
|----------------------|-----------------------------------------------------------------------------------------------|
| **Nome**            | Atualizar requisição                                                                          |
| **Ator**            | Administrador                                                                                 |
| **Fluxo Principal** | 1. O administrador acessa o sistema e escolhe a opção de atualizar requisição.                |
|                      | 2. O administrador seleciona a requisição desejada para edição.                              |
|                      | 3. O administrador altera os dados necessários e insere a dataAtualização e um comentário.    |
|                      | 4. O sistema valida e salva as alterações realizadas.                                        |
| **Fluxo Alternativo**| 1a. Caso algum campo obrigatório não seja preenchido ou inválido:                             |
|                      | - O sistema exibe uma mensagem de erro, informando os campos que precisam ser corrigidos.     |
| **Critérios**        | - A dataAtualização deve ser gerada automaticamente ou informada pelo administrador.          |
|                      | - É necessário adicionar um comentário justificando a alteração.                             |

---

### Caso de Uso: Comentar Requisição

| **ID**              | RF04                                                                                          |
|----------------------|-----------------------------------------------------------------------------------------------|
| **Nome**            | Comentar requisição                                                                           |
| **Ator**            | Cidadão, Funcionário, Administrador                                                           |
| **Fluxo Principal** | 1. O usuário acessa a página *Área do Cidadão*.                                               |
|                      | 2. O usuário seleciona a requisição desejada.                                                |
|                      | 3. O usuário insere o comentário na caixa de texto e clica no botão de comentar.             |
|                      | 4. O sistema valida e salva o comentário vinculado à requisição.                             |
| **Fluxo Alternativo**| 1a. Caso o comentário esteja vazio:                                                           |
|                      | - O sistema exibe uma mensagem informando que o campo comentário não pode estar vazio.       |
| **Critérios**        | - O comentário deve ser vinculado à requisição correta e salvo com a identificação do autor.  |

---

### Caso de Uso: Cadastrar Funcionário

| **ID**              | RF05                                                                                          |
|----------------------|-----------------------------------------------------------------------------------------------|
| **Nome**            | Cadastrar funcionário                                                                         |
| **Ator**            | Administrador                                                                                 |
| **Fluxo Principal** | 1. O administrador acessa o sistema e escolhe a opção de cadastrar funcionário.               |
|                      | 2. O administrador insere os dados necessários: conta Google, hierarquia, status e privilégio.|
|                      | 3. O sistema valida as informações fornecidas.                                               |
|                      | 4. O sistema salva os dados do funcionário no banco de dados e retorna uma mensagem de sucesso.|
| **Fluxo Alternativo**| 1a. Caso algum campo obrigatório não seja preenchido ou inválido:                             |
|                      | - O sistema exibe uma mensagem de erro, informando os campos que precisam ser corrigidos.     |
| **Critérios**        | - Os dados do funcionário devem ser armazenados com os níveis de privilégio adequados.        |
