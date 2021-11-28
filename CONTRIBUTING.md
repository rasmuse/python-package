# Install in dev mode

1. Create a virtual environment

```
python -m venv .venv
```

2. Activate the venv.

On Linux:
```
python3 -m venv .venv
. .venv/bin/activate
```

On Windows:
```
.venv\Scripts\activate
```

3. Install dev dependencies and then the package in editable mode:
```
pip install -r requirements/dev.txt && pip install -e .
```

# Run tests

To run the test suite, do

```
pytest
```

To run the whole tox testing party, do

```
tox
```
