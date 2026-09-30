
CT_RF03_ Gestão de clientes.mdMódulo: Gestão de Clientes   
Funcionalidade: Atualização de cadastro, interação com perfil do aluno, agendamento de avaliação, consulta de métricas e filtros de busca.   
Cenário de Teste 1: Atualização de Dados Cadastrais do ClienteObjetivo: 
Validar o preenchimento e salvamento das informações de endereço, aplicativo e responsável do cliente.   Passos Executados:Acessar o formulário de edição/cadastro do cliente.   
Preencher os campos de endereço (bairro "bairro da Catarina" e complemento "Casa da Catarina").   
Informar o código do leitor biométrico ("123456").   
Configurar os dados de acesso ao aplicativo (e-mail "catarina@gmail.com" e senha).   
Preencher os dados do responsável e outros dados adicionais (telefone "(44) 99885-9666", profissão "Professor universitário", CPF, estado civil "Solteiro" e profissão secundária "Doceira").  
Resultado Esperado: Os dados devem ser salvos com sucesso no cadastro do cliente.   
Resultado Obtido: Sucesso no preenchimento das informações.   
Cenário de Teste 2: Ações no Perfil do Aluno e Agendamento de AvaliaçãoObjetivo: 
Verificar a navegação no perfil do aluno "Guilherma Morangona", abertura de mensagens, verificação de pagamentos e agendamento de avaliação.   
Passos Executados:Selecionar o aluno "Guilherma Morangona" na listagem para visualizar o perfil.   
Testar o botão "Enviar mensagem" (geração de modelo de mensagem via WhatsApp).   
Clicar em "Agendar avaliação", selecionando a personal responsável ("Gabriella"), a data (05/09/2026) e o horário (07:30).   
Verificar opções de "Registrar pagamento", "Histórico de presenças" e o painel "Inteligência Sifit".   
Resultado Esperado: O agendamento deve ser confirmado e as modais/painéis de suporte devem responder corretamente.  
Resultado Obtido: Sucesso no preenchimento do formulário de avaliação e na visualização das métricas do perfil.   
Cenário de Teste 3: Tentativa de Exclusão de ClienteObjetivo: 
Validar a funcionalidade de exclusão de registro de cliente diretamente pela listagem.   
Passos Executados:Localizar a cliente "Catarina Resende" na tabela de clientes.   
Clicar no ícone de exclusão/deletar registro.   Resultado Esperado: O sistema deve solicitar confirmação e remover o cliente do banco de dados.   
Resultado Obtido: Falha. O sistema retornou o modal de aviso: "Erro no servidor - Erro interno inesperado".  
Cenário de Teste 4: Pesquisa de Clientes com Filtros AvançadosObjetivo: Validar a consulta de clientes utilizando filtros por código de biometria e nome.   
Passos Executados:Acessar a tela de listagem de clientes.   Preencher o campo de código/biometria com "200306".   
Preencher o campo de nome com "Guilherma Morangona".   Clicar no botão "Buscar".   Resultado Esperado: O sistema deve filtrar e retornar apenas o registro correspondente aos parâmetros digitados.  
Resultado Obtido: Falha. Ao submeter a busca, o sistema exibiu um alerta de "Erro no servidor - Erro interno inesperado".  
Cenário de Teste 5: Validação de Mapeamento de Rotas (Navegação)Objetivo: Validar o redirecionamento de páginas no módulo de clientes.   
Passos Executados:Navegar entre os menus da aplicação.   
Resultado Esperado: Carregamento correto das visões do sistema.  
Resultado Obtido: Falha. A aplicação direcionou para a tela de erro 404 ("This Page Does Not Exist"). 

https://jam.dev/c/493528c5-fa47-42ad-835a-0f6499a5c6ea
https://jam.dev/c/2aa6309a-66ea-49fa-bfc8-368289cb5e89
https://jam.dev/c/00b55482-263c-4d73-a02b-6cc3d1de0fb1
