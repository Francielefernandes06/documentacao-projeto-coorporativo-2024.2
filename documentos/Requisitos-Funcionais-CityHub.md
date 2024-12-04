## **2. Requisitos Funcionais**

| **ID** |  **Nome**  | **Descrição** | **Prioridade** | **Dependência** |
|--------|----------|---------------|----------------|-----------------|
| RF01   |  Cadastrar requisição  | O administrador deve cadastrar as requisições com os seguintes dados: descrição, dataCriação, usuário, departamento, prioridade, statusProcesso. | Alta | Nenhuma |
| RF02   |  Consultar requisição  | O cidadão e funcionário podem consultar o status de suas requisições, usando o protocolo da requisição desejada no filtro de busca na página Área do cidadão. | Alta | RF01 |
| RF03   |  Atualizar requisição  | O administrador pode editar informações de requisições, se necessárias, deve atualizar os dados:(RF01) + dataAtualização e anexa um comentário da atualização. | Alta | RF01 |
| RF04   |  Comentar requisição  | O cidadão, funcionário e administrador podem comentar as requisições cadastradas, na página Área do cidadão, haverá uma caixa de comentários que após preenchido clica o botão-comentar. | Média | RF01, RF03 |
| RF05  |  Cadastrar funcionário  | O administrador pode cadastrar funcionário, com os dados da conta google mais os dados: hierarquia, status e privilégio. | Alta |  |

---
