
---

# Casos de Teste - Módulo Autenticação (Login)

* **Sistema:** SIFIT
* **Módulo:** Autenticação > Login
* **Ficheiro de Cenário:** `CT_RF01_Login na Plataforma.md`

---

### 1. C01-CT01 - Login com Credenciais Válidas

* **Objetivo:** Validar o acesso à plataforma SIFIT utilizando nome de usuário e senha válidos.
* **Pré-condições:** Credenciais do usuário (`marcelo_zandonadi`) devidamente cadastradas e ativas no sistema.
* **Passos de Execução:**
1. Acessar a página de login do SIFIT.
2. Preencher o campo **Login** com `marcelo_zandonadi`.
3. Preencher o campo **Senha** com a senha válida.
4. Clicar no botão **Entrar**.


* **Resultado Esperado:** O sistema deve autenticar o usuário e redirecioná-lo para a Página Inicial / Dashboard com a saudação de boas-vindas ("Bom dia, Jair!").
* **Resultado Obtido:** Redirecionamento realizado com sucesso para a Dashboard exibindo a mensagem de boas-vindas.
* **Status:** PASSOU

---

### 2. C01-CT02 - Tentativa de Login com Credenciais Incorretas

* **Objetivo:** Verificar a resposta do sistema ao tentar realizar login com usuário ou senha inválidos.
* **Pré-condições:** Nenhuma.
* **Passos de Execução:**
1. Acessar a página de login do SIFIT.
2. Preencher o campo **Login** com `asfadf`.
3. Preencher o campo **Senha** com `********`.
4. Clicar no botão **Entrar**.


* **Resultado Esperado:** O login não deve ser efetuado e o sistema deve exibir a mensagem de alerta no topo do formulário: *"O nome de usuário e senha não correspondem."*
* **Resultado Obtido:** Acesso bloqueado e mensagem de erro apresentada conforme esperado.
* **Status:** PASSOU

---

### 3. C01-CT03 - Tentativa de Login com Campos em Branco

* **Objetivo:** Validar a obrigatoriedade do preenchimento dos campos de login e senha.
* **Pré-condições:** Nenhuma.
* **Passos de Execução:**
1. Acessar a página de login do SIFIT.
2. Manter os campos **Login** e **Senha** em branco.
3. Clicar no botão **Entrar**.


* **Resultado Esperado:** O sistema deve impedir a submissão do formulário e exibir as mensagens/indicadores de validação solicitando o preenchimento dos campos obrigatórios.
* **Resultado Obtido:** Submissão bloqueada com exibição dos alertas de validação nos campos obrigatórios.
* **Status:** PASSOU

---

## Resumo da Execução

* **Total de Testes:** 3
* **Passou:** 3
* **Falhou:** 0
https://jam.dev/c/b225c763-bd9d-4085-b055-ad10afde41f0
