# InventoryManage-WithKafka

Kafka ui works on 7075 swagger ui 7575

For creating table Sql codes here : 

CREATE TABLE products (
    id INT PRIMARY KEY,
    name VARCHAR(255),
    category VARCHAR(255),
    quantity INT,
    is_deleted BOOLEAN
);

For instance 10 sql objects: 

INSERT INTO products (id, name, category, quantity, is_deleted) VALUES
(1, 'Smartphone', 'Electronics', 100, false),
(2, 'T-shirt', 'Clothing', 50, false),
(3, 'Milk', 'Groceries', 200, false),
(4, 'Laptop', 'Electronics', 20, false),
(5, 'Sofa', 'Furniture', 10, false),
(6, 'Jeans', 'Clothing', 150, false),
(7, 'Bread', 'Groceries', 80, false),
(8, 'Headphones', 'Electronics', 30, false),
(9, 'Ball', 'Toys', 75, false),
(10, 'Table', 'Furniture', 5, false);

in this project PostgreSql has been used for h2 dependency : 

<dependency>
    <groupId>com.h2database</groupId>
    <artifactId>h2</artifactId>
    <scope>runtime</scope>
</dependency>

and properties :
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.h2.console.enabled=true



