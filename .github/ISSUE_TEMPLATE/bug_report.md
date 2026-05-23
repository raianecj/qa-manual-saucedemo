## Descrição do Bug
<!-- Faça um resumo claro e conciso do problema encontrado. -->
Ao tentar finalizar uma compra com o carrinho cheio, o botão "Finish" não responde aos cliques na resolução mobile, impedindo a conclusão do pedido.

## Passos para Reproduzir
<!-- Liste o passo a passo exato para chegar ao bug. -->
1. Acesse a página inicial do e-commerce.
2. Faça login com o usuário `standard_user` e a senha correta.
3. Adicione o item "Sauce Labs Backpack" ao carrinho.
4. Clique no ícone do carrinho no canto superior direito.
5. Clique no botão "Checkout".
6. Preencha as informações de entrega (First Name, Last Name, Zip/Postal Code) e clique em "Continue".
7. Na tela de "Checkout: Overview", clique no botão "Finish".

## Comportamento Esperado
O sistema deveria processar o pedido, redirecionar o usuário para a página de "Checkout: Complete!" e exibir a mensagem "Thank you for your order!".

## Comportamento Atual
O botão "Finish" reage visualmente ao clique (muda de cor), mas nenhuma ação ocorre. O usuário permanece na mesma tela e nenhum erro é exibido no console do navegador, tornando impossível finalizar a compra pelo celular.

## Ambiente
<!-- Detalhe o hardware, sistema operacional e navegador onde o teste foi executado. -->
* **Tipo de Teste:** Mobile (Dispositivo Físico)
* **Dispositivo:** POCO X7 Pro
* **Sistema Operacional:** Android 14
* **Navegador:** Google Chrome Mobile (Versão 123.0)

<!-- Exemplo alternativo para Desktop:
* **Tipo de Teste:** Desktop
* **Dispositivo:** PC Intel i5, 8GB RAM
* **Sistema Operacional:** Windows 10
* **Navegador:** Mozilla Firefox (Versão 125.0.1)
-->

## Evidências
<!-- Anexe screenshots, GIFs ou pequenos vídeos mostrando o erro acontecendo. No GitHub, basta arrastar o arquivo para cá. -->
[Inserir Screenshot da tela travada no Checkout ou GIF tentando clicar no botão]

## Severidade e Prioridade
* **Severidade:** Crítica (Impede a conversão/venda e o fluxo principal de negócio).
* **Prioridade de Correção:** Alta
