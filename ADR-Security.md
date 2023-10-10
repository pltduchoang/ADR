# **Architectural Decision Record (ADR)** 

## **Title:**

Data Privacy and Security Measures for University Social Networking App

## **Context:**

We need to make architectural decisions regarding data privacy and security to ensure that user data, including sensitive information like grades, remains protected and compliant with relevant regulations.  

## **Decision:**

We have decided to implement a series of data privacy and security measures, including encryption, secure data transmission protocols (HTTPS), and compliance with relevant data protection regulations.  

## **Rationale:** 

**Encryption:** 
  > Data encryption will be implemented to protect sensitive information both at rest and in transit. This includes encrypting data stored in databases and ensuring secure communication between the app and backend services.  

**Secure Data Transmission:** 
  > HTTPS will be used to encrypt data transmitted between the app and server, safeguarding data during transit. 

**Compliance:** 
  > The app will adhere to relevant data protection regulations, such as GDPR or HIPAA, to ensure the privacy and security of user data. Compliance is essential when handling sensitive information like student grades.

**Data Minimization:** 
  > Data minimization principles will be followed, meaning that only necessary data will be collected and stored, reducing the potential exposure of sensitive information. 

**Access Control:**
  > Role-Based Access Control (RBAC) will be enforced to restrict access to sensitive data only to authorized users, such as professors and administrators. 


## **Consequences:** 

**User education:**
  > It may require to provide basic training to the user so that they understand how the security measures of the app works. 

**Performance tradeoff:**
  > Security measures like encryption and secure data transmission protocols can  impact the app's performance, especially on devices with limited processing power or network connectivity.  