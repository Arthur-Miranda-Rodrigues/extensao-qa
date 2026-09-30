# Casos de Teste - Gestão de Turmas

**Sistema:** SIFIT

**Módulo:** Treinamento > Turmas

**Arquivo de Referência:** `CT_RF15_ Gestão de turmas.md`

---

## 1. CT01 - Filtragem e Pesquisa de Turmas

* **Objetivo:** Validar o funcionamento dos filtros por Código, Nome da Turma e Status na listagem de turmas.
* **Pré-condições:** Utilizador autenticado no sistema SIFIT e na página de "Turmas".
* **Passos de Execução:**
1. Digitar o código `1` no campo **Código** e clicar em **"Buscar"**.
2. Limpar o campo de código, digitar `teste` no campo **Nome da Turma** e clicar em **"Buscar"**.
3. Limpar o campo de nome, selecionar a opção **Inativo** no campo **Status** e clicar no botão **"Buscar"**.


* **Resultado Esperado:** A tabela deve atualizar exibindo apenas as turmas correspondentes aos filtros aplicados e apresentar a mensagem "Nenhuma turma encontrada" quando não houver registos que atendam aos critérios de pesquisa.
* **Resultado Obtido:** Os filtros por Código, Nome da Turma e Status funcionaram corretamente conforme esperado.
* **Status:** **PASSOU**

---

## 2. CT02 - Edição e Atualização de Turma Existente

* **Objetivo:** Verificar a alteração de configurações e status de uma turma já cadastrada.
* **Passos de Execução:**
1. Na listagem de turmas, localizar a turma **Horário da** (Código 8) e clicar no ícone de edição (Lápis).
2. No modal "Editar Turma", alterar o **Status** para `Inativo`.
3. Clicar no botão **"Salvar"**.
4. Filtrar pelo status **Inativo** para confirmar a alteração na listagem.


* **Resultado Esperado:** As alterações da turma devem ser gravadas com sucesso e o status atualizado na listagem.
* **Resultado Obtido:** A turma teve o status alterado para Inativo e os dados foram atualizados com sucesso.
* **Status:** **PASSOU**

---

## 3. CT03 - Inclusão de Nova Turma

* **Objetivo:** Validar o registo de uma nova turma com preenchimento completo dos campos obrigatórios e horários.
* **Passos de Execução:**
1. Clicar no botão **"Cadastrar Turma"**.
2. No modal "Cadastrar Turma", preencher o campo **Nome** com `Turma dos Bodybuilders`.
3. Selecionar o **Plano** `AVA`, marcar **Aula Experimental** como `Sim`, definir o **Tempo (meses)** como `16` e **Tem Personal** como `Sim`.
4. Selecionar a personal `Marília Rhana Souza` e marcar os dias da semana (`Seg`, `Ter`, `Qua`, `Qui`, `Sex`, `Sáb`).
5. Clicar no botão **"Salvar"**.


* **Resultado Esperado:** A nova turma deve ser registada com sucesso e disponibilizada na listagem geral de turmas.
* **Resultado Obtido:** A turma "Turma dos Bodybuilders" foi cadastrada com sucesso.
* **Status:** **PASSOU**

---

## 4. CT04 - Exclusão de Turma

* **Objetivo:** Verificar a funcionalidade de remoção de uma turma inativa do sistema.
* **Passos de Execução:**
1. Filtrar pelo status **Inativo** para exibir a turma **Horário da** (Código 8).
2. Clicar no ícone de exclusão (Lixeira) na linha correspondente à turma.
3. No modal de confirmação (*"Deseja deletar esta turma?"*), clicar em **"Confirmar"**.


* **Resultado Esperado:** O sistema deve remover a turma e atualizar a listagem confirmando a exclusão.
* **Resultado Obtido:** A turma foi eliminada com sucesso e deixou de ser exibida na listagem.
* **Status:** **PASSOU**

---

## Resumo da Execução

* **Total de Testes:** 4
* **Passou:** 4
* **Falhou:** 0

https://jam.dev/c/580df45f-52e6-43c2-94f8-783cc8027bbd 

