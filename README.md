# Data Warehouse Project

This project is a data warehouse setup using dbt (data build tool). It includes configurations, models, macros, and tests to transform raw data into meaningful insights.

## Prerequisites

- Docker
- Python 3.7
- dbt

## Setup

1. **Clone the repository:**

   ```sh
   git clone https://github.com/hanifahrizqy/Project2
   cd project2
   ```

2. **Build and start the Docker containers:**

   ```sh
   docker-compose up --build
   ```

3. **Set up the Python virtual environment:**

   ```sh
   cd dbt/devEnv
   python3.7 -m venv .
   source bin/activate
   pip install -r requirements.txt
   ```

4. **Configure dbt:**
   - Update the `profiles.yml` file located at [`project2/dwh/profiles.yml`] with your database credentials.
   - Ensure the `dbt_project.yml` file is correctly configured.

## Running dbt

1. **Activate the virtual environment:**

   ```sh
   source dbt/devEnv/bin/activate
   ```

2. **Run dbt commands:**
   - **Initialize a new dbt project:**
     ```sh
     dbt init
     ```
   - **Run dbt models:**
     ```sh
     dbt run
     ```
   - **Debug dbt models:**
     ```sh
     dbt debug
     ```
3. **Generate and serve the documentation:**
   ```sh
   dbt docs generate
   ```
4. **Serve the documentation:**
   ```sh
   dbt docs serve
   ```
5. **Deactivate the virtual environment:**

   ```sh
    deactivate
   ```

