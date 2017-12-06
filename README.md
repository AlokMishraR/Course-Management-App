Developed a standalone end-to-end Course management spring application having complete database backed REST API using Spring Boot. 

In this project, i have created some RESTful endpoints for course management system by developing business controllers, services and 
repository classes using spring boot. 

Topic and Cource are two models or database entities used in the project. A topic can have multiple courses, hence maintained the 
foreign-key relationship between the entities using JPA.

I have used embedded apache derby as database and implemented the data layer using Spring Data JPA

This app will support all CRUD operations like GET, POST, PUT and DELETE over topic and course entities. For instance:

GET request to  API localhost:8080/topics will return all the topics from the database in json format.
GET request to  API localhost:8080/topics/topicId will return a topic of given id from the database
POST request with a topic payload to API localhost:8080/topics will insert the topic into the database
PUT request with topic payload to API localhost:8080/topics/topicId will update a topic into the database
DELETE request to API localhost:8080/topics/topidId will delete a topic from the database

GET request to API localhost:8080/topics/topicId/courses will return all the courses of give topic in json format.
GET request to API localhost:8080/topics/topicId/courses/courseId will return a course of a topic by courseId.
POST request with topic payload to API localhost:8080/topics/topicId/courses will insert a course in the topic.
PUT request with course payload to API localhost:8080/topics/topicId/courses/courseId will update a course in the topic
DELETE request to API localhost:8080/topics/topidId/courses/courseId - to delete a course from the database.


