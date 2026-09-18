Cenário 01: Login na plataforma.Caso de Teste 01: Login com as credenciais válidas.ID: C01-CT01 
Descrição: O login será realizado com um nome de usuário e uma senha válidos na plataforma SIFIT.

Pré-condições: As credenciais fornecidas (marcelo_zandonadi / senha) devem ser válidas e cadastradas no sistema.   
Passos:DADO que estamos na página de login do SIFIT   E preenchemos "marcelo_zandonadi" no campo Login   E preenchemos a senha válida no campo Senha 

QUANDO clicarmos no botão "Entrar"   
ENTÃO seremos redirecionados para a Página Inicial / Dashboard do sistema SIFIT   Critérios de aceitação: O redirecionamento para a Página Inicial ("Bom dia, Jair!") deve ocorrer corretamente.   

Caso de Teste 02: Tentativa de login com credenciais incorretas.ID: C01-CT02   Descrição: O login falhará quando o nome de usuário ou a senha forem inválidos.   
Pré-condições: Nenhuma.  

Passos:DADO que estamos na página de login do SIFIT   E preenchemos "asfadf" no campo Login   E preenchemos "********" no campo Senha   QUANDO clicarmos no botão "Entrar"   ENTÃO uma mensagem de erro "O nome de usuário e senha não correspondem." será exibida no topo do formulário   Critérios de aceitação: A mensagem de alerta "O nome de usuário e senha não correspondem." deve ser exibida ao usuário.

Caso de Teste 03: Tentativa de login com campos em branco.ID: C01-CT03   
Descrição: O login falhará quando os campos de login e senha forem apaga dos ou mantidos em branco.   

Pré-condições: Nenhuma.   Passos:DADO que estamos na página de login do SIFIT   E deixamos os campos Login e Senha em branco   
QUANDO clicarmos no botão "Entrar"   

ENTÃO o sistema deve impedir a submissão e exibir mensagens de validação solicitando o preenchimento dos campos   Critérios de aceitação: Os campos obrigatórios devem impedir o acesso e exibir alertas de validação apropriados

https://jam.dev/c/b225c763-bd9d-4085-b055-ad10afde41f0
