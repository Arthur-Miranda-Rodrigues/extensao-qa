Aqui está a consolidação dos cenários e casos de teste em formato Markdown (pronto para o arquivo `CT_RF19_ Aba de gestão principal.md`), estruturado no mesmo padrão apresentado.

---

# Cenário de Testes: Aba de Gestão Principal (RF19)

---

## Caso de Teste 01: Gerenciamento de Colaboradores

| ID | Descrição |
| --- | --- |
| RF19-CT01 | Verificar a pesquisa, cadastro, gerenciamento de funções e exclusão de colaboradores no sistema.

 |

| **Pré-condições** |
| --- |
| O usuário deve estar autenticado com permissões administrativas na aba de gestão.

 |

| **Passos** |
| --- |
| **DADO** que o usuário está na tela de gerenciamento de Colaboradores

<br>

<br>**QUANDO** realizar a pesquisa por código ou nome

<br>

<br>**ENTÃO** o sistema deve filtrar e exibir os registros correspondentes.

<br>

<br>**E QUANDO** clicar no botão "Novo Colaborador" e preencher os dados obrigatórios e opcionais (Nome, Status, Nascimento, Sexo, Tipo Sanguíneo, Documentos, Login/Senha, Contato, Endereço, Biometria e Observação)

<br>

<br>**ENTÃO** o registro do colaborador deve ser salvo com sucesso.

<br>

<br>**E QUANDO** acessar o modal "Gerenciar Funções" de um colaborador

<br>

<br>**ENTÃO** deve ser possível vincular ou remover funções/permissões (ex: "Treinador da academia", "Personal Externo").

<br>

<br>**E QUANDO** selecionar as opções de visualização, edição ou exclusão

<br>

<br>**ENTÃO** o sistema deve permitir a alteração e deleção do cadastro.

 |

| **Critérios de aceitação** |
| --- |
| O sistema deve realizar a busca, a inclusão completa, a vinculação de funções e a manutenção do cadastro de colaboradores sem divergências de dados.

 |

---

## Caso de Teste 02: Gerenciamento de Atividades

| ID | Descrição |
| --- | --- |
| RF19-CT02 | Verificar a busca, criação e edição de atividades no sistema.

 |

| **Pré-condições** |
| --- |
| O usuário deve estar autenticado no sistema com acesso ao módulo de atividades.

 |

| **Passos** |
| --- |
| **DADO** que o usuário está na tela de Atividades

<br>

<br>**QUANDO** utilizar os filtros de pesquisa

<br>

<br>**ENTÃO** as atividades cadastradas devem ser filtradas corretamente.

<br>

<br>**E QUANDO** cadastrar uma nova atividade (ex: "Treino de perna" com pontuação e descrição)

<br>

<br>**ENTÃO** a atividade deve ser salva no banco de dados.

<br>

<br>**E QUANDO** editar os dados de uma atividade existente

<br>

<br>**ENTÃO** as alterações devem ser atualizadas com sucesso.

 |

| **Critérios de aceitação** |
| --- |
| A busca, inclusão e edição de atividades devem ser processadas corretamente.

 |

---

## Caso de Teste 03: Gerenciamento de Tipos de Documentos

| ID | Descrição |
| --- | --- |
| RF19-CT03 | Verificar a consulta, criação, alteração de escopo e exclusão de tipos de documentos.

 |

| **Pré-condições** |
| --- |
| O usuário deve estar logado e possuir permissões de configuração de documentos.

 |

| **Passos** |
| --- |
| **DADO** que o usuário está na tela de Tipos de Documentos

<br>

<br>**QUANDO** pesquisar por código e nome

<br>

<br>**ENTÃO** os tipos cadastrados devem ser exibidos na listagem.

<br>

<br>**E QUANDO** criar um novo tipo de documento (ex: "Eventos")

<br>

<br>**ENTÃO** o novo tipo deve ser cadastrado com sucesso.

<br>

<br>**E QUANDO** alterar o escopo/aplicação do documento (ex: entre "Conta / Fornecedor" e "Colaborador")

<br>

<br>**ENTÃO** o escopo deve ser atualizado.

<br>

<br>**E QUANDO** solicitar a exclusão de um tipo de documento

<br>

<br>**ENTÃO** o item deve ser removido do sistema.

 |

| **Critérios de aceitação** |
| --- |
| Todas as operações de CRUD e alteração de escopo para tipos de documentos devem funcionar conforme especificado.

 |

---

## Caso de Teste 04: Gerenciamento de Fornecedores

| ID | Descrição |
| --- | --- |
| RF19-CT04 | Verificar a busca, inclusão, consulta e edição de fornecedores.

 |

| **Pré-condições** |
| --- |
| O usuário deve estar autenticado e na tela de gestão de Fornecedores.

 |

| **Passos** |
| --- |
| **DADO** que o usuário acessou a tela de Fornecedores

<br>

<br>**QUANDO** efetuar a pesquisa de fornecedores

<br>

<br>**ENTÃO** a lista deve retornar os cadastros encontrados.

<br>

<br>**E QUANDO** clicar para incluir um novo fornecedor (ex: "Jeremias Castro") preenchendo dados pessoais, contato, endereço e observações

<br>

<br>**ENTÃO** o registro deve ser salvo com sucesso.

<br>

<br>**E QUANDO** abrir os detalhes de um cadastro existente para visualização ou edição

<br>

<br>**ENTÃO** as informações devem ser exibidas e alteradas corretamente.

 |

| **Critérios de aceitação** |
| --- |
| A inclusão e a manutenção das informações de fornecedores devem funcionar perfeitamente.

 |

---

## Caso de Teste 05: Gerenciamento e Permissões de Funções

| ID | Descrição |
| --- | --- |
| RF19-CT05 | Verificar busca, criação de funções, atribuição de permissões e visualização.

 |

| **Pré-condições** |
| --- |
| O usuário deve estar autenticado com acesso à tela de Funções.

 |

| **Passos** |
| --- |
| **DADO** que o usuário está na tela de Funções

<br>

<br>**QUANDO** pesquisar por código (ex: #3, #4), por nome ("Proprietário") ou filtrar por tipo ("Todos", "Externo", "Interno")

<br>

<br>**ENTÃO** os resultados devem corresponder aos filtros aplicados.

<br>

<br>**E QUANDO** cadastrar a função "Treinador de Apoio" (Tipo: Externo, Personal: Sim, Avaliador: Sim)

<br>

<br>**ENTÃO** a função deve ser salva com sucesso (gerando código, ex: #8).

<br>

<br>**E QUANDO** abrir o modal de Permissões para uma função (ex: Atendente, Jaimes) e configurar as permissões (Avaliações, Caixas, Clientes, Fichas, Relatórios)

<br>

<br>**ENTÃO** as permissões devem ser atualizadas.

<br>

<br>**E QUANDO** abrir o modal de visualização de uma função

<br>

<br>**ENTÃO** os dados detalhados da função devem ser exibidos corretamente.

 |

| **Critérios de aceitação** |
| --- |
| Criação, filtragem, parametrização de permissões e visualização de funções devem ser executadas sem inconsistências.

 |

---

## Caso de Teste 06: Gerenciamento de Pontuação, Ranking e Erros de Persistência

| ID | Descrição |
| --- | --- |
| RF19-CT06 | Verificar a criação de regras de pontuação, vincular atividades, consultar ranking, tratamento de erro ao editar e exclusão.

 |

| **Pré-condições** |
| --- |
| O usuário deve estar autenticado na tela de Pontuação.

 |

| **Passos** |
| --- |
| **DADO** que o usuário está na tela de Pontuação

<br>

<br>**QUANDO** pesquisar por nome ("Teste Dezembro") ou alternar o status ("Ativo" e "Inativo")

<br>

<br>**ENTÃO** os registros devem ser filtrados conforme a seleção.

<br>

<br>**E QUANDO** cadastrar uma nova pontuação ("Legpress", período de 09/10/2026 a 05/06/2027, produto: "Notebook Fitness")

<br>

<br>**ENTÃO** o registro deve ser salvo com sucesso (código #5).

<br>

<br>**E QUANDO** vincular a atividade "Postar todos os treinos" à pontuação e tentar visualizar o Ranking de Participantes

<br>

<br>**ENTÃO** a vinculação deve ser efetuada e a consulta ao ranking deve retornar o status correspondente (exibindo "Erro no servidor" ou "Nenhum participante encontrado").

<br>

<br>**E QUANDO** tentar editar o status de uma pontuação existente para "Inativo" e salvar

<br>

<br>**ENTÃO** o sistema deve tratar a falha exibindo a mensagem "Erro ao salvar pontuação".

<br>

<br>**E QUANDO** solicitar a exclusão de uma pontuação ("Legpress") e confirmar na caixa de diálogo

<br>

<br>**ENTÃO** a pontuação deve ser removida do sistema.

 |

| **Critérios de aceitação** |
| --- |
| A criação, alteração de atividades e exclusão devem funcionar; exceções e falhas na alteração de status/ranking devem ser devidamente reportadas por mensagens de erro amigáveis ao usuário.

 |

---

## Caso de Teste 07: Gerenciamento de Enquetes e Validação de Erros do Sistema

| ID | Descrição |
| --- | --- |
| RF19-CT07 | Verificar buscas, validação ao criar enquetes com opções, alteração de status e exclusão de enquetes com tratamento de exceções.

 |

| **Pré-condições** |
| --- |
| O usuário deve estar autenticado na tela de Enquetes.

 |

| **Passos** |
| --- |
| **DADO** que o usuário acessa a tela de Enquetes

<br>

<br>**QUANDO** filtrar por código (#4), por nome ("tase") ou por status ("Inativo")

<br>

<br>**ENTÃO** a listagem deve filtrar os dados (exibindo "Nenhuma enquete encontrada" se o filtro não retornar registros).

<br>

<br>**E QUANDO** tentar criar uma nova enquete (Nome: "Tass", Pergunta: "O que é tass", Resposta 1: "Tass é um exercício") e clicar em "Salvar"

<br>

<br>**ENTÃO** o sistema deve validar a requisição (exibindo "Erro ao salvar enquete" caso falhe).

<br>

<br>**E QUANDO** adicionar a Resposta 2 ("Tass é uma pessoa") e tentar salvar novamente

<br>

<br>**ENTÃO** a tentativa deve ser processada e o erro tratado se a falha de persistência mantiver-se.

<br>

<br>**E QUANDO** tentar alterar o status de uma enquete existente (#2 "tase") para "Inativo" e salvar

<br>

<br>**ENTÃO** o sistema deve capturar a falha e exibir modal "Erro ao salvar enquete".

<br>

<br>**E QUANDO** tentar deletar uma enquete (#1 "tase") e confirmar a ação

<br>

<br>**ENTÃO** o sistema deve processar a exclusão ou exibir o alerta "Erro ao deletar Enquete" em caso de falha no servidor.

 |

| **Critérios de aceitação** |
| --- |
| Os filtros de busca devem operar corretamente; as operações de cadastro, alteração e exclusão devem ser validadas e quaisquer erros de backend/banco de dados devem ser notificados em alertas visuais adequados.

 |

 https://jam.dev/c/0a093418-b086-4d01-8767-52162deece27

 https://jam.dev/c/70ba2354-8319-4221-85e6-071dc2bfcd57

 https://jam.dev/c/7665800f-fc1f-4d0f-90f1-d9c24924f244

 https://jam.dev/c/7dda0042-47b2-496a-b614-7b3bde126852

 https://jam.dev/c/6471ff44-b8aa-437b-b41d-436061366b55

 https://jam.dev/c/60180959-723d-492f-9092-32c01b65c20a

 https://jam.dev/c/379e33b4-4a28-400f-a51d-145934dea313

 https://jam.dev/c/06ce9a56-a25d-41bb-a0a3-fe15f41523fa
