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
- an entity is an object with independent physical(car, home, person) or conceptual (company, university course) existence in the real world.
### attribute
- each real world entity has certain properties that represent its significance in real world or describes it. these properties of an entity are known as attribute.
- 例えば車の内容（モデル、ブランド、色、費用等）
### attribute value　属性値
- Associated with each real world entity are certain attributes that describe that entity. Value of these attributes for any entity is called attribute value.
- ex) attribute of car entity can be Red.
### relationship instance
- it is instance that associates an entity from an entity type to another entity of another entity type, in order to establish a relationship among various participating entity types.
- attributeをシェアしている。
### composite attribute
- an attribute that can be divided into smaller subparts, which represent more basic attributes with independent meanings, is called a composite attribute.
- 例えば携帯電話だとエリアコード、ナンバーなどに再分割できる。
### multivalued attribute
- for a real world entity, an attribute may have more than one value.
- 携帯電話が人というentityにあるとして、その人が２、３台持っている可能性がある。
### derived attribute　派生attribute
- for a real world entity, an attribute may have value that is independent of other attributes or can not be derived from other attributes; such as attributes are called as stored attributes. there are also certain attributes, whose value can be derived using value of other attributes; such attributes are known as derived attributes.
- 年齢は誕生日からのderived attribute.
### complex attribute
- composite and multivalued attribute can be nested arbitrarily. Arbitrary nesting can be represented by grouping components of a composite attribute between parenthesis () and separating the components with comas, and by displaying multivalued attributes between braces {}. such attributes are called composite attribute
### key attribute
- each real world entity is unique in itself. there are certain attributes whose value is different for all similar type of entities. These attributes are called Key attributes. These attributes are used to specify uniqueness constraint in a relation.
- 例えば、車体ナンバーと登録番号は重なることがない。
### value set(domain)
- for an attribute of a real world entity, there is a range of values from which a particular attribute can take value.
- 定義域　例えば、社員コード、名前、入社日という属性があるときに、社員コードは半角数字による0000~9999、名前の定義域は全角文字列、入社日の定義域は西暦年号での年月日という感じ。

# 5.1 they apply to the relational model of data.
### domain
- it is a set of atomic(indivisible) values that can appear in a particular column in a relational schema. a common method of specifying domain is to specify a data type(integer, char, float, etc...) from which the data values forming a domain can be drawn.
- relational schema called Student. the name of the student must be a char string. so we can say domain of name is char string.
### attribute
- an attribute is a role played by some domain in the relational schema.
- In relational schema Student, Name can be one of the attributes of the relation.
### n-tuple
- if a relational schema consists of n Attributes, i.e., degree of relational schema is n, then n-tuple is an ordered list of n values that represent a tuple, t=; where each value vi, 1 <= i <= n, is a element of dom(Ai) or is a special NULL value.
### relation schema
- it is but collection of attributes that define facts and relation between a real world entity and name.
### relation state
- collection of various tuples, R(A1, A2, ..., An)
### degree of a relation
- the degree of a relation is the number of attributes n of its relational schema.
### relational database schema
- A relational database schema S is a set of relation schemas, S = {R1, R2,..., Rn} and a set of integrity constraints IC.
### relational database state
- A relational database state is DB of S is set of relation states, DB = {r1, r2,..., rn}, such that each ri is state of Ri and such that the ri relation states satisfy the integrity constraints specified in IC.
