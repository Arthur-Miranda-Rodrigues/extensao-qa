Cenário 02: Acesso e visualização do Dashboard   

Caso de Teste 01: Acesso à tela de DashboardCampoDetalhesIDC02-CT01 

DescriçãoVerificar a navegação e a exibição correta da tela de Dashboard através do menu lateral do SIFIT.
Pré-condiçõesO usuário deve estar autenticado no sistema.   

PassosDADO que o usuário está autenticado no sistemaQUANDO clicar na opção "Dashboard" do menu lateral principal 
ENTÃO a página de Dashboard deve ser carregada exibindo os gráficos, relatórios e o painel de Inteligência Sifit   

Critérios de aceitaçãoA tela de Dashboard deve ser exibida corretamente ao ser selecionada no menu.   
Caso de Teste 02: Navegação e interação com a Inteligência SifitCampoDetalhesIDC02-CT02   

DescriçãoVerificar o acesso à tela "Resultados da Inteligência" através do botão "Ver Inteligência" e a filtragem por período.   
Pré-condiçõesO usuário deve estar visualizando a tela de Dashboard.   

PassosDADO que o usuário está no DashboardQUANDO clicar no botão "Ver Inteligência" no card de Inteligência SifitE selecionar os filtros de período (ex: "Últimos 7 dias", "Últimos 30 dias") 

ENTÃO os dados de automações executadas, relatórios enviados, alunos em risco e demais métricas devem atualizar conforme o período selecionado   
Critérios de aceitaçãoO painel "Resultados da Inteligência" deve carregar e permitir a alternância de filtros temporal de forma funcional.

Caso de Teste 03: Interação com os gráficos interativos do DashboardCampoDetalhesIDC02-CT03   
DescriçãoVerificar se os elementos gráficos do Dashboard respondem à passagem do cursor (hover) mostrando os detalhes das métricas.  

Pré-condiçõesO usuário deve estar na tela de Dashboard.   PassosDADO que o usuário está visualizando a tela de DashboardQUANDO passar o cursor sobre as barras dos gráficos de clientes, gráfico de rosca de pagamentos ou modalidades ENTÃO o sistema deve exibir os balões de informação (tooltips) com os valores e categorias correspondentes   

Critérios de aceitaçãoTodos os gráficos interativos devem exibir os valores de cada seção ao passar o mouse sobre eles.   

https://jam.dev/c/5c1713ea-159f-4087-9e02-38767a30c1e6 
