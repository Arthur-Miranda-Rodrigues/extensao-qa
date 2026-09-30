

# Casos de Teste - Módulo Categorias Crossfit

* **Sistema:** SIFIT


* **Módulo:** Treinamento > Categorias Crossfit


* **Ficheiro de Cenário:** `CT_RF16_Gestão de Categorias Crossfit.md`


---

### 1. CT01 - Cadastramento de Nova Categoria de Crossfit

* **Objetivo:** Validar a criação e inclusão de uma nova categoria de Crossfit no sistema.


* **Pré-condições:** Utilizador autenticado e situado no menu **Categorias Crossfit**.


* **Passos de Execução:**
1. Clicar no botão **+ Nova Categoria**.


2. No modal *Cadastrar Categoria*, preencher o campo **Nome** com `BodyBuilder`.


3. Clicar no botão **Salvar**.




* **Resultado Esperado:** A nova categoria deve ser cadastrada com sucesso e exibida na listagem com o seu respetivo código, data de criação e atualização.


* **Resultado Obtido:** A categoria "BodyBuilder" foi inserida com o código `#4`, registando as datas de criação e atualização corretamente (`30/09/2026`).


* **Status:** PASSOU

---

### 2. CT02 - Edição de Categoria de Crossfit

* **Objetivo:** Verificar se o sistema permite alterar o nome de uma categoria já existente.


* **Passos de Execução:**
1. Na listagem de **Categorias Crossfit**, localizar a categoria recém-criada (`BodyBuilder`).


2. Clicar no ícone de edição (lápis) na coluna **Ações**.


3. No modal *Editar Categoria*, alterar o campo **Nome** de `BodyBuilder` para `BodyBuilder supremo`.


4. Clicar no botão **Salvar**.




* **Resultado Esperado:** O registo deve ser atualizado na base de dados e a tabela deve refletir o novo nome imediatamente.


* **Resultado Obtido:** O nome da categoria foi alterado para "BodyBuilder supremo" com sucesso.


* **Status:** PASSOU

---

### 3. CT03 - Filtragem/Pesquisa de Categorias por Código e Nome

* **Objetivo:** Testar o funcionamento dos campos de busca por Código e Nome da Categoria.


* **Passos de Execução:**
1. No campo **Código**, digitar `2` e verificar a filtragem.


2. Limpar o campo e, no campo **Nome**, digitar `E`.


3. Clicar no botão **Buscar** ou aguardar o recarregamento.




* **Resultado Esperado:** A tabela deve filtrar os registos e atualizar o indicador de "Exibidas".


* **Resultado Obtido:** O sistema efetuou a filtragem dinâmica exibindo a categoria correspondente e ajustando o card de contagem "Exibidas" para `2`.


* **Status:** PASSOU

---

### 4. CT04 - Exclusão de Categoria de Crossfit (Identificação de Erro)

* **Objetivo:** Verificar a funcionalidade de remoção de uma categoria cadastrada.


* **Passos de Execução:**
1. Na linha da categoria `BodyBuilder supremo`, clicar no ícone de exclusão (lixeira).


2. No modal de confirmação (*"Deseja deletar esta categoria?"*), clicar no botão **Confirmar**.




* **Resultado Esperado:** A categoria deve ser eliminada do sistema, emitindo uma mensagem de sucesso e removendo o item da tabela.


* **Resultado Obtido (FALHA):** O sistema apresentou um modal de erro com a mensagem **"Erro ao deletar categoria."** e o registo não foi excluído.


* **Status:** FALHOU

---

## Relatório de Erros / Bugs Encontrados

1. **BUG-01: Erro ao apagar categoria recém-criada**

* **Módulo:** Categorias Crossfit


* **Descrição:** Ao tentar excluir uma categoria criada/editada na própria sessão (`BodyBuilder supremo`), o sistema exibe o modal *"Erro: Erro ao deletar categoria."* e impede a eliminação do registo.


* **Severidade:** Alta / Média (Impede a gestão completa do ciclo de vida do registo CRUD).





---

## Resumo da Execução

* **Total de Testes:** 4


* **Passou:** 3


* **Falhou:** 1

https://jam.dev/c/7cadafc7-b6df-4e3a-9619-7d4f8a5d5082
