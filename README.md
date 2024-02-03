This Postman collection is to test the bdo_demo_backend of Nikos Mpakaris 

This Collection can run automatically. 
It is important, that the PostgreSQL Database is empty. 

Step 1: 
Start Backend incl. new PostgreSQL DB in Docker of Backend. 

Step 2: 
Make sure DB is empty 

Step 3: 
Run the API Tests of this collection in Postman 

  Stage 1: Genereal CRUD Operations for Tasks & Users
  It will create, update and soft delete 1 User --> User 1 
  It will create, update and soft delete 1 Task assigned to User 1--> Task 1

  Stage 2: Soft Delete of User 2 --> Will automatically Soft Delete all Tasks assigned to this User 
  It will create 1 User --> User 2
  It will create 2 Tasks assigned to User 2 --> Task 2 and Task 3
  It will soft delete User 2 --> Task 2 and Task 3 will automatically be markes as deleted in DB 
  
