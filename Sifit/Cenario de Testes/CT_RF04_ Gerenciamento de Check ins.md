CT_RF04_Gerenciamento de Check ins
Descrição do Cenário
Validação do módulo de gerenciamento de check-ins, englobando a navegação entre unidades, realização de entrada manual de alunos, tratamento de exceções no check-in por código/biometria e navegação entre abas de status.

Casos de Teste
Caso de Teste 1: Seleção e Troca de Unidade Operacional
Objetivo: Verificar a alternância de dados e métricas ao selecionar diferentes unidades no cabeçalho superior.

Pré-condições: Usuário autenticado na plataforma com acesso a múltiplas unidades.

Passos:

Acessar o menu lateral Check-in.

Clicar no seletor de unidade localizado no topo da tela (ex: "Unidade Centro").

Selecionar outra unidade disponível (ex: "Unidade Sul" ou "Unidade Norte").

Resultado Esperado: Os dados de métricas (Check-ins hoje, Presentes agora, Meta do dia, Média diária) e a listagem de clientes devem atualizar de acordo com a unidade selecionada.

Caso de Teste 2: Registro de Entrada Manual de Cliente
Objetivo: Confirmar o registro manual de presença para alunos através da busca por nome, código ou CPF.

Pré-condições: Cliente cadastrado e ativo no sistema.

Passos:

Na tela de Check-ins, clicar no botão + Check-in manual.

No modal "Entrada manual", selecionar a aba Cliente existente.

Digitar o nome, CPF ou código do cliente no campo de busca (ex: "Rodolfo").

Confirmar os dados exibidos no resultado do cliente encontrado.

Clicar em Registrar entrada.

Resultado Esperado: O registro é processado com sucesso e o cliente passa a ser listado na tabela de check-ins da página principal com status "Pendente" ou "Ativo".

Caso de Teste 3: Entrada Rápida com Código Invalido / Não Encontrado
Objetivo: Validar a mensagem de erro ao tentar realizar o check-in rápido utilizando um código ou biometria não associado à empresa/unidade.

Pré-condições: Estar na tela inicial de Check-ins.

Passos:

Localizar o painel lateral de Entrada rápida.

Inserir no campo "Código do cliente" um número de biometria/identificador cadastrado em outra unidade ou inexistente (ex: 123456).

Clicar no botão Realizar check-in.

Resultado Esperado: O sistema deve exibir um modal de alerta com a mensagem: "Não foi possível concluir - Cliente não encontrado para esta empresa."

Caso de Teste 4: Filtro por Abas de Status de Presença
Objetivo: Validar a filtragem dos registros através das abas de navegação da listagem principal.

Pré-condições: Existirem registros com diferentes estados de presença no dia.

Passos:

Na tela de Check-ins, navegar entre as abas:

Todos

Presentes agora

Não compareceram

Check-in pendente

Resultado Esperado: A tabela de resultados deve recarregar e exibir exclusivamente os registros correspondentes ao filtro/aba selecionado.

https://jam.dev/c/014ff3c9-66c7-4a8d-9d1d-488ef529f977 
