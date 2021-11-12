# EmployeeManagement

# **Iteration 1**

## *APIs*
#### CRUD for employee REST API
- CRUD for a single employee `done`
- Get employees by list of IDs `TODO`
- Employee search by criteria ( name, department )
- Paginated employee search

#### CRUD for department REST API
- CRUD for single department `in-progress`
- API to add and remove employees in a department
  - Check if the employee exists in any other department or not

#### Payroll REST API
- For counting salary based on number of unpaid leaves

#### Analytics REST API
- Total salary payout by department
- Average paid and unpaid leaves by department


## *Tech stack and tools*
- Spring boot
- Oracle
- JDBC (no hibernate or spring data JPA for now. We will use that in next iteration)
- Java 11
- IntelliJ Idea
- Github
- JUnit
- Maven
- cUrl / Postman

## *Recommendations*
- Use streams and lambdas for all collection operations
- Use SOLID principles of object oriented programming
- Write tests first and then write actual code
- Do development on local->commit->push to your fork->open PR for employee management repo

# **Iteration 2**

- CRUD for leaves and approval
- HR department data to manage leaves
- spring data JPA integration
- swagger integration
- Containerization with Docker
- Github pages integration
- Integration with Jenkins
- Integration with static code analysis

# **Iteration 3**

- Implement simple JDBC and remove data-JPA
- Implement in-memory cache using hashmap for each microservices
- Implement all search functionalities using this cache and not database queries
- Implement sort order in each search API
- Implement DB connection pool
  - datastructure or structures to hold connection
  - you should be able to know which connection object is in use
  - public getConnection()
  - private createNewConnection()
  - there should be an upper limit on how many db connections can be created by DB pool
  - there should be a lower limit or an initialization number which will determine how many connections will be created at the time of db pool initialization
