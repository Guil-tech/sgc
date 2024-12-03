## English Documentation:

## Commercial Management System (SGC)

This was my first project that I pushed to github (In the year 2021). The project contains a SQL script to create one database for a Commercial Management System (SGC). The database includes essential tables for managing warehouses, parts, customers, sellers, and orders.

## Table Structure

1. **armazem**:
   - `id`: Unique identifier for the warehouse.
   - `nome`: Warehouse name.

2. **peca**:
   - `id`: Unique identifier for the part.
   - `nome`: Part name.
   - Foreign key: `id` referencing `armazem(id)`.

3. **cliente**:
   - `id`: Unique identifier for the customer.
   - `nome`: Customer name.
   - `credito`: Available credit for the customer.

4. **vendedor**:
   - `id`: Unique identifier for the seller.
   - `nome`: Seller name.

5. **pedido**:
   - `id`: Unique identifier for the order.
   - `comissao`: Seller commission associated with the order.
   - Foreign keys: `id` referencing `cliente(id)` and `vendedor(id)`.

6. **item**:
   - `id`: Unique identifier for the item.
   - `quantidade`: Quantity of the item in the order.
   - `preco`: Item price.
   - Foreign keys: `id` referencing `peca(id)` and `pedido(id)`.

- Observation 1: The extesion .brm3 is from a relational database modeling tool called "brModelo".
- Observation 2: It's worth remembering that much of what was written (code, challenge and documentation) is for Portuguese speakers, but I believe that the general scope can be understood by speakers of any language.

## Brazilian Portuguese Documentation

## Sistema de Gerenciamento Comercial (SGC)

Esse foi o meu primeiro projeto que subi no github. No ano de 2021. Este projeto contém um script SQL para criar o banco de dados de um Sistema de Gerenciamento Comercial (SGC). O banco de dados inclui tabelas essenciais para gerenciamento de armazéns, peças, clientes, vendedores e pedidos.

## Estrutura das Tabelas

1. **armazem**:
   - `id`: Identificador único do armazém.
   - `nome`: Nome do armazém.

2. **peca**:
   - `id`: Identificador único da peça.
   - `nome`: Nome da peça.
   - Foreign key: `id` referenciando `armazem(id)`.

3. **cliente**:
   - `id`: Identificador único do cliente.
   - `nome`: Nome do cliente.
   - `credito`: Crédito disponível para o cliente.

4. **vendedor**:
   - `id`: Identificador único do vendedor.
   - `nome`: Nome do vendedor.

5. **pedido**:
   - `id`: Identificador único do pedido.
   - `comissao`: Comissão do vendedor associada ao pedido.
   - Foreign keys: `id` referenciando `cliente(id)` e `vendedor(id)`.

6. **item**:
   - `id`: Identificador único do item.
   - `quantidade`: Quantidade do item no pedido.
   - `preco`: Preço do item.
   - Foreign keys: `id` referenciando `peca(id)` e `pedido(id)`.
