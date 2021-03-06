# Real-Time Data Feed from Python to Supabase

## Prepare Environment & Dependencies

Dependency management with Poetry: https://python-poetry.org/docs/#installation

1. Inside your desired python environment (`^3.9`) run:

    ```bash
    python3.9 -m venv venv
    pip install poetry  # install the poetry package manager
    poetry install      # use poetry to install dependencies
    ```

2. Place the `.env` file in the projects root directory (same level as `run.py`). The `.env` file should look like this:

    ```bash
    SUPABASE_URL="..."
    SUPABASE_PUBLIC="..."
    SUPABASE_TABLE="air-quality-timeseries"

    USER_EMAIL="..."
    USER_PASSWORD="..."
    ```

3. Push data to the rt-feed - example in `run.py`:

    ```python
    DB.insert_data({...});
    ```
