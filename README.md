# Blockchain-Based Audit Trail Web Application

A **secure, transparent, and tamper-proof audit trail system** built using **blockchain technology**.  
This project ensures that every user action or transaction is recorded in an immutable ledger, offering verifiable accountability across operations.  

---

## 🚀 Features

- **Blockchain Integration**: Each operation generates a transaction stored on a blockchain network for immutability.  
- **User Authentication**: Secure login system with role-based access (admin, auditor, user).  
- **Audit Logging**: Tracks every action (create, update, delete) for transparency and traceability.  
- **Data Integrity**: Prevents unauthorized manipulation of records.  
- **Web-Based Interface**: Built using Java EE and deployed on a servlet-based web server.  
- **Scalable Architecture**: Modular design supporting future extensions or integration with other systems.  

---

## ⚙️ Tech Stack

| Component | Technology |
|------------|-------------|
| **Frontend** | HTML, CSS, JavaScript, JSP |
| **Backend** | Java EE (Servlets, JSP), Maven |
| **Blockchain** | Custom lightweight blockchain implementation in Java(Using Ethereum or Local Ganauche Instance) |
| **Server** | Jetty or Tomcat |
| **Version Control** | Git & GitHub |

---

## 🧩 How It Works

1. **User Authentication**  
   Users log in using credentials stored securely in the database.  

2. **Transaction Recording**  
   Every action (insert/update/delete) triggers a blockchain transaction containing:  
   - User details  
   - Timestamp  
   - Operation type  
   - Data hash  

3. **Block Generation**  
   Transactions are grouped into blocks and linked using cryptographic hashes.  

4. **Validation**  
   Each new block is validated before being added to the chain, ensuring data integrity.  

5. **Audit Retrieval**  
   Auditors can view and verify the complete immutable transaction history through the web interface.  

---

## 🧰 Installation and Setup

### Prerequisites
- JDK 11 or higher  
- Apache Maven  
- Apache Tomcat (or any servlet container)  
- MySQL (or your chosen database)  
- Git  

---

### Steps to Run

1. **Clone this repository**
   ```bash
   git clone https://github.com/<your-username>/blockchain-audit-trail.git
   cd blockchain-audit-trail
2. **Build the project**
Use Maven to clean and install dependencies.
    ```bash
    mvn clean install

3. **Run the application**
    Run the application using the following command
   ```bash
   cd webapp
   mvn jetty:run -Dorg.eclipse.jetty.annotations.maxWait=120
4. **After some time you should see [INFO] Started Jetty Server in your console and you should be able to access the application at localhost:8080/admin with credentials admin/pass.**
