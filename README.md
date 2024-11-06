# TaskNest - A Simple Task Managemnet API
TaskNest is a simple, yet powerful API built with Python, Flask, and MongoDB, designed to manage tasks efficiently. This project demonstrates various modern development practices, including Test-Driven Development (TDD), Continuous Integration (CI), and Continuous Deployment (CD). Developed based on the course "Do Zero ao Deploy" by Cássio Botaro, this API allows users to create and retrieve tasks with ease.

Key Features:
-Python 3.6: Written using Python 3.6, ensuring compatibility with the latest features.
-Pipenv or Virtualenv: Easily manage project dependencies with Pipenv or Virtualenv.
-Test-Driven Development (TDD): Developed with PyTest for testing endpoints, ensuring code quality.
-Flask Framework: A lightweight framework for building APIs quickly and efficiently.
-Continuous Integration & Deployment: Integrated with Travis CI for seamless automated testing and Heroku for easy deployment.
-MongoDB Persistence: Tasks are stored and managed in a MongoDB database, providing flexibility and scalability.

Installation & Setup
-Prerequisites:
Python 3.6: Install Python 3.6 for the correct functioning of the application.
MongoDB: Install MongoDB and ensure the MongoDB service is running on your machine.
-Setting Up the Environment:
Using Pipenv: If you're using Pipenv to manage dependencies:
bash
Copy code
$ pipenv install
$ pipenv shell
Using Virtualenv: If you're using Virtualenv, activate the environment and install the dependencies:
bash
Copy code
$ source YOUR_ENVIRONMENT_DIRECTORY/bin/activate
$ pip install -r requirements.pip
Running the Application:
After installing dependencies, run the API:

bash
Copy code
$ python tasknest.py
This will start the server at http://127.0.0.1:5000/.

API Endpoints:
GET /tasks: Fetch all tasks stored in the database.
POST /tasks: Create a new task with a title and description.
Example:
GET /tasks:

bash
Copy code
$ http http://127.0.0.1:5000/tasks
Returns all tasks in the database.

POST /tasks:

bash
Copy code
$ http POST http://127.0.0.1:5000/tasks title="New Task" description="Task Description"
Creates a new task in the database.

Testing:
To run tests, make sure development dependencies are installed:

bash
Copy code
$ pipenv install --dev
Then, run the tests with:

bash
Copy code
$ python -m pytest
