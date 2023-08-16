# Task Hunter backend
Django project for Task Hunter backend.

## Pre-requisites
- PostgreSQL database server
- Python 3.10

## Setup
### Dependencies
Activate venv.
```bash
python3.10 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install pip-tools
```

Install for development.
```bash
pip-sync requirements-dev.txt
```

Install for production [optional].
```bash
pip-sync
```

### Modifying dependencies [optional]
Modify the list of dependencies in `requirements.in` or `requirements-dev.in`. Then update requirements.txt and requirements-dev.txt with `pip-compile`.
```bash
pip-compile -o requirements.txt pyproject.toml
pip-compile --extra dev -o requirements-dev.txt pyproject.toml
```

### Database

Run PostgreSQL server.

Copy `.env.example` to `.env` and fill in the values.

```bash
cp .env.example .env
```