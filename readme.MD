# FastAPI Sample Project for DigitalOcean Deployment

This is a sample FastAPI project created to test deployment on DigitalOcean with CI/CD pipelines. The project contains two simple routes: a root route and an item route.

## Routes

- **GET /**  
  Returns a JSON response:

  ```json
  { "Hello": "World" }
  ```

- **GET /items/{item_id}**
  Takes an `item_id` (integer) as a path parameter and an optional query parameter `q` (string).
  Returns a JSON response:
  ```json
  { "item_id": item_id, "q": q }
  ```

## Project Structure

```
├── main.py              # Main FastAPI app with routes
├── requirements.txt    # Python package dependencies
├── README.md           # Project documentation (this file)
```

## Requirements

- Python 3.7+
- FastAPI

## Installation and Setup

Follow the steps below to set up and run the project locally:

1. **Clone the repository:**

   ```bash
   git clone git@github.com:hironate/fast-api-test-project.git
   cd fast-api-test-project
   ```

2. **Create a virtual environment (optional but recommended):**

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. **Install the required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Running the Application

To run the FastAPI app locally using FastAPI CLI, execute the following command:

```bash
fastapi dev run.py
```

To run the FastAPI app on production using FastAPI CLI, execute the following command:

```bash
fastapi run
```

This will start the development server with auto-reloading enabled. You should see output like:

```
INFO:     Serving at http://127.0.0.1:8000
INFO:     API docs: http://0.0.0.0:8000/docs
INFO:     Running in production mode, for development use:

fastapi dev
```

Now, you can visit the following endpoints in your browser or API testing tool (e.g., Postman):

- Root: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
- Item: [http://127.0.0.1:8000/items/1?q=test](http://127.0.0.1:8000/items/1?q=test)

## License

This project is licensed under the MIT License - see the LICENSE file for details.

```

### Key Steps Included:
- Cloning the repo
- Setting up a virtual environment
- Installing dependencies
- Running the FastAPI server locally
- Explaining the available routes and example usage
```
