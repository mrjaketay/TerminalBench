Root Cause

The API is failing because the database service is not running or not reachable.

The logs show repeated connection failures to 127.0.0.1:5432, which indicates:

The database server is down
OR it is not properly configured or started
Why the system “starts” but fails later

The API service starts successfully because:

It does not require a live database connection to boot
It only fails when actual requests hit the database layer
Fix
Start the database service (e.g. PostgreSQL)
Verify correct host and port configuration
Ensure environment variables are correctly set:
DB_HOST
DB_PORT
DB_USER
DB_PASSWORD
Key Lesson

System health at startup does not guarantee runtime stability.
Dependencies must be verified during both initialization and request handling.