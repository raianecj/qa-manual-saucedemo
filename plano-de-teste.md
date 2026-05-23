# Plano de Teste - Swag Labs (SauceDemo)

## 1. Introdução
Este documento define a estratégia de testes manuais e exploratórios para a aplicação web e-commerce Swag Labs (SauceDemo). O objetivo principal é avaliar a qualidade e a estabilidade dos fluxos críticos de negócio, garantindo uma jornada do usuário fluida desde a autenticação até a finalização de uma compra.

## 2. Escopo

**O que será testado:**
* Autenticação de usuários (Login de contas padrão, bloqueadas e com falhas);
* Exibição e ordenação do catálogo de produtos;
* Gerenciamento do Carrinho de Compras (Adição, remoção e persistência de itens);
* Fluxo completo de Checkout (Preenchimento de dados de entrega e confirmação de pedido).

**O que não será testado:**
* Recuperação de senha e criação de contas (funcionalidades não implementadas na aplicação de teste);
* Testes de carga, performance ou stress no servidor de hospedagem;
* Integração com gateways de pagamento reais.

## 3. Estratégia e Tipos de Teste
* **Testes Funcionais:** Validação das regras de negócio através de Casos de Teste estruturados utilizando a sintaxe BDD (Gherkin);
* **Testes Exploratórios baseados em Sessão:** Testes não roteirizados focados em encontrar comportamentos anômalos em fluxos de exceção;
* **Testes de UI/Responsividade:** Verificação de quebra de layout, sobreposição de elementos e clareza das mensagens de erro na interface.

## 4. Ambientes de Teste
Para garantir a fidelidade do comportamento da aplicação no mundo real, os testes serão executados nos seguintes ambientes:

**Ambiente Desktop:**
* Sistema Operacional: Windows 11
* Navegadores: Google Chrome e Mozilla Firefox (versões estáveis mais recentes)

**Ambiente Mobile:**
* Dispositivo Físico: POCO X7 Pro
* Sistema Operacional: Android
* Navegador: Mozilla Firefox Mobile

## 5. Gerenciamento de Defeitos
Todas as falhas e inconsistências encontradas serão reportadas na aba **Issues** deste repositório. O padrão de reporte inclui obrigatoriamente:
* Título claro e objetivo;
* Pré-condições e Passos para reproduzir;
* Comportamento Esperado vs. Comportamento Atual;
* Ambiente utilizado (Desktop ou Mobile);
* Evidências visuais (Screenshots ou vídeos curtos);
* Etiquetas (Labels) indicando o nível de Severidade (Critica, Alta, Média, Baixa).

## 6. Critérios de Conclusão 
A etapa de testes manuais será considerada concluída quando:
* 100% dos Casos de Teste documentados forem executados;
* Nenhum defeito de severidade "Crítica" ou "Alta" estiver bloqueando os fluxos de Login e Checkout;
* Os resultados da execução estiverem sumarizados no `README.md` principal do projeto.
