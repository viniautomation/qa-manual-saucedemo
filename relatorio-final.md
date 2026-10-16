Relatório de Testes Manuais Web

Aplicação: Swag Labs (SauceDemo)
Data: 16/10/2026
Autor: Vinícius Gomes - QA Automation
Contexto: Projeto de portfólio realizado em aplicação demonstrativa.

1. Objetivo

Avaliar funcionalidades selecionadas da aplicação Swag Labs, registrar os resultados dos testes executados, identificar possíveis defeitos e apresentar recomendações com base nas evidências coletadas.

2. Funcionalidades avaliadas

Login: O acesso com as credenciais válidas utilizadas durante os testes funcionou. Quatro combinações de credenciais inválidas foram rejeitadas, mantendo o usuário fora da área autenticada.

Carrinho: Os produtos selecionados foram adicionados corretamente. A remoção de um produto foi realizada sem afetar os outros dois itens presentes no carrinho.

Checkout: Em uma compra com dois produtos, os preços unitários apresentados corresponderam aos preços observados na seleção. O subtotal correspondeu à soma dos produtos, e o valor total correspondeu ao subtotal acrescido do imposto exibido.

Pós-compra: A confirmação da compra foi apresentada. O recibo em PDF foi gerado e os produtos e valores conferidos corresponderam aos da compra testada.

3. Problemas identificados

BUG-001 — Texto sobreposto na mensagem de erro de login

A mensagem exibida após uma tentativa de autenticação inválida apresentou sobreposição e corte parcial do texto, dificultando sua leitura.

Ambiente observado: Chromium 155.0.8059.80, Windows, zoom de 100%.

Gravidade proposta: Baixa.

Impacto: Prejudica a legibilidade da mensagem, mas não impede o funcionamento do login.

Os passos para reprodução e as evidências estão registrados no relatório específico do defeito.

4. Recomendação de liberação

As funcionalidades avaliadas apresentaram comportamento satisfatório nos cenários executados, com um defeito visual de baixa gravidade identificado.

Não foram observadas falhas que impedissem os fluxos de compra testados.

Entretanto, este relatório não representa uma aprovação integral do sistema, pois outras funcionalidades e cenários permanecem sem avaliação. Recomenda-se ampliar a cobertura antes de uma decisão definitiva sobre a liberação de toda a aplicação.

5. Limitações da cobertura

As seguintes funcionalidades não foram avaliadas de maneira específica ou completa:

Navegação por todas as opções do menu, incluindo All Items e About.

Dynamic Catalog.

Logout e Reset App State.

Links de redirecionamento para redes sociais.

Filtros e ordenação de produtos.

Também não foram explorados suficientemente os seguintes cenários:

Outros tipos de falha de autenticação.

Diferentes quantidades e combinações de produtos.

Campos vazios ou inválidos durante o checkout.

Comportamento da sessão em períodos prolongados.

6. Conclusão

Os testes realizados apresentaram resultados satisfatórios nos fluxos selecionados de autenticação, carrinho e finalização de compra.

Foi identificado um defeito visual de baixa gravidade na apresentação da mensagem de erro de login.

Os resultados são limitados aos cenários executados e não garantem a ausência de defeitos nas demais funcionalidades da aplicação.