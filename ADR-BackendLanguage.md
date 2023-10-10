# **Architectural Decision Record (ADR)** 

## **Title:**

Selection of Backend Language for University Social Networking App 

## **Context:**

We are responsible for choosing the programming language for the server-side (backend) development of the university social networking app. The chosen language will have a significant impact on the app's scalability, flexibility, and ability to handle real-time interactions. 

## **Decision:**

We have decided to use Node.js as the backend language for the university social networking app.  

## **Rationale:** 

**Scalability:** 
  > Node.js is renowned for its scalability due to its event-driven, non-blocking I/O model. This architecture allows the server to handle a large number of concurrent connections efficiently, a critical requirement for a social networking app with many users. 

**Flexibility:** 
  > Node.js is flexible and well-suited for various backend requirements, including building APIs, real-time applications, and microservices. This flexibility enables us to adapt to the diverse needs of a social networking app. 

**Efficient Data Handling:** 
  > Node.js has a rich ecosystem of libraries and packages for working with databases and data manipulation. This facilitates efficient data handling, which is crucial for managing user profiles, posts, messages, and other data within the app. 

**Real-time Interactions:** 
  > Social networking apps often require real-time features such as chat, notifications, and updates. Node.js excels in building real-time applications, making it well-suited for ensuring users receive immediate updates and messages.  

**Developer Familiarity:**
  > JavaScript, the language used with Node.js, is widely known among developers. This familiarity simplifies the hiring process and promotes code reusability between frontend and backend components. 

**Community and Ecosystem:**
  > Node.js benefits from a vibrant and active developer community. This community support provides access to a wide range of libraries, tools, and resources, expediting development and troubleshooting. 


## **Consequences:** 

**Callback Hell:**
  > Node.js heavily relies on asynchronous programming using callbacks. This can lead to deeply nested callback structures. This can make the code difficult to read and maintain. 

**Callback Errors:**
  > Managing errors in callback-based code can be tricky. Developers need to be diligent in handling errors properly, and unhandled errors can lead to application crashes. 
