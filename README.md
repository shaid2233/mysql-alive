# Database Health Check Service

This is a lightweight Flask-based HTTP service that checks the availability of a MySQL database. The service exposes an endpoint at `/is-db-alive`, which returns the database connection status.

## Features
- **Health Check Endpoint**: Verifies if the MySQL database is accessible.
- **Environment Configurable**: Database connection settings are passed through environment variables.

## Requirements
- Python 3.7 or higher
- MySQL server
- Dependencies listed in `requirements.txt`

# Configuration
Set the following environment variables to configure the database connection:

|Variable |	Default | Value |	Description|
--------------------------------------
|DB_HOST |	localhost |	Hostname of the MySQL server.|
|DB_PORT |	3306 | Port number for MySQL. |
|DB_USER |	root | MySQL username. |
|DB_PASSWORD |	"" | MySQL password. |
|DB_NAME |	test	| Name of the database to check.|

## Example:

```bash
export DB_HOST="localhost"
export DB_PORT="3306"
export DB_USER="root"
export DB_PASSWORD="password"
export DB_NAME="test"
```
