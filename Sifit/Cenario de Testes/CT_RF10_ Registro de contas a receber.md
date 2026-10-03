CT_RF07 - Registro e Gestão de Contas a Receber
1. Descrição
Este documento especifica os cenários de teste referentes ao Requisito Funcional 07 (RF07) - Registro e Gestão de Contas a Receber . O objetivo é validar o fluxo de pesquisa, criação de novos recebimentos, edição de lançamentos pendentes, validação de campos obrigatórios, eliminação de contas e filtragem por datas/status no sistema SIFIT .

2. Cenários de Teste
CT01 - Filtro e Pesquisa por Código/Cliente
Descrição: Validar o funcionamento do filtro de pesquisa na listagem de Contas a Receber 

Pré-condições: Estar autenticado no sistema e aceder à página "Contas a Receber" 

Passos:

Informar o código do registo (ex.: 1590) no campo Código 

Clicar no botão Buscar [source: 15].

Resultado Esperado: A tabela deve filtrar e exibir apenas os registos correspondentes ao código inserido 

CT02 - Tentativa de Cadastro sem Seleção de Cliente (Validação de OBRIGATORIEDADE)
Descrição: Validar se o sistema impede a criação de uma nova conta a receber caso nenhum cliente seja selecionado 

Pré-condições: Aceder à modal "Cadastrar Conta a Receber" clicando em + Nova Conta 

Passos:

Deixar o campo de pesquisa de Cliente em branco 

Preencher o Título (ex.: Leo) 

Definir Criar Cópias como Sim 

Inserir o Valor a Receber (ex.: 200,00) 

Preencher os Dados do Recebimento (Local: Caixa Academia, Observação: Teste 1) 

Clicar no botão Salvar 

Resultado Esperado: O sistema exibe um alerta de atenção com a mensagem "Selecione o cliente.", impedindo a conclusão do cadastro até que o cliente seja fornecido 

CT03 - Eliminação de Conta a Receber
Descrição: Validar a exclusão de um lançamento na listagem de Contas a Receber 

Pré-condições: Ter um registo existente na lista de recebimentos 

Passos:

Localizar o registo desejado (ex.: código 1590) e clicar no ícone de Lixeira na coluna de ações 

Na modal de confirmação ("Deseja deletar esta conta?"), clicar no botão Confirmar 

Resultado Esperado: A conta é eliminada e removida da grelha de lançamentos 

CT04 - Edição e Atualização de Lançamento Pendente
Descrição: Validar a alteração de dados de uma conta com status "PENDENTE" 

Pré-condições: Existir uma conta pendente cadastrada 

Passos:

Localizar um registo com status PENDENTE (ex.: 1583 - Marcelo Longo Zandonadi) e clicar no ícone de edição/visualização

Clicar na opção de editar recebimento 

Alterar o Tipo de Pagamento para Cartão de Débito 

Alterar o Local de Recebimento para Caixa Muay Thai

Clicar em Salvar e, caso surja o alerta de caixa não aberto no dia, clicar em Confirmar 

Resultado Esperado: Os dados do recebimento são atualizados com sucesso e refletidos no resumo financeiro 

CT05 - Aplicação de Filtros Rápidos por Período e Status
Descrição: Verificar a atualização dos relatórios card/cards financeiros e listagens ao alterar os filtros de período e status 

Pré-condições: Ter registos em variadas datas e status 

Passos:

Clicar nos botões de atalho: Hoje, Ontem, Últimos 7 dias e Este mês 

Ajustar os filtros de Data Inicial e Data Final no cabeçalho 

Alterar o filtro Status (ex.: alternar entre Todos, Pendente e Recebido) e clicar em Buscar 

https://jam.dev/c/aae899c5-f4dc-44b7-a506-01ac1f829a9a

Resultado Esperado: Os valores dos cards informativos (Entradas, Saídas, Líquido, Previsto para o mês, Recebido no mês) e a lista abaixo atualizam corretamente de acordo com os critérios definidos [source: 15].
