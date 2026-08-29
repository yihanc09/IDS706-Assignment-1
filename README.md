# IDS706-Assignment-1

[![Python tests](https://github.com/yihanc09/IDS706-Assignment-1/actions/workflows/test.yml/badge.svg)](https://github.com/yihanc09/IDS706-Assignment-1/actions/workflows/test.yml)

# My Python Project

This project asks for a name and prints a welcome message for the Data Engineering course.

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
