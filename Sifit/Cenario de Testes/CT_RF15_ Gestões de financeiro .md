# Casos de Teste - Gestão de Financeiro

**Sistema:** SIFIT

**Módulo:** Financeiro

**Arquivo de Referência:** `CT_RF15_ Gestões de financeiro.md`

---

## 1. CT01 - Cadastro e Gerenciamento de Despesas Fixas

- **Objetivo:** Validar o funcionamento da tela de Despesas Fixas, incluindo a consulta, aplicação de filtros e cadastro de uma nova despesa.

- **Pré-condições:** Utilizador autenticado no sistema SIFIT e com acesso ao módulo **Financeiro > Despesas Fixas**.

- **Passos de Execução:**

1. Acessar o menu **Financeiro > Despesas Fixas**.
2. Verificar a listagem das despesas cadastradas.
3. Utilizar os filtros disponíveis de **Código**, **Nome**, **Status** e **Recorrência**.
4. Clicar no botão **"Buscar"** para aplicar os filtros.
5. Clicar no botão de **Adicionar (+)** para cadastrar uma nova despesa.
6. No modal **"Nova Despesa"**, preencher o campo **Nome**.
7. Selecionar o **Status** como `Ativo`.
8. Informar o **Valor** da despesa.
9. Selecionar a opção de **Recorrência**.
10. Clicar em **"Salvar Despesa"**.

- **Resultado Esperado:** O sistema deve permitir a aplicação dos filtros e o cadastro da nova despesa, exibindo-a corretamente na listagem de Despesas Fixas após o salvamento.

- **Resultado Obtido:** A tela de Despesas Fixas permitiu realizar a pesquisa utilizando os filtros disponíveis e cadastrar uma nova despesa por meio do formulário apresentado.

- **Status:** **PASSOU**

---

## 2. CT02 - Consulta e Abertura de Caixa

- **Objetivo:** Verificar o funcionamento da tela de Caixas, incluindo filtros por período, consulta dos registros e abertura de um novo caixa.

- **Pré-condições:** Utilizador autenticado no sistema SIFIT e com acesso ao módulo **Financeiro > Caixas**.

- **Passos de Execução:**

1. Acessar o menu **Financeiro > Caixas**.
2. Informar a **Data Inicial** e a **Data Final** para o período de consulta.
3. Selecionar o **Status** desejado ou manter a opção `Todos`.
4. Clicar no botão **"Buscar"**.
5. Verificar os registros apresentados na tabela.
6. Conferir os indicadores de **Caixas Abertos**, **Caixas Fechados**, **Locais de Caixa** e **Registros no Período**.
7. Clicar no botão **"Abrir Caixa"**.
8. Verificar a criação do novo registro de caixa.

- **Resultado Esperado:** O sistema deve retornar os caixas correspondentes ao período e status selecionados e permitir a abertura de um novo caixa, apresentando o registro com status **Aberto**.

- **Resultado Obtido:** A consulta dos caixas foi realizada corretamente pelos filtros de período e status, sendo possível visualizar os caixas abertos e fechados e utilizar a opção de abertura de caixa.

- **Status:** **PASSOU**

---

## 3. CT03 - Consulta Financeira no Pagar.me

- **Objetivo:** Validar a visualização das informações financeiras disponibilizadas pelo módulo Pagar.me, incluindo recebimentos, meios de pagamento e ações financeiras.

- **Pré-condições:** Utilizador autenticado no sistema SIFIT e com acesso ao módulo **Financeiro > Pagar.me**.

- **Passos de Execução:**

1. Acessar o menu **Financeiro > Pagar.me**.
2. Verificar os indicadores de **Disponível para saque**, **Em processamento**, **Recebíveis futuros** e **Recebido no mês**.
3. Consultar o gráfico de **Recebimentos**.
4. Alterar o período de consulta, quando necessário.
5. Verificar o gráfico de **Meios de pagamento**.
6. Conferir as opções disponíveis em **Ações rápidas**.
7. Verificar as opções **Solicitar saque**, **Ver extrato completo**, **Nova cobrança** e **Configurações**.

- **Resultado Esperado:** O sistema deve apresentar corretamente os indicadores financeiros, os recebimentos registrados, a distribuição dos meios de pagamento e disponibilizar as ações financeiras configuradas para o usuário.

- **Resultado Obtido:** O módulo Pagar.me apresentou os indicadores de recebimentos, gráfico de evolução financeira, distribuição por meios de pagamento e as opções de ações rápidas.

- **Status:** **PASSOU**

---

## 4. CT04 - Geração de Relatório Financeiro

- **Objetivo:** Verificar a geração de relatórios relacionados à movimentação financeira do sistema.

- **Pré-condições:** Utilizador autenticado no sistema SIFIT e com acesso ao módulo **Financeiro > Relatórios**.

- **Passos de Execução:**

1. Acessar o menu **Financeiro > Relatórios**.
2. Verificar os tipos de relatórios disponíveis.
3. Selecionar o relatório **Contas a Receber**.
4. Informar o período desejado por meio dos campos **Data Inicial** e **Data Final**.
5. Verificar os filtros disponibilizados para o relatório selecionado.
6. Clicar no botão **"Gerar Relatório"**.
7. Repetir o procedimento selecionando o relatório **Contas a Pagar**.
8. Selecionar o relatório **Caixas**.
9. Definir o formato do relatório como **Detalhado**.
10. Informar o período desejado.
11. Clicar em **"Gerar Relatório"**.

- **Resultado Esperado:** O sistema deve permitir selecionar diferentes tipos de relatórios financeiros, aplicar os filtros correspondentes ao relatório escolhido e gerar o documento com os dados referentes ao período informado.

- **Resultado Obtido:** Os relatórios financeiros foram disponibilizados para seleção, permitindo consultar informações de **Contas a Receber**, **Contas a Pagar** e **Caixas**, inclusive com opção de relatório detalhado para movimentações de caixa.

- **Status:** **PASSOU**

---

## Resumo da Execução

- **Total de Testes:** 4
- **Passou:** 4
- **Falhou:** 0
https://jam.dev/c/504c40b9-a1f4-4b1a-87b9-ac134afdf171
https://jam.dev/c/24e36cb0-b257-48ba-ab07-77578f65ef26
https://jam.dev/c/60a97112-4d54-4458-98dd-bbf6c2031909
https://jam.dev/c/448e633b-4073-4b50-a158-20ec1dcc75b5
