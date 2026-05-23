# Popular banco de dados H2

Sempre que a aplicação para de rodar, os dados inseridos no banco de dados H2 são deletados. Isso porque ele é um banco de dados em memória, então só existe enquanto a aplicação ainda está funcionando.

Após entender o conceito e fazer funcionar as ações de `create` de uma entidade, é possível criar um arquivo SQL para popular essa base sempre que a aplicação for iniciada. Assim, será possível focar nos testes de  listagem ou atualização de dados já existentes sem ficar criando-os toda vez.

Esse processo facilita muito quando é necessário criar dados para mais de uma entidade.

## Local do arquivo

Crie um arquivo SQL em:
`src/main/resources/data.sql`

#### Exemplo de arquivo
```INSERT INTO clientes (id, nome, email)
VALUES (1, 'Ana Silva', 'ana@email.com');

INSERT INTO produtos (id, nome, preco)
VALUES (1, 'Notebook', 3500.00);

INSERT INTO pedidos (id, cliente_id, data_pedido)
VALUES (1, 1, CURRENT_TIMESTAMP);

INSERT INTO pedido_produtos (pedido_id, produto_id)
VALUES (1, 1);
```

## Configuração para leitura do arquivo
```
spring.sql.init.mode=always
spring.jpa.defer-datasource-initialization=true
```

#### Explicação
`spring.sql.init.mode` - Define quando os scripts SQL automáticos devem ser executados.

`spring.jpa.defer-datasource-initialization` - Faz com que a aplicação expere o Hibernate terminar de criar as tabelas para só depois ler o arquivo SQL.