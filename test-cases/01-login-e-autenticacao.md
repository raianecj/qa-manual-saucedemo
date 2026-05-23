## CT01: Login com credenciais válidas
**Funcionalidade:** Autenticação de Usuário

**Cenário:** Acesso bem-sucedido ao catálogo de produtos
  Dado que o usuário está na página de login
  Quando insere o username "standard_user" e a senha secreta
  E clica no botão "Login"
  Então o sistema redireciona para a página de inventário
  E o título "Products" é exibido na tela
