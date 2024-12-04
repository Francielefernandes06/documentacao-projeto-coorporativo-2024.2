## **4. Regras de Negócio**

| **ID** | **Descrição**                                                                                                                            | **Prioridade** | **Dependência** |
| ------ | ---------------------------------------------------------------------------------------------------------------------------------------- | -------------- | --------------- |
| RN01   | O sistema não permite a exclusão de uma requisição cadastrada, caso a requisição for negada ou executada o sistema automaticamente arquiva a requisição.                            | Alta           | RF01, RF03            |
| RN02   | O funcionário só poderá realizar requisições após completar o cadastro interno, informando seu privilégio.                                   | Alta           | RF05, RNF01            |
| RN03   | O sistema deve verificar se o email do cidadão, funcionário ou administrador está vinculado ao cadastro do sistema antes de permitir o acesso a Área do cidadão.    | Alta           | RNF01            |

---
