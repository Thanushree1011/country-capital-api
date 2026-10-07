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

## Git Commands:

# Assignment 1: Create the project
mkdir my-exciting-project
cd my-exciting-project
git init
git branch -M main

# Create files and add initial content
touch README.md
git add .
git commit -m "Initial commit"

# Connect to GitHub
git remote add origin https://github.com/Thanushree1011/my-exciting-project.git
git push -u origin main

# Create and switch to development branch
git switch -c develop
git push -u origin develop

# Create feature branches and make changes
git switch -c feature/initial-setup
git add .
git commit -m "Add initial setup"
git push -u origin feature/initial-setup

git switch develop
git switch -c feature/enhancement-1
git add .
git commit -m "Add enhancement one"
git push -u origin feature/enhancement-1

git switch develop
git switch -c feature/enhancement-2
git add .
git commit -m "Add enhancement two"
git push -u origin feature/enhancement-2

# Merge feature branches
git switch develop
git merge feature/initial-setup
git merge feature/enhancement-1
git merge feature/enhancement-2
git push origin develop

# View branches and commit history
git branch -a
git log --oneline --all --graph --decorate
git status

# Assignment 2: Clone the repository
git clone https://github.com/Thanushree1011/country-capital-api.git
cd country-capital-api

# Check repository
git status
git branch -a
git remote -v

# Create the feature branch
git switch -c feature/FEAPP-420-whatsapp-notifications

# Stage and commit changes
git status
git add whatsapp_notifications.md
git diff --cached
git commit -m "docs: add WhatsApp notification feature notes"

# Push the feature branch
git push --set-upstream origin feature/FEAPP-420-whatsapp-notifications

# After creating and merging the pull request on GitHub
git switch main
git pull origin main
git status
ls -la
git log --oneline --all --graph --decorate
