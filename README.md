# Country Capital API

## What is this?

Country Capital API is a Python-based API that returns the name of a country when a capital city is provided.

The API is built using **Flask** and is served using the **Uvicorn** ASGI server.

A microservice endpoint is also available for other projects in the organization to consume:

`https://example.com/country-capital/<query-params>`

## Prerequisites

Before running the API locally, make sure you have:

* Python installed
* `pip` installed
* Required Python dependencies installed

## Local Setup

### 1. Clone the repository

```bash
git clone <repository-url>
cd country-capital-api
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate the virtual environment.

**Windows:**

```bash
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Running the API

The API is served using Uvicorn.

Start the application using the project's configured application entry point:

```bash
uvicorn <module>:<application> --reload
```

The API will then be available locally for development and testing.

## API Usage

The API accepts a capital city as input and returns the corresponding country.

The organization-wide microservice endpoint can be accessed using:

```text
https://example.com/country-capital/<query-params>
```

Replace `<query-params>` with the appropriate capital-city query parameters.
