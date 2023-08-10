# Todo App API

This Django project implements a Todo app API, demonstrating CRUD (Create, Read, Update, Delete) operations for managing tasks.

## Features

- Create tasks with a title, description, and completion status.
- Read a list of all tasks or retrieve a specific task.
- Update task details, including title, description, and completion status.
- Delete tasks to remove them from the database.

## Endpoints

The following API endpoints are available for managing tasks:

- `GET /api/tasks/`: Retrieve a list of all tasks.
- `POST /api/tasks/`: Create a new task.
- `GET /api/tasks/{task_id}/`: Retrieve details of a specific task.
- `PUT /api/tasks/{task_id}/`: Update details of a specific task.
- `DELETE /api/tasks/{task_id}/`: Delete a specific task.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/Homeroida/todo-API.git
   cd todo-API
2. Download django usig pip
   ```bash
   sudo apt install python3-pip -y
   pip install django 
3. Install project dependencies:
   ```bash
   pip install -r requirements.txt
4. Apply database migrations:
   ``` bash
   python3 manage.py makemigrations
5. Start the development server:
   ```bash
   python3 manage.py migrate
6. Create SuperUser:
   ```bash
   python3 manage.py createsuperuser
7. Run Server:
   ```bash
   python3 manage.py runserver
   
   

## Usage
You can use tools like curl or API testing tools like Postman to interact with the Todo app API. Here are a few examples:

1. Retrieve all tasks:
   ```bash
   curl http://localhost:8000/api/tasks/
2. Create new task:
   ```bash
   curl -X POST -H "Content-Type: application/json" -d '{"title": "Finish README", "description": "Write the README file for the project"}' http://localhost:8000/api/tasks/
3. Update a Task:
   ```bash
   curl -X PUT -H "Content-Type: application/json" -d '{"title": "Updated Title", "completed": true}' http://localhost:8000/api/tasks/{task_id}/ 
4. Delete a Task:
   ```bash
   curl -X DELETE http://localhost:8000/api/tasks/{task_id}/

## Contact

If you have any questions, suggestions, or feedback regarding the Todo App API, feel free to reach out to us:

- **Maintainer Name:** Zurab Tchanishvili
- **Maintainer Email:** chanishvili@gmail.com

You can also open an issue in the repository if you encounter any problems or want to discuss improvements.

We appreciate your interest in the project and look forward to hearing from you!
   
