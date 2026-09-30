# Casos de Teste - Módulo Dashboard

* **Sistema:** SIFIT
* **Módulo:** Visão Geral > Dashboard
* **Ficheiro de Cenário:** `CT_RF03_Acesso e Visualização do Dashboard.md`

---

### 1. C02-CT01 - Acesso à Tela de Dashboard

* **Objetivo:** Verificar a navegação e a exibição correta da tela de Dashboard através do menu lateral do SIFIT.
* **Pré-condições:** Usuário autenticado no sistema.
* **Passos de Execução:**
1. No menu lateral principal, localizar o grupo de navegação.
2. Clicar na opção **Dashboard**.


* **Resultado Esperado:** A página de Dashboard deve ser carregada corretamente, exibindo os gráficos, relatórios e o painel de Inteligência Sifit.
* **Resultado Obtido:** Página de Dashboard carregada com sucesso, apresentando todos os cards e gráficos do painel geral.
* **Status:** PASSOU

---

### 2. C02-CT02 - Navegação e Interação com a Inteligência Sifit

* **Objetivo:** Verificar o acesso à tela "Resultados da Inteligência" através do botão "Ver Inteligência" e a filtragem por período.
* **Pré-condições:** Usuário posicionado na tela de Dashboard.
* **Passos de Execução:**
1. No card de Inteligência Sifit, clicar no botão **Ver Inteligência**.
2. Na tela de resultados, selecionar os filtros de período (ex: "Últimos 7 dias", "Últimos 30 dias").


* **Resultado Esperado:** O painel "Resultados da Inteligência" deve ser carregado e os dados de automações executadas, relatórios enviados, alunos em risco e demais métricas devem atualizar conforme o período selecionado.
* **Resultado Obtido:** Redirecionamento efetuado e métricas atualizadas dinamicamente de acordo com a alternância dos filtros temporais.
* **Status:** PASSOU

---

### 3. C02-CT03 - Interação com os Gráficos Interativos do Dashboard

* **Objetivo:** Verificar se os elementos gráficos do Dashboard respondem à passagem do cursor (*hover*) mostrando os detalhes das métricas.
* **Pré-condições:** Usuário posicionado na tela de Dashboard.
* **Passos de Execução:**
1. Passar o cursor sobre as barras dos gráficos de clientes.
2. Passar o cursor sobre as seções do gráfico de rosca de pagamentos.
3. Passar o cursor sobre os elementos do gráfico de modalidades.


* **Resultado Esperado:** O sistema deve exibir os balões de informação (*tooltips*) detalhando os valores e categorias correspondentes a cada seção consultada.
* **Resultado Obtido:** Todos os gráficos interativos apresentaram os *tooltips* informativos com os valores exatos ao posicionar o mouse sobre os elementos.
* **Status:** PASSOU

---

## Resumo da Execução

* **Total de Testes:** 3
* **Passou:** 3
* **Falhou:** 0

https://jam.dev/c/5c1713ea-159f-4087-9e02-38767a30c1e6 
