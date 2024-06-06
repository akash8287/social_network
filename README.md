# Social Networking Application API

This is a Django Rest Framework-based API for a social networking application.

## Features

- User Signup and Login
- Search Users by Email and Name
- Send, Accept, and Reject Friend Requests
- List Friends
- List Pending Friend Requests
- Limit Friend Requests to 3 per Minute

## Installation

### Prerequisites

- Docker
- Docker Compose

### Steps

1. **Clone the repository:**
    ```sh
    git clone <repository_link>
    cd <repository_directory>
    ```

2. **Build and run the Docker containers:**
    ```sh
    docker-compose up --build
    ```

3. **Apply the database migrations:**
    ```sh
    docker-compose exec web python manage.py migrate
    ```

4. **Create a superuser (optional):**
    ```sh
    docker-compose exec web python manage.py createsuperuser
    ```

5. **Access the application:**
    - The application should now be running at `http://localhost:8000/`.

### Importing Postman Collection

1. **Download the Postman collection JSON file:** Ensure you have the JSON file for the Postman collection saved on your local machine.

2. **Open Postman:** Launch the Postman application on your computer.

3. **Import the collection:**
    - Click on the `Import` button located in the top-left corner of the Postman interface.
    - Select the `Choose Files` button.
    - Navigate to the location where you saved the JSON file, select it, and click `Open`.

4. **Confirm import:** The Postman collection should now appear in your Postman under the `Collections` tab, allowing you to test the API endpoints easily.



