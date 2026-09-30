


# Casos de Teste - Módulo Gestão de Box (Turmas e Modalidades)

* **Sistema:** SIFIT


* **Módulo:** Treinamento > Box - Turmas


* **Ficheiro de Cenário:** `CT_RF17_Gestão de Box - Turmas.md`


---

### 1. CT01 - Cadastramento de Nova Modalidade

* **Objetivo:** Validar o cadastro de uma nova modalidade de treino no Box.


* **Pré-condições:** Utilizador autenticado no SIFIT e posicionado no menu **Box - Turmas**.


* **Passos de Execução:**
1. No painel superior (*Modalidades*), preencher o campo **Nome da modalidade** com `Leo`.


2. Preencher o campo **Descrição** com `Leo`.


3. Clicar no botão **+ Modalidade** no canto superior direito.




* **Resultado Esperado:** A nova modalidade deve ser cadastrada com status "Ativo" e exibida na tabela de modalidades.


* **Resultado Obtido:** A modalidade "Leo" foi cadastrada com sucesso e exibida na listagem como "Ativo".


* **Status:** PASSOU

---

### 2. CT02 - Cadastramento de Nova Turma Recorrente

* **Objetivo:** Verificar o cadastro de uma turma vinculada a uma modalidade existente.


* **Passos de Execução:**
1. No painel *Turmas recorrentes*, preencher o **Nome da turma** com `Leo`.


2. Selecionar a **Modalidade** `Leo`.


3. Marcar os dias da semana desejados (ex: Seg, Qua, Qui, Sex).


4. Definir a quantidade de **Vagas** como `20`.


5. Configurar o horário (Início: `20:09` / Fim: `20:30`).


6. Clicar no botão **+ Turma**.




* **Resultado Esperado:** A turma recorrente deve ser criada e listada na tabela inferior com as informações de horário, dias e vagas ativas.


* **Resultado Obtido:** A turma foi criada com sucesso exibindo o horário `20:00:00 - 20:30:00` e 20 vagas.


* **Status:** PASSOU

---

### 3. CT03 - Edição de Modalidade (Status e Nome)

* **Objetivo:** Testar a alteração dos dados e do status de uma modalidade.


* **Passos de Execução:**
1. Alterar a descrição/nome da modalidade para `Leo valesk`.


2. Alterar o seletor de status para `Inativo` e depois retornar para `Ativo` / salvar alterações.




* **Resultado Esperado:** Os dados e o status da modalidade devem ser atualizados na tabela.


* **Resultado Obtido:** A modalidade teve a descrição/nome alterados para `Leo valesk` e o status foi atualizado para "Inativa".


* **Status:** PASSOU

---

### 4. CT04 - Edição de Horário e Atualização de Turma

* **Objetivo:** Validar a atualização dos parâmetros de horário e vagas de uma turma existente.


* **Passos de Execução:**
1. Na linha da turma cadastrada, alterar os horários de início e fim nos campos correspondentes (ex: definindo para `09:30` até `12:30`).


2. Clicar no botão **+ Turma** ou ícone de edição para salvar.




* **Resultado Esperado:** O intervalo de horário da turma na listagem deve ser atualizado corretamente.


* **Resultado Obtido:** O horário da turma na tabela foi alterado para `09:30:00 - 12:30:00`.


* **Status:** PASSOU

---

### 5. CT05 - Exclusão de Horário e Atualização de Turma

* **Objetivo:** Validar a atualização dos parâmetros de horário e vagas de uma turma existente.


* **Passos de Execução:**
1. clique no botão de excluir
2. Nada Acontece

* **Status:** FALHOU


## Relatório de Inconsistências / Apontamentos de Interface

1. **AP-01: Comportamento da máscara/seleção de horário**
* **Descrição:** Durante o preenchimento dos campos de horário na criação/edição da turma, o seletor apresenta uma usabilidade instável ao digitar os minutos e horas diretamente no input.


* **Severidade:** Baixa (Melhoria de UX/Usabilidade).





---

## Resumo da Execução

* **Total de Testes:** 5


* **Passou:** 4


* **Falhou:** 1

https://jam.dev/c/f3126bb6-21e6-4af8-ad30-bea4effe0d7a
