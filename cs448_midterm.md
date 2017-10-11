# 1.1
### data:
- Known facts that can be recorded and have an implicit meaning.
### database:
- a collection of related data
### DBMS:
- a software package/system to facilitates the creation and maintenance of a computerized database.
### database system:
- The DBMS software together with the data itself.
### database catalog:
- stores the description of a particular database(data structure, types, and constraints)
### program-data independence:
- allows changing data structures and storage organization without having to change the DBMS access programs.
### user view:
- the way in which the database appears to a particular user is called user view
### DBA(database administrator):
- a person who is responsible for authorizing access to the database, coordinating an monitoring its use, and acquiring software and hardware resources as needed.
### end user:
- the people who want to access the database for different purposes like, querying, updating, and generating reports.
### canned transaction:
- standardized queries and updates on the database using carefully programmed and tested programs.
### deductive database system:
- a database system that can make deductions based on rules and facts stored in the database.
### persistent object:
- An object that is stored in such a way that it survives that termination of the DBMS program is persistent.
### meta-data:
- allows the DBMS software to work with different database applications.
### transaction-processing application:
- a logical unit of database.


# 2.1
### data model
- a collection of concepts that can be used to described the structure of a database.
### database schema
- the overall design/description of the database.
### database state
- the data in the database at a particular moment in time.
### internal schema
- at the internal level to describe physical storage structures and access paths.
### conceptual schema
- at the conceptual level to describe the structure and constraints for the whole database for a community of users.
### external schema
- at the external level to describe the various user views.
### data independence
- the capacity to change the schema at one level of a database system without having to change the schema at the next higher level.
### DDL(data definition language)
- it is used by the DBA and developers to create a database with specific schemas.
### DML(data manipulation language)
- it is used to perform data manipulations such as data addition, data retrieval, data insertion, data deletion and data modification.
### SDL(storage definition language)
- it is used to spent the internal schema of the database.
### VDL(view definition language)
- it us used to specify user view and their mappings to conceptual schema.
### query language
- it is a high level data manipulation language used in a stand alone interactive manner.
### host language
- it is the computer language, which either high level are low level data manipulation language commands embedded in a general-pure pose programming language.
### data sublanguage
- the data manipulation language embedded in the last language.
### database utility
- software modules that help the DBA to manage a database system.
### catalog
- a complete description of the database structure and constraints .
### client/server architecture
- it is a database architecture in which the system functionality is distributed between two types of modules.
    - the client module consists of application programs to provide a user interface to access the database.
    - the server module landless data storage, access, and search.
### three-tier architecture
1. presentation tier:
    - occupies the top level and displays information related to services available on a website.
    - This tier communicates with other tiers by sending results to the browser and other tiers in the network.
2. application tier:
    - also called the middle tier, logic tier, business logic tier, this tier is pulled from the presentation tier.
    - it controls application functionality by performing detailed processing.
3. data tier:
    - houses database servers where information is stored and retrieved.
    - data in this tier is kept independent of application servers or business logic.
### n-tier-architecture
- also called multi-tier architecture because the software is engineered to have the processing, data management, and presentation functions physically and logically separated.
- that means that these different functions are hosted on several machines or clusters, ensuring that services are provided without resources being shared and, as such, these services are delivered at top capacity.


# 3.3
### entity
### attribute
### attribute value
### relationship instance
### composite attribute
### multivalued attribute
### derived attribute
### complex attribute
### key attribute
### value set


# 5.1
### domain
### attribute
### n-tuple
### relation schema
### relation state
### degree of a relation
### relational database schema
### relational database state
