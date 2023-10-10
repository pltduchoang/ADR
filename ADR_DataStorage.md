# **Architectural Decision Record (ADR)** 

## **Title:**

Selection of Data Storage Solutions for University Social Networking App

## **Context:**

We need to make a decision regarding the data storage solutions that will be used to manage various types of data within the university social networking app. This includes user profiles, posts, messages, and other app-related information. There are various options to choose from, such as Relational Database, NoSQL Database, Graph Database, Object Storage, etc. Each offers different benefits and presents unique drawbacks. 

## **Decision:**

We have decided to use a **combination of relational and NoSQL databases** to manage data within the app. 

## **Rationale:** 

**The best of both worlds:** 
  > Combining relational and NoSQL databases allows us to handle a variety of data types effectively. Relational databases are suitable for structured data such as user profiles and grades, while NoSQL databases are better for semi-structured data like user-generated content, posts, message and multimedia contents. 

**Efficiency:** 
  > Relational databases offer efficient data retrieval and querying capabilities, ensuring that structured data can be accessed and manipulated effectively. NoSQL databases excel at handling semi-structured and unstructured data, which is common in social networking apps. 

**Scalability:** 
  > NoSQL databases are horizontally scalable and can accommodate high volumes of data and user-generated content, which is crucial for a social networking app with potentially constant growth in user base. 

**Data Integrity:** 
  > Relational databases provide data integrity through ACID (Atomicity, Consistency, Isolation, Durability) transactions, which is essential for maintaining the integrity of sensitive data, such as student grades. 

**Flexibility:** 
  > The combination of relational and NoSQL databases offers flexibility in data modeling, allowing us to adapt to changing requirements and data structures as the app evolves. 


## **Consequences:** 

**Complexity:**
  > Managing both types of databases can significantly increase the complexity of your application's architecture. Developers need to understand and work with two different database paradigms, which can lead to more intricate code and data synchronization logic. 

**Data Consistency:**
  > Maintaining data consistency between relational and NoSQL databases can be challenging. Inconsistent or out-of-sync data can occur if updates are not carefully managed. 

**Data Migration:**
  > Data migration between relational and NoSQL databases, especially when changing the data model or making schema updates, can be complex and error-prone. Ensuring data integrity during migrations is crucial. 
