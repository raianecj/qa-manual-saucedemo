# Casos de Teste: Carrinho de Compras

## CT04: Adicionar produto ao carrinho
**Funcionalidade:** Gerenciamento do Carrinho  
**Descrição:** Validar se os produtos selecionados são contabilizados corretamente.

**Cenário:** Adicionar um único item pela página de inventário  
  **Dado** que o usuário está logado e na página de inventário  
  **Quando** clica no botão "Add to cart" do produto "Sauce Labs Backpack"  
  **Então** o botão do produto deve mudar para "Remove"  
  **E** o ícone do carrinho no topo da tela deve exibir o contador "1"  

---

## CT05: Remover produto do carrinho
**Funcionalidade:** Gerenciamento do Carrinho  
**Descrição:** Validar se os produtos selecionados são removidos do carrinho.

**Cenário:** Remover item diretamente da tela do carrinho  
  **Dado** que o usuário possui o item "Sauce Labs Backpack" no carrinho  
  **E** está na página do Carrinho ("Your Cart")  
  **Quando** clica no botão "Remove" correspondente ao item  
  **Então** o item deve desaparecer da lista  
  **E** o contador do ícone do carrinho deve ficar vazio (ou diminuir em 1)
