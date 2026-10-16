# QA Manual — SauceDemo (Swag Labs)

## Sobre o projeto

Projeto de portfólio de Quality Assurance (QA), desenvolvido para demonstrar habilidades de testes manuais em aplicações web.

A aplicação utilizada foi o [SauceDemo](https://www.saucedemo.com/), um ambiente demonstrativo para prática de testes de software.

## Funcionalidades testadas

| ID | Funcionalidade | Resultado |
|---|---|---|
| CT-001 | Adição de produto ao carrinho | Aprovado |
| CT-002 | Remoção de produto do carrinho | Aprovado |
| CT-003 | Finalização de compra e conferência de valores | Aprovado nos cenários verificados |
| CT-004 | Autenticação com credenciais inválidas | Aprovado |

## Defeito identificado

**BUG-001 — Sobreposição de texto na mensagem de erro de login**

Durante os testes, foi identificado um problema visual na apresentação da mensagem de erro após uma tentativa de autenticação inválida.

- Tipo: Interface (UI)
- Gravidade proposta: Baixa
- Ambiente: Chromium / Windows
- Situação: Documentado

## Documentação

- [Relatório final de testes](relatorio-final.md)
- [Relatório do defeito BUG-001](bug-001.md)
- [Evidências dos testes](evidencias/)

## Escopo e limitações

Os testes foram executados manualmente, em cenários selecionados de login, carrinho e checkout.

Os resultados não representam uma validação completa da aplicação. Funcionalidades e condições adicionais ainda exigiriam testes.

## Autor

**Vinícius Gomes**  
QA Automation | Testes manuais e automação de testes

Projeto independente de estudo e portfólio, sem vínculo comercial com a Sauce Labs.
