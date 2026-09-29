
Casos de Teste - Gerenciamento de Exercícios 
Sistema: SIFIT

Módulo: Treinamento > Exercícios

1. CT01 - Visualização e Edição de Exercício Existente
Objetivo: Verificar a abertura do modal de edição de um exercício cadastrado num grupo muscular.

Pré-condições: Utilizador autenticado e na tela "Biblioteca de Exercícios".

Passos de Execução:

No grupo muscular Bíceps, localizar o exercício AA.

Clicar no ícone de pesquisa/visualização (lupa) do exercício.

No modal "Exercício", carregar uma imagem para o exercício.

Clicar no botão "Salvar".

Resultado Esperado: As alterações do exercício devem ser salvas com sucesso.

Resultado Obtido: O modal salvou a inclusão da imagem e retornou à lista da biblioteca.

Status: PASSOU

2. CT02 - Cadastro de Novo Exercício num Grupo Muscular
Objetivo: Validar a criação e associação de um novo exercício a um grupo muscular específico.

Passos de Execução:

No card do grupo muscular Bíceps, clicar no botão "+ Adicionar".

No modal "Exercício", preencher o campo Nome (ex: "Quarken").

Anexar uma imagem e/ou vídeo demonstrativo.

Clicar no botão "Salvar".

Resultado Esperado: O novo exercício deve ser cadastrado e exibido no card do grupo muscular correspondente, atualizando o contador total.

Resultado Obtido: O exercício "Quarken" foi adicionado ao grupo Bíceps e o contador total da biblioteca passou de 5 para 6 (e posteriormente para 7 com novos testes).

Status: PASSOU

3. CT03 - Exclusão/Deleção de Exercício de um Grupo Muscular
Objetivo: Verificar se o sistema permite remover um exercício de um grupo muscular.

Passos de Execução:

No grupo muscular Bíceps, localizar o exercício desejado (ex: "Quarken" ou "AA").

Clicar no ícone de exclusão (X em vermelho) ao lado do exercício.

No modal de confirmação ("Deseja deletar o exercício?"), clicar em "Confirmar".

Resultado Esperado: O exercício deve ser removido do grupo muscular e o totalizador da biblioteca deve ser decrementado.

Resultado Obtido: O exercício foi removido da lista e o contador total de exercícios foi atualizado corretamente.

Status: PASSOU

4. CT04 - Validação de Campo Obrigatório no Cadastro de Exercício
Objetivo: Validar a regra de negócio que impede o cadastro de um exercício sem preencher o nome.

Passos de Execução:

Clicar em "+ Adicionar" num grupo muscular (ex: Teste).

No modal "Exercício", anexar uma imagem sem preencher o campo Nome.

Clicar no botão "Salvar".

Resultado Esperado: O sistema deve bloquear a gravação e exibir uma mensagem de aviso solicitando o preenchimento do campo obrigatório.

Resultado Obtido: O sistema exibiu a mensagem de aviso: "Informe o nome do exercício.".

Status: PASSOU

Resumo da Execução
Total de Testes: 4

Passou: 4

Falhou: 0

https://jam.dev/c/a6ce9380-799e-4fb0-8438-1b430601706d
