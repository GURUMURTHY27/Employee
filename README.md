Employee Management System (EMS)

 A full-stack Java web application for managing employee records with full CRUD and search functionality, built using Spring MVC, JPA/Hibernate, and JSP.

(A sample java project)

Tech Stack

  * Backend: Java, Spring MVC (@Controller, ModelAndView), JPA (EntityManager)
  * Frontend: JSP (create.jsp, allemployees.jsp, update.jsp)
  * Build Tool: Maven (pom.xml)



Features and Endpoints

  * /createpage (Create UI): Loads the employee creation form (create.jsp).
  * /save (Create): Persists a new employee record with Name, Email, Phone, Department, Position, Salary, Address, and Date of Joining.
  * /allemployees (Read): Fetches and displays all employee records (allemployees.jsp).
  * /search?sq=... (Search): Case-insensitive search across all employee fields (ID, Name, Email, Phone, Department, Position, Salary, Address, Date of Joining).
  * /updatepage?id=... (Update UI): Loads the pre-filled update form for a specific employee (update.jsp).
  * /update (Update): Merges updated employee details into the database.
  * /delete?id=... (Delete): Removes an employee record by ID.


Project Structure

ems/
src/main/
java/org/jsp/
Config.java
Employee.java
EmployeeController.java
resources/META-INF/
webapp/
pom.xml



Setup and Run

 Configure your database connection inside src/main/resources/META-INF/persistence.xml.
 Build with Maven and deploy to a servlet container (such as Apache Tomcat): mvn clean package
