# IDS706-Assignment-1

[![Python tests](https://github.com/yihanc09/IDS706-Assignment-1/actions/workflows/test.yml/badge.svg)](https://github.com/yihanc09/IDS706-Assignment-1/actions/workflows/test.yml)

# My Python Project

This project asks for a name and prints a welcome message for the Data Engineering course.

# Project Structure
IDS706-Assignment-1/
├── .github/
│   └── workflows/
│       └── test.yml
├── src/
│   └── main.py
├── tests/
│   └── test_main.py
├── Dockerfile
├── Makefile
├── README.md
└── requirements.txt

## Setup
Create a virtual environment:
```
python -m venv .venv
source .venv/bin/activate      # Mac / Linux
.venv\Scripts\activate          # Windows
pip install -r requirements.txt
```
Install the required dependencies:
`
make install
`
The project uses the following development dependencies:
- `pytest` for automated testing
- `black` for code formatting
- `ruff` for linting

## Run tests
`
python -m pytest
`
## Example
Enter your name when prompted:

Yihan, welcome to the Data Engineering course.





# IDS 706 Assignment 1

This project is a simple Python application created for IDS 706: Data Engineering Systems at Duke University. The application asks the user for their name and prints a personalized welcome message for the Data Engineering course.

The project demonstrates a basic development workflow using Python, including virtual environments, automated testing, Makefile commands, Docker, code formatting and linting, and GitHub Actions.

## Project Structure

```text
IDS706-Assignment-1/
├── .github/
│   └── workflows/
│       └── test.yml
├── src/
│   └── main.py
├── tests/
│   └── test_main.py
├── Dockerfile
├── Makefile
├── README.md
└── requirements.txt
```

## Setup

Create a virtual environment:

```bash
python3 -m venv .venv
```

Activate the virtual environment on Mac/Linux:

```bash
source .venv/bin/activate
```

Install the required dependencies:

```bash
make install
```

The project uses the following development dependencies:

* `pytest` for automated testing
* `black` for code formatting
* `ruff` for linting

## Run the Application

Run the application with:

```bash
make run
```

The program asks the user to enter a name and then generates a welcome message.

### Example

```text
Enter your name: Yihan
Yihan, welcome to the Data Engineering course.
```

## Run Tests

Run the test suite with:

```bash
make test
```

The tests use `pytest` to verify that the main functionality produces the expected output.

## Code Formatting and Linting

This project uses Black and Ruff to maintain consistent and clean Python code.

Format the Python files with:

```bash
make format
```

Check the code with Ruff:

```bash
make lint
```


## Available Make Commands

| Command             | Description                   |
| ------------------- | ----------------------------- |
| `make install`      | Install project dependencies  |
| `make test`         | Run the pytest test suite     |
| `make run`          | Run the Python application    |
| `make format`       | Format Python code with Black |
| `make lint`         | Check Python code with Ruff   |
| `make docker-build` | Build the Docker image        |
| `make docker-run`   | Run the application in Docker |
| `make docker-test`  | Run tests inside Docker       |
| `make clean`        | Remove generated cache files  |
