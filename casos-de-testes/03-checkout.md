# Casos de Teste: Checkout

## CT06: Finalizar compra com sucesso
**Funcionalidade:** Finalização de Pedido  
**Descrição:** Validar o fluxo completo desde a inserção de dados de entrega até o fim da jornada.

**Cenário:** Compra realizada com formulário preenchido corretamente  
  **Dado** que o usuário está na página "Checkout: Your Information"  
  **E** possui itens no carrinho  
  **Quando** preenche "First Name" com "João"  
  **E** preenche "Last Name" com "Silva"  
  **E** preenche "Zip/Postal Code" com "70000-000"  
  **E** clica no botão "Continue"  
  **Então** o sistema redireciona para a página "Checkout: Overview"  
  **Quando** o usuário clica no botão "Finish"  
  **Então** o sistema exibe a página "Checkout: Complete!"  
  **E** exibe a mensagem de sucesso "Thank you for your order!"  

---

## CT07: Validação de campos obrigatórios no Checkout
**Funcionalidade:** Finalização de Pedido  
**Descrição:** Validar os campos obrigatórios.

**Cenário:** Tentativa de avançar sem preencher o "First Name"  
  **Dado** que o usuário está na página "Checkout: Your Information"  
  **Quando** deixa o campo "First Name" em branco  
  **E** preenche "Last Name" e "Zip/Postal Code"  
  **E** clica no botão "Continue"  
  **Então** o sistema não deve avançar de página  
  **E** deve exibir a mensagem de erro "Error: First Name is required"
