# Postgres_API

- Esse é um código que automatiza e facilita operações dentro de um ou mais banco de dados com o Sistema Gerenciador de Banco de Dados PostgreSQL, como criar tabelas, inserir, atualizar e excluir dados de forma mais prática.

## Configurações Iniciais

- Antes de utilizar este código, é necessário realizar algumas configurações iniciais:

- Instalar o pacote psycopg2: pip install psycopg2.
- Ter acesso a um banco de dados PostgreSQL, com o nome do banco de dados, usuário e senha.

## Funcionalidades

- Criar Tabela

- Para criar uma tabela, utilize o método create_table(table_name), passando como parâmetro o nome da tabela a ser criada.

```python
db = PostgresDB()
db.create_table('nome_da_tabela')
Excluir Tabela
Para excluir uma tabela, utilize o método drop_table(table_name), passando como parâmetro o nome da tabela a ser excluída.
```
```python
db = PostgresDB()
db.drop_table('nome_da_tabela')
Inserir Dados
Para inserir dados em uma tabela, utilize o método insert_data(table_name, values), passando como parâmetros o nome da tabela e os valores a serem inseridos.
```
```python
db = PostgresDB()
db.insert_data('nome_da_tabela', 'valor1, valor2, valor3')
Selecionar Dados
Para selecionar dados de uma tabela, utilize o método select_data(table_name, column='*', condition=None), passando como parâmetros o nome da tabela, a coluna a ser selecionada (opcional) e uma condição (opcional).
```
```python
db = PostgresDB()
db.select_data('nome_da_tabela', 'coluna1, coluna2', 'condicao')
Atualizar Dados
Para atualizar dados de uma tabela, utilize o método update_data(table_name, column, value, condition), passando como parâmetros o nome da tabela, a coluna a ser atualizada, o valor a ser inserido e uma condição.
```
```python
db = PostgresDB()
db.update_data('nome_da_tabela', 'coluna', 'novo_valor', 'condicao')
Adicionar Coluna
Para adicionar uma coluna em uma tabela, utilize o método add_column(table_name, column_name, data_type), passando como parâmetros o nome da tabela, o nome da coluna e o tipo de dado.
```
```python
db = PostgresDB()
db.add_column('nome_da_tabela', 'nome_da_coluna', 'tipo_de_dado')
Excluir Dados
Para excluir dados de uma tabela, utilize o método delete_data(table_name, condition, limit=None), passando como parâmetros o nome da tabela, uma condição e um limite de exclusão (opcional).
```
```python
db = PostgresDB()
db.delete_data('nome_da_tabela', 'condicao', limit=10)
Excluir Banco de Dados
Para excluir um banco de dados, utilize o método drop_database(database_name), passando como parâmetro o nome do banco de dados.
```
```python
db = PostgresDB()
db.drop_database('nome_do_banco_de_dados')
Fechar Conexão
Para fechar a conexão com o banco de
```

## Ferramentas

- Postgres
- Python