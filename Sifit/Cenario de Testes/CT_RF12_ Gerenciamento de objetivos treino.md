Casos de Teste - Gerenciamento de Objetivos de TreinoSistema: 
SIFITMódulo: Treinamento > ObjetivosArquivo de Referência: 
CT_RF12_ Gerenciamento de objetivos treino.md   
1. CT01 - Filtragem e Busca de Objetivos de TreinoObjetivo: Verificar o funcionamento dos filtros por Código e Nome na listagem de Objetivos de Treino.
2.   Pré-condições: Utilizador autenticado no sistema SIFIT e na página "Objetivos Treino".
3.   Passos de Execução:Digitar o código 1 no campo Código e clicar em "Buscar".
4.   Limpar o campo Código.   Digitar crescer no campo Nome e clicar em "Buscar".
5.   Clicar novamente no botão "Buscar" para recarregar a lista completa.
6.   Resultado Esperado: A tabela deve filtrar e exibir corretamente os registros correspondentes aos parâmetros informados.
7.   Resultado Obtido:
8.   A busca filtrou corretamente o registro do objetivo "Crescer" pelos campos de Código e Nome.
9.   Status: PASSOU   
10. CT02 - Tentativa de Cadastro de Objetivo Sem Código de IdentificaçãoObjetivo:
11. Verificar a validação de erro ao tentar salvar um novo objetivo sem preenchimento correto ou atribuição do código no sistema.
12.    Passos de Execução:Clicar no botão "+ Novo Objetivo".
13.No modal "Objetivo", preencher o campo Nome com Emagrecer e deixar os demais campos conforme padrão.
     Clicar no botão "Salvar".
   Resultado Esperado: O sistema deve tratar a inclusão e exibir uma mensagem de erro caso o cadastro não possa ser finalizado.
     Resultado Obtido: O sistema exibiu um modal de alerta com a mensagem: "Erro ao salvar objetivo".
   Status: FALHOU
   3. CT03 - Edição e Atualização de Descrição do ObjetivoObjetivo: Validar a alteração e atualização dos dados de um objetivo cadastrado.
   4.  Passos de Execução:Localizar o objetivo Crescer (Código 1) na listagem.
   5.  Clicar no ícone de visualização/edição (lupa) na coluna de ações.
   6.  No modal "Objetivo", preencher o campo Descrição com Crescer Músculos.
   7.   Clicar no botão "Salvar".
   8.   Resultado Esperado: O objetivo deve ser atualizado com a nova descrição informada.
   9.   Resultado Obtido: O modal não salva a descrição.
   10.   Status: FALHOU 
   11.   4. CT04 - Tentativa de Exclusão de Objetivo VinculadoObjetivo:
         5. Verificar a regra de integridade que impede a remoção de um objetivo de treino em uso ou vinculado.
         6. Passos de Execução:Na linha do objetivo Crescer, clicar no ícone de exclusão (X).
         7. No modal de confirmação ("Deseja deletar o Objetivo?"), clicar no botão "Confirmar".
         8. Resultado Esperado: O sistema deve tratar a tentativa de exclusão e exibir uma mensagem de erro adequada.
         9. Resultado Obtido:
         10. O sistema exibiu o modal de aviso com a mensagem: "Erro ao deletar Objetivo".
         11. Status: FALHOU
         12. Resumo da ExecuçãoTotal de Testes: 4
         13. Passou: 1   Falhou: 3

         https://jam.dev/c/47aadfe2-569d-413e-a2a4-0d5a7f5f1cff
