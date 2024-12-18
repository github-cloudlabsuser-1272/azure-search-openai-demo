# Backend Folder Documentation

## Overview
This document provides an overview of the backend folder structure and its components for the Azure Search OpenAI Demo application.

## Folder Structure
```
backend/
├── app/
│   ├── __init__.py
│   ├── main.py
│   ├── config.py
│   ├── models/
│   │   ├── __init__.py
│   │   ├── model.py
│   ├── services/
│   │   ├── __init__.py
│   │   ├── search_service.py
│   │   ├── openai_service.py
│   ├── utils/
│   │   ├── __init__.py
│   │   ├── helpers.py
│   ├── tests/
│   │   ├── __init__.py
│   │   ├── test_main.py
│   │   ├── test_services.py
├── requirements.txt
├── README.md
```

## Components

### `app/`
This is the main application directory containing the core components of the backend.

#### `__init__.py`
Initializes the app module.

#### `main.py`
The entry point of the application. It sets up the FastAPI app and includes route definitions.

#### `config.py`
Contains configuration settings for the application, such as environment variables and constants.

### `models/`
Contains the data models used in the application.

#### `model.py`
Defines the data models and schemas used by the application.

### `services/`
Contains the service layer of the application, which includes business logic and interactions with external services.

#### `search_service.py`
Implements the logic for interacting with Azure Search.

#### `openai_service.py`
Implements the logic for interacting with OpenAI's API.

### `utils/`
Contains utility functions and helpers used throughout the application.

#### `helpers.py`
Provides helper functions for common tasks.

### `tests/`
Contains unit tests for the application.

#### `test_main.py`
Tests for the main application logic.

#### `test_services.py`
Tests for the service layer.

## Dependencies
The `requirements.txt` file lists all the dependencies required for the backend application.

## Getting Started
To set up the backend application, follow these steps:

1. Clone the repository.
2. Navigate to the `backend` directory.
3. Install the dependencies:
    ```sh
    pip install -r requirements.txt
    ```
4. Run the application:
    ```sh
    uvicorn app.main:app --reload
    ```

## Contributing
Contributions are welcome! Please submit a pull request or open an issue to discuss any changes.

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.