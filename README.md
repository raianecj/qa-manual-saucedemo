# QA Portfolio | Testes Manuais & Modelagem BDD

Bem-vindo ao repositório de testes manuais do meu portfólio de Quality Assurance. 

Este projeto tem como objetivo demonstrar a aplicação de técnicas de **Engenharia de Qualidade** em um ambiente web simulado. O foco deste portfólio é mostrar como estruturar o pensamento analítico, modelar cenários de negócio e documentar falhas.

## Aplicação Alvo
A aplicação testada é o **Swag Labs (SauceDemo)**, um e-commerce fictício utilizado na comunidade de testes para validar fluxos de autenticação, gestão de estado (carrinho) e finalização de pedidos.

---

## Estrutura e Navegação do Projeto

Aqui você encontra toda a documentação gerada durante o ciclo de testes, dividida por responsabilidades:

### 1. Estratégia de Qualidade
* 📄 **[Plano de Teste](./plano-de-teste.md):** Documento detalhando escopo, ambientes (Desktop e Mobile) e critérios de aceite para os testes.

### 2. Modelagem de Testes (BDD / Gherkin)
Os cenários foram modelados em linguagem natural estruturada (Gherkin) para facilitar a comunicação com áreas de negócio e para futura automação.
* 📦 **[CTs de Login e Autenticação](./casos-de-testes/01-login-e-autenticacao.md)** (Caminhos felizes e fluxos de exceção)
* 📦 **[CTs do Carrinho de Compras](./casos-de-testes/02-carrinho-de-compras.md)** (Lógica de adição, remoção e persistência)
* 📦 **[CTs de Checkout](./casos-de-testes/03-checkout.md)** (Fluxo End-to-End de compra e validação de formulários)

### 3. Gestão de Defeitos (Bug Tracking)
Os bugs encontrados durante os testes exploratórios ficam diretamente na aba de Issues do repositório.
* 🐛 **[Visualizar Bugs Reportados](../../issues)** *(Clique na aba "Issues" deste repositório)*
* 📝 **[Template Padrão de Bug Report](.github/ISSUE_TEMPLATE/bug_report.md)** criado para padronizar as evidências e passos de reprodução.

---

## 🛠️ Tecnologias e Metodologias Aplicadas
* **Metodologia Ágil:** Escrita de cenários orientados a comportamento (BDD).
* **Testes Exploratórios:** Sessões não roteirizadas baseadas em heurísticas.
* **Markdown:** Documentação versionada no próprio código.

---

## 📊 Métricas da Execução
| Tipo | Quantidade | Status |
| :--- | :---: | :---: |
| **Casos de Teste Criados** | 7 | ✅ Concluídos |
| **Bugs Críticos/Altos** | 1 | 🔴 Aberto na Issue |

> **Próximos Passos:** Este repositório serve como base para o projeto de automação. Os cenários mapeados aqui em Gherkin serão automatizados utilizando **Cypress** e integrados em uma esteira de CI/CD (GitHub Actions) em um repositório dedicado.
