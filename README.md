# CRUD Operations with Multiple Databases

## Overview

This repository contains implementations of CRUD operations across six different types of databases: Relational, Document, Vector, Graph, Key-Value Pair, and Time-Series. Each database is chosen based on specific use cases to highlight its unique strengths and capabilities.

## Databases and Use Cases

1. **Relational Database (MySQL):** User Management System  
2. **Document Database (MongoDB):** Product Catalog  
3. **Vector Database (Pinecone):** Semantic Search for Text Documents  
4. **Graph Database (Neo4j):** Organizational Hierarchy  
5. **Key-Value Pair Database (Redis):** Session Management  
6. **Time-Series Database (InfluxDB):** Monitoring and Metrics  

## Why These Databases?

Each database was selected based on its strengths and suitability for the given use case:

- **MySQL:** Fast, reliable, and suitable for read-heavy applications with robust ACID support.
- **MongoDB:** Flexible schema, ideal for unstructured data like product catalogs.
- **Pinecone:** Specialized in vector searches, perfect for semantic search applications.
- **Neo4j:** Optimized for handling complex relationships and hierarchical data.
- **Redis:** In-memory storage, providing extremely fast session management.
- **InfluxDB:** Efficient handling of time-series data, great for monitoring and metric storage.

## Setting Up the Environment

### Environment Configuration

To securely manage sensitive information like database credentials, create a `.env` file in the project root directory. This file should contain the following environment variables:

```plaintext
# .env file
MYSQL_HOST=localhost
MYSQL_USER=root
MYSQL_PASSWORD=yourpassword
MYSQL_DB=yourdatabase

MONGODB_URI=mongodb://localhost:27017/
PINECONE_API_KEY=your_pinecone_api_key

NEO4J_URI=bolt://localhost:7687
NEO4J_USER=neo4j
NEO4J_PASSWORD=yourpassword

REDIS_HOST=localhost
REDIS_PORT=6379

INFLUXDB_HOST=localhost
INFLUXDB_PORT=8086
INFLUXDB_DB=metrics
INFLUXDB_DB=token
```

## How to Run the Code

1. Clone the repository to your local machine.
2. Set up the required databases and ensure they are running locally or accessible via network.
3. Install the necessary Python libraries:
   ```bash
   pip install mysql-connector-python pymongo pinecone-client neo4j redis influxdb
