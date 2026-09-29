Casos de Teste - Gestão de Grupos MuscularesSistema: 
SIFITMódulo: Treinamento > Grupos MuscularesArquivo de Referência: CT_RF11_ Gestão de grupos musculares.md   
1. CT01 - Filtragem e Busca de Grupos MuscularesObjetivo:
2. Verificar o funcionamento dos filtros por Código, Nome e Tipo de Membro na listagem de Grupos Musculares.
3. Pré-condições: Utilizador autenticado no sistema SIFIT e na página "Grupos Musculares".
4. Passos de Execução:Digitar o código 2 no campo Código e clicar em "Buscar".
5. Limpar o campo Código.   Digitar Biceps no campo Nome e clicar em "Buscar".
6. Limpar o campo Nome.
7. Selecionar Inferiores no dropdown Tipo Membro e clicar em "Buscar".
8. Alterar o filtro para Superiores e clicar em "Buscar".
9. Alterar o filtro para Aerobio e clicar em "Buscar".
10. Resultado Esperado: A tabela deve filtrar os registros exibidos corretamente de acordo com os critérios informados.
11.    Resultado Obtido: A busca funcionou corretamente para todos os campos e filtros de membros testados.
12.Status: PASSOU
   2. CT02 - Edição de Grupo Muscular Existente com Inclusão de ImagemObjetivo: Validar a alteração e atualização de imagem de um grupo muscular cadastrado.
   3.    Passos de Execução:Na listagem de grupos musculares, localizar o registro Bíceps (Código 1).
   4.Clicar no ícone de edição (lupa) na coluna Ações.
     No modal "Grupo Muscular", clicar em "Escolher ficheiro" e selecionar uma imagem (imagem.png).
     Clicar no botão "Salvar".   Resultado Esperado: O registro do grupo muscular deve ser atualizado e salvo com sucesso.
     Resultado Obtido: O modal salvou a imagem anexada e retornou para a listagem principal.
     Status: PASSOU
     3. CT03 - Tentativa de Exclusão de Grupo Muscular VinculadoObjetivo:
     Verificar se o sistema trata e impede a exclusão de um grupo muscular que possui vínculo ou restrição no sistema.
        Passos de Execução:Na tabela de Grupos Musculares, clicar no ícone de exclusão (lixeira) de um registro existente.
     No modal de confirmação ("Deseja deletar o Grupo?"), clicar no botão "Confirmar".
     Resultado Esperado:
     O sistema deve tratar a requisição e exibir uma mensagem de erro adequada caso o registro não possa ser removido.
        Resultado Obtido: O sistema exibiu um modal de alerta com a mensagem de erro: "Erro ao deletar Grupo".
     Status: Falhou
     4. CT04 - Cadastro de Novo Grupo MuscularObjetivo: Validar o cadastro de um novo grupo muscular preenchendo Nome, Tipo de Membro e anexando imagem.
        Passos de Execução:Na tela "Grupos Musculares", clicar no botão de cadastro ("+") no canto superior direito.
     No modal "Grupo Muscular", preencher o campo Nome com Peitoral.   Selecionar o Tipo Membro como Superiores.
      Anexar um arquivo de imagem.
     Clicar no botão "Salvar".
     Resultado Esperado: O novo grupo muscular deve ser cadastrado e os cards superiores de contadores de registros devem ser atualizados.
     Resultado Obtido: O grupo Peitoral foi inserido com sucesso (Código 12). O número de "Grupos cadastrados" subiu de 10 para 11, e o contador de membros "Superiores" subiu de 6 para 7.
     Status: PASSOU
     Resumo da ExecuçãoTotal de Testes:
      Passou: 3   Falhou: 1   

https://jam.dev/c/a8f20df5-1340-4a00-a04c-b8894dd1a2a0
