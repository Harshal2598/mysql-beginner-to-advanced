# Relational vs Non-Relational Databases

## 🧩 What are Relational Databases?
A **Relational Database (RDBMS)** stores data in **tables (rows and columns)**.  
Each table is related to others using **keys**.

### Examples:
- MySQL  
- PostgreSQL  
- Oracle  
- SQL Server  

### Characteristics:
- Structured and organized  
- Uses **SQL**  
- Ensures **ACID** properties (safe & consistent)  
- Best for applications requiring transactions  

---

## 🧩 What are Non-Relational Databases?
A **Non-Relational Database (NoSQL)** stores data in **flexible formats**, not limited to tables.

### Examples:
- MongoDB (Document)
- Cassandra (Column store)
- Redis (Key-Value)
- Neo4j (Graph)

### Characteristics:
- Flexible, unstructured or semi-structured data  
- Highly scalable  
- Faster for large datasets  
- Best for Big Data and real-time applications  

---

## 🔍 Key Differences

| Feature | Relational Databases | Non-Relational Databases |
|--------|------------------------|---------------------------|
| Data Model | Tables (rows & columns) | Documents, key-value, graphs, wide columns |
| Query Language | SQL | No fixed language (MongoDB queries, GraphQL, JSON-like queries) |
| Schema | Fixed schema | Dynamic/flexible schema |
| Relationships | Strong, structured relations | Loose or no relations |
| Transactions | ACID compliant | BASE (Basically Available, Soft state, Eventually consistent) |
| Scaling | Vertical scaling | Horizontal scaling |
| Best For | Banking, ERP, eCommerce | Big Data, IoT, social networks, analytics |

---

## 📝 Simple Understanding

### Relational = Structured  
- Like Excel sheets with columns & rows  
- Perfect when data is consistent and related  
- Example use: Banking, eCommerce orders

### Non-Relational = Flexible  
- Like storing JSON files  
- Great when data keeps changing form  
- Example use: Instagram posts, chats, logs

---

