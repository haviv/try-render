# Simple Hello World REST API

This is a simple Flask REST API that exposes a GET `/hello` endpoint which returns a "Hello, World!" message in JSON format.

## Setup

1. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

## Running the Application Locally

Run the application with:
```bash
python app.py
```

The server will start on `http://localhost:5001`

## Testing the API Locally

You can test the API using curl:
```bash
curl http://localhost:5001/hello
```

Expected response:
```json
{
    "message": "Hello, World!"
}
```

## Deploying to Render

1. Create a new account on [Render](https://render.com) if you haven't already
2. Fork or push this repository to your GitHub account
3. In Render dashboard:
   - Click "New +"
   - Select "Web Service"
   - Connect your GitHub repository
   - Render will automatically detect the configuration from `render.yaml`
4. Click "Create Web Service"

The deployment will start automatically. Once completed, you can access your API at the URL provided by Render. 