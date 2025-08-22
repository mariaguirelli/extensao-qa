## Cenário 03: Gestão de funcionários via módulo PIM.

### Caso de Teste 01: Adicionar novo funcionário com dados válidos.

| ID       | Descrição                                                          |
| :------- | :----------------------------------------------------------------- |
| C03-CT01 | O sistema deve permitir o cadastro de um funcionário com dados válidos. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e ter acesso ao módulo PIM.       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"PIM\"                     |
| **E** clica em \"Add Employee\"                                  |
| **E** preenche \"John\" no campo First Name e \"Doe\" no Last Name |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** o funcionário deve ser cadastrado e exibido na lista do PIM |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O funcionário deve aparecer corretamente listado no módulo PIM. |
Teste realizado e evidenciado.
https://jam.dev/c/34c9d2e7-cad6-4b27-a657-dcdc8005ccde
---

### Caso de Teste 02: Tentar adicionar funcionário sem preencher campos obrigatórios.

| ID       | Descrição                                                                  |
| :------- | :------------------------------------------------------------------------- |
| C03-CT02 | O sistema deve exibir erros ao tentar salvar um funcionário sem preencher os campos obrigatórios. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa a tela de \"Add Employee\"          |
| **E** deixa os campos obrigatórios em branco                     |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** mensagens de erro devem ser exibidas nos campos obrigatórios |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Os campos obrigatórios devem exibir mensagens de validação.     |
Teste realizado e evidenciado
https://jam.dev/c/f2a02f0a-17f7-4853-813a-e4a9eecf1195
---

### Caso de Teste 03: Pesquisar funcionário já cadastrado.

| ID       | Descrição                                                  |
| :------- | :--------------------------------------------------------- |
| C03-CT03 | O sistema deve retornar corretamente o funcionário pesquisado. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O funcionário deve já estar cadastrado no sistema.            |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"PIM\"                     |
| **E** digita \"John Doe\" no campo de busca                      |
| **QUANDO** clicar no botão \"Search\"                            |
| **ENTÃO** o sistema deve exibir \"John Doe\" na lista de resultados |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O funcionário correspondente deve ser listado corretamente.     |
Teste realizado e evidenciado
https://jam.dev/c/c479d3af-2b64-45e3-8a53-2ea4ba1685b7
