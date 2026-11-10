# PM-Noite-Pratica-5

## Prática 5 — Testes Automatizados com JUnit

### Exercício: Testes Automatizados do Sistema de Pedidos

Nesta prática, devem ser implementados os testes automatizados para o sistema de pedidos criado na Prática 5. Todas as regras de negócio e exceções devem ser testadas.

1. Adicionar a **JUnit Jupiter API** e o **JUnit Jupiter Engine** em `Properties > Libraries` nas propriedades do projeto. Também é possível baixá-los pelo site [junit.org](https://junit.org/), caso não seja possível adicioná-los pela IDE.
2. Adicionar os arquivos JAR ao projeto, verificando o procedimento de acordo com a IDE utilizada.
   - **Observação:** em projetos Maven, essa etapa não é necessária. A dependência do JUnit deve ser configurada no `pom.xml`.
3. Criar uma classe de teste para cada classe de domínio do projeto, sem incluir as exceções personalizadas. Por exemplo: `PedidoEletronicoTest.java`.
4. Implementar os seguintes testes:
   - cálculo do valor final;
   - exceções personalizadas;
   - exceções do Java;
   - processamento do pedido, validando a alteração do status;
   - regra do enum: pedidos com status `ENTREGUE` não podem ser alterados;
   - utilizar `@AfterEach` para instanciar objetos e inicializar valores antes de cada teste;
   - utilizar `@AfterEach` para informar que o teste foi finalizado.
5. Observações:
   - todos os tipos de pedido devem ser testados;
   - caso alguma regra de negócio esteja no lugar incorreto (por exemplo, na classe `main`), ela deve ser movida para a classe correta;
   - os testes não devem ser executados na classe `main`.