# **Architectural Decision Record (ADR)** 

## **Title:**

Role-Based Access Control (RBAC) for University Social Networking App

## **Context:**

We must decide among many models, such as Role-Based Access Control, Attribute-Based Access Control, or Mandatory Access Control, etc. To choose an approach for managing permissions and access control within the university social networking app. Effective access control is crucial for ensuring that users have appropriate access to features and data. 

## **Decision:**

We have decided to implement a Role-Based Access Control (RBAC) system for managing permissions within the app. 

## **Rationale:** 

**Granular Control:** 
  > RBAC provides granular control over user access based on predefined roles. This aligns with the app's need to differentiate between various user types, such as students and professors, and control their access to specific features and data. 

**Simplicity and Clarity:** 
  > RBAC is straightforward and easy to understand. It simplifies the management of permissions by associating roles with specific actions and resources, making it clear who can do what within the app. In the case of our application, there are not many roles to be expected, which makes RBAC suitable. 

**Scalability:** 
  > Keeping in mind the scalability requirement of our social app, RBAC is scalable and can accommodate additional roles and permissions as the app's functionality expands. This ensures that the access control system can grow with the app. 

**Ease in enforcing Security Policies:** 
  > RBAC enables the enforcement of security policies and helps prevent unauthorized access to sensitive data or functionality. This is particularly important when handling user profiles, grades, and other confidential information. 

**Developer-Friendly:** 
  > RBAC is popular and developer-friendly, it can be easily understood and implemented efficiently, ensuring that permissions are properly enforced in the backend. 


## **Consequences:** 

**Role complexity:**
  > While being suitable for our social app and offering certain scalability, the user base and roles need to be efficiently managed to avoid excessive diversifying (or Role Explosion), since RBAC is not ideal in the case of a large organization with heavily diverse user roles. 

**Flexibility:**
  > RBAC, in its own strength, works well in assuming that the users fit neatly into predefined roles, where the permission of different roles is not excessively overlapped. This might not be the case in reality. By choosing RBAC, some of the flexibility is sacrificed. 

**Lack of context:**
  > RBAC does not take into account the context when granting or denying access to users. In some cases, this can be troublesome, potentially leading to over-privileged or under-privileged. 
