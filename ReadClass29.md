## Database Engine Room is wrapped around
Room is wrapped around a SQLite database engine. Since SQLite is a small, standalone database engine, no additional server processes are needed. It is appropriate for embedded systems and mobile applications.


## Is this a good choice?
The suitability of Room for your needs will depend on them. Room is a good choice if you require a compact, user-friendly database solution for your embedded system or mobile app. However, you might want to think about using a different database engine if you require a more robust or scalable database solution.
Comparisons between JPA and Room

## Do Rooms have any similarities to JPA?
The object-relational mapping (ORM) frameworks Room and JPA are both used. You can easily persist and retrieve data by mapping your Java objects to database tables thanks to ORMs. But there are some significant distinctions between JPA and Room.

A lightweight ORM framework made specifically for mobile applications is called Room. Although it has fewer features than JPA, it is easier to use. A more robust ORM framework that supports a wider variety of applications is JPA. It is more difficult to use than Room, though.


## Describe DAO.
DAO (Data Access Object) is a design pattern that provides an abstraction layer between your application code and the underlying database. This makes it possible to consolidate database usage logic into a single class, making code easier to maintain and update. 
 
 The DAO generally has the following responsibilities: 
 
- Connect to  database 
- Running SQL queries 
- Associate database results with Java objects 
- Closing the database connection