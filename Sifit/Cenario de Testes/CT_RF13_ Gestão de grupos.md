Casos de Teste - Gestão de GruposSistema: SIFITMódulo: 
Treinamento > GruposArquivo de Referência: CT_RF13_ Gestão de grupos.md   
1. CT01 - Filtragem e Pesquisa de GruposObjetivo:
2. Validar o funcionamento dos filtros por Código, Nome, Status e Tipo de Caixa na listagem de grupos.
3. Pré-condições: Utilizador autenticado no sistema SIFIT e na página de "Grupos".
4. Passos de Execução:Digitar o código 1 no campo Código e filtrar.
5. Limpar o campo e digitar Treino no campo Nome do grupo.
6. Filtrar pelo nome completo Treino Personal.
7. Selecionar a opção Inativo no campo Status e clicar no botão de pesquisa.
8. Selecionar o tipo de caixa Externo no campo Tipo Caixa e clicar no botão de pesquisa.
9. Resultado Esperado:
10. A tabela deve atualizar exibindo apenas os registos correspondentes aos filtros aplicados e apresentar a mensagem "Nenhum grupo encontrado" quando não houver correspondências.
11. Resultado Obtido: Os filtros por Código, Nome, Status e Tipo de Caixa funcionaram corretamente conforme esperado.
12. Status: PASSOU
13.  2. CT02 - Edição e Atualização de Grupo ExistenteObjetivo:
     3. Verificar a alteração das configurações de status, exibição e tipo de caixa de um grupo cadastrado.
     4.    Passos de Execução:Na listagem de grupos, clicar no ícone de edição (lápis) do grupo Teste (Código 3).
     5.No modal "Editar Grupo", alterar o Status para Inativo e o Tipo Caixa para Interno.
       Clicar no botão "Salvar Grupo".
       Repetir a operação para o grupo Teste Novo (Código 5), alterando o Status para Inativo e clicando em "Salvar Grupo".
       Resultado Esperado: As alterações devem ser gravadas e refletidas no sistema.
       Resultado Obtido: Os grupos foram editados mas os dados não foram atualizados .
       Status: FALHOU
       3. CT03 - Inclusão de Novo Grupo com Status Inativo Objetivo:
       4. Validar o registo de um novo grupo com preenchimento dos campos obrigatórios e definindo status inativo.
       5. Passos de Execução:Clicar no botão "+" (Novo Grupo).   No modal "Novo Grupo", preencher o campo Nome com Teste 2.   Alterar o Status para Inativo e preencher a Descrição com teste 2.
       6. Clicar no botão "Salvar Grupo".
       7. Resultado Esperado: O novo grupo deve ser registado e exibido na listagem.
       8. Resultado Obtido: O grupo "Teste 2" foi criado com sucesso e adicionado à lista.
       9. Status: PASSOU
       4. CT04 - Tentativa de Exclusão de Grupo VinculadoObjetivo: Verificar a validação de integridade do sistema ao tentar eliminar um grupo que possui vínculos ativos.
       5. Passos de Execução:Na linha do grupo Teste, clicar no ícone de remoção (Lixeira).   No modal de confirmação ("Deseja deletar o Grupo?"), clicar em "Confirmar".
       6. Resultado Esperado: O sistema deve impedir a exclusão e apresentar uma mensagem de erro indicando a impossibilidade de remover o registo.   Resultado Obtido: O sistema exibiu a mensagem de alerta: "Erro ao deletar Grupo".
       7. Status: FALHOU
       8. Resumo da ExecuçãoTotal de Testes: 4   Passou: 2   Falhou: 2

       https://jam.dev/c/f449384d-fb57-4e6e-8acf-71fcfbb6a69d
