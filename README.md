# Hackathon-2025
All about our project idea and visualizing it through diagrams and other stuffs.
### Team Name
404_Brains

### Project Idea
A digital platform to connect all categories people with healthcare professionals easily & updatedly.

###  Tech Stack
Frontend: React  
Backend: Node.js (Express)  
Database: MySQL  

### High-Level Design (HLD)
https://app.eraser.io/workspace/6XbvHSNentqzrsL9OVV6?origin=share

### API Specification

We are developing our backend using **Node.js (Express)** and **MySQL**.  
Below are the main API endpoints that will be implemented:

1. **POST /register**
   - Description: Used to create a new user account.
   - Input (from frontend):
     ```json
     {
       "name": "Rahima",
       "phone": "01700000000",
       "password": "123456"
     }
     ```
   - Output (response):
     ```json
     {
       "message": "User registered successfully"
     }
     ```

2. **POST /login**
   - Description: Used for user login and authentication.
   - Input:
     ```json
     {
       "phone": "01700000000",
       "password": "123456"
     }
     ```
   - Output:
     ```json
     {
       "message": "Login successful",
       "token": "abc123xyz"
     }
     ```

3. **GET /health-tips**
   - Description: Returns a list of general health advice for users.
   - Output:
     ```json
     [
       "Drink clean water",
       "Wash hands before eating",
       "Eat fresh vegetables daily"
     ]
     ```


### Postman Collection
We are testing all backend APIs using **Postman**.
The following endpoints are included for testing:

1. `POST /register` → To create a new user  
2. `POST /login` → To verify user credentials  
3. `GET /health-tips` → To fetch health-related information  

Each API request is tested with valid and invalid inputs to ensure proper responses.

*(The Postman JSON file will be uploaded once all endpoints are ready.)*

### Docker
 Docker will not be used for this submission. The backend runs locally using Node.js and MySQL.
