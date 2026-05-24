# Virtual_env

cd backend

# 1. Initialize the modern virtual environment
uv venv

# 2. Fast-install all requirements 
uv pip install -r requirements.txt

# 3. Create the database schema tables
.venv\Scripts\python -m flask create-db

# 4. Seed the sandbox B2B records
.venv\Scripts\python -m flask seed

# 5. Start the backend developer server
.venv\Scripts\python run.py

# 1. Activate the environment
source .venv/Scripts/activate

# 2. Run the commands directly
flask create-db
flask seed
python run.py
