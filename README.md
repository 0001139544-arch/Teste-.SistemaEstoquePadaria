 Casos de Teste — SistemaEstoquePadaria

 CT01

  ID Caso de Teste: CT01
  ID Requisito Funcional: RF01
  Descrição: Testar cadastro de produto
  Precondição: Banco de dados conectado
  Passos:
  1. Inserir um novo produto
  2. Salvar no banco
  Resultado esperado:
  Produto cadastrado com sucesso

CT02

  ID Caso de Teste: CT02
  ID Requisito Funcional: RF02
  Descrição: Testar consulta de produtos
  Precondição: Produtos cadastrados no banco
  Passos:
  1. Executar SELECT * FROM produtos
  Resultado esperado:
  Lista de produtos exibida corretamente

CT03

  ID Caso de Teste: CT03
  ID Requisito Funcional: RF03
  Descrição: Testar produtos abaixo do estoque mínimo
  Precondição: Produto com quantidade menor que a mínima
  Passos:
  1. Executar consulta de estoque mínimo
  Resultado esperado:
  Sistema exibe alerta de estoque baixo

 CT04

  ID Caso de Teste: CT04
  ID Requisito Funcional: RF04
  Descrição: Testar filtro por categoria
  Precondição: Produtos cadastrados com categorias
  Passos:
  1. Executar filtro da categoria Bolos
  Resultado esperado:
  Apenas produtos da categoria Bolos aparecem

 CT05

  ID Caso de Teste: CT05
  ID Requisito Funcional: RF05
  Descrição: Testar consulta de produtos vencidos
  Precondição: Produto vencido cadastrado
  Passos:
  1. Executar consulta de produtos vencidos
  Resultado esperado:
  Sistema exibe produtos vencidos

CT06

  ID Caso de Teste: CT06
  ID Requisito Funcional: RF06
  Descrição: Testar entrada de estoque
  Precondição: Produto existente no banco
  Passos:
  1. Executar UPDATE aumentando quantidade
  Resultado esperado:
  Quantidade do produto atualizada corretamente

 CT07

  ID Caso de Teste: CT07
  ID Requisito Funcional: RF07
  Descrição: Testar saída de estoque
  Precondição: Produto existente no banco
  Passos:
  1. Executar UPDATE diminuindo quantidade
  Resultado esperado:
  Quantidade do produto reduzida corretamente

CT08

 ID Caso de Teste: CT08
 ID Requisito Funcional: RF08
 Descrição: Testar conexão com banco de dados
 Precondição: MySQL iniciado
 Passos:
 1. Executar classe Conexao.java
 Resultado esperado:
 Mensagem de conexão realizada com sucesso
