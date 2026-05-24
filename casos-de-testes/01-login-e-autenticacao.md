# Casos de Teste: Login e Autenticação

## CT01: Login com credenciais válidas
**Funcionalidade:** Autenticação de Usuário  
**Descrição:** Validar que um usuário comum consegue acessar o catálogo de produtos.

**Cenário:** Acesso bem-sucedido com usuário padrão  
  **Dado** que o usuário está na página inicial de login  
  **Quando** insere o usuário "standard_user"  
  **E** insere a senha "secret_sauce"  
  **E** clica no botão "Login"  
  **Então** o sistema redireciona para a página de inventário  
  **E** o título "Products" é exibido no topo da tela  
  **E** o ícone do carrinho de compras fica visível  

---

## CT02: Tentativa de login com usuário bloqueado (Cenário Negativo)
**Funcionalidade:** Autenticação de Usuário  
**Descrição:** Garantir que usuários com restrição de acesso sejam impedidos de logar.

**Cenário:** Acesso negado para usuário bloqueado  
  **Dado** que o usuário está na página inicial de login  
  **Quando** insere o usuário "locked_out_user"  
  **E** insere a senha "secret_sauce"  
  **E** clica no botão "Login"  
  **Então** o sistema deve permanecer na página de login  
  **E** exibir a mensagem de erro: "Epic sadface: Sorry, this user has been locked out."

---

## CT03: Tentativa de login com senha incorreta
**Funcionalidade:** Autenticação de Usuário  
**Descrição:** Garantir que usuários com senha incorreta não consiga logar.

**Cenário:** Acesso negado por credenciais inválidas  
  **Dado** que o usuário está na página inicial de login  
  **Quando** insere o usuário "standard_user"  
  **E** insere a senha "senha_errada_123"  
  **E** clica no botão "Login"  
  **Então** exibir a mensagem de erro: "Epic sadface: Username and password do not match any user in this service"
