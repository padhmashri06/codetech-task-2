NAME: PADHMASHRI KA
COMPANY: CODTECH IT SOLUTION 
ID:CT08FTN
DOMAIN: FULL STACK WEB DEVELOPER
DURATION DATE:DEC TO JAN 20
Overview of the Recipe Sharing Platform Project

This project is a Recipe Sharing Platform where users can:

Register and log in to the platform.

Share recipes, including a title, ingredients, and instructions.

View, update, and delete their own recipes.

Save and manage their recipe collection in a user-friendly environment.





The application is built using Vue.js for the frontend (UI) and Express.js for the backend (server-side). The JWT (JSON Web Tokens) authentication mechanism is used to handle user authentication and secure the API endpoints.

Key Features of the Project:

1. User Authentication:

Registration: Users can create an account by providing their username, email, and password. The password is hashed for security using bcrypt.

Login: Users log in with their email and password. Upon successful login, they receive a JWT token that is used to authenticate their future requests.

Token-based Authentication: The server verifies the JWT token on requests that require user authentication (such as adding, updating, or deleting recipes).



2. Recipe Management:

Create Recipes: Authenticated users can add new recipes with a title, ingredients, and instructions.

View Recipes: All authenticated users can view a list of recipes, including those created by themselves and others.

Update Recipes: Users can update their own recipes.

Delete Recipes: Users can delete their own recipes.



3. Frontend (Vue.js):

The frontend is a simple single-page application (SPA) that allows users to interact with the platform by:

Registering or logging in through forms.

Adding, viewing, updating, and deleting recipes.

Displaying a list of recipes in a user-friendly format.




4. Backend (Express.js):

The backend handles requests such as:

User registration and login.

CRUD (Create, Read, Update, Delete) operations for recipes.

JWT-based authentication for secure access to recipe management.


The server also serves the Vue.js frontend as static files using Express's static file serving capabilities.



5. In-memory Storage:

Users and recipes are stored in memory as arrays for simplicity. In a production environment, you'd want to replace this with a database (e.g., MongoDB, PostgreSQL).



6. Basic Validation:

Simple validation is performed, such as checking if the user exists during login and ensuring that the required fields are provided for recipes.




How the Application Works:

1. User Registration:

The user provides a username, email, and password.

The backend hashes the password and stores the user details in memory.

After successful registration, the user is prompted to log in.



2. User Login:

The user enters their email and password.

If the credentials are correct, the backend generates a JWT token, which is sent to the frontend.

This token is stored on the frontend (typically in local storage or session storage) and used in subsequent requests to access protected API routes.



3. Managing Recipes:

Authenticated users can create new recipes by providing a title, ingredients, and instructions.

Recipes are stored in memory and are associated with the user who created them.

The user can view all recipes, update their own recipes, and delete them if needed.




Technologies Used:

1. Vue.js (Frontend):

Vue.js is used for creating the user interface and handling user interactions.

The frontend interacts with the backend through HTTP requests to create, read, update, and delete recipes.



2. Express.js (Backend):

Express.js is used to build the server and handle API requests.

The server uses JWT for secure authentication.

It also serves static files from the public directory, which contains the Vue.js frontend.



3. JWT (JSON Web Token):

JWT is used for user authentication. After logging in, the user gets a token that must be included in the headers of future API request…



![Screenshot (57)](https://github.com/user-attachments/assets/0811ed3e-3368-4a19-bef6-d25dc36e1109)
![Screenshot (58)](https://github.com/user-attachments/assets/0dc3cbc2-f789-416f-a059-41b988fdadd5)

