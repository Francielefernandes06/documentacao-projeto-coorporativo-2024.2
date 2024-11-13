## **4. Regras de Negócio**

| **ID** | **Descrição**                                                                                                                            | **Prioridade** | **Dependência** |
| ------ | ---------------------------------------------------------------------------------------------------------------------------------------- | -------------- | --------------- |
| RN01   | O sistema deve validar as credenciais do usuário de forma que a senha nunca seja armazenada em texto simples.                            | Alta           | RF02            |
| RN02   | O usuário só poderá realizar requisições após completar o cadastro interno, informando sua hierarquia.                                   | Alta           | RF08            |
| RN03   | O sistema deve verificar se o email do usuário está vinculado ao cadastro do sistema antes de permitir o acesso ao portal do cidadão.    | Alta           | RF07            |
| RN04   | Caso o email do usuário não esteja cadastrado, o sistema deve solicitar o preenchimento do cadastro interno com a hierarquia do usuário. | Alta           | RF07            |

---
