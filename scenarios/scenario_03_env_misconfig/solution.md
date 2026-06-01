Root Cause

The application is missing critical environment variables in production:

JWT_SECRET is not set
API_KEY for external service is missing

As a result:

authentication tokens cannot be validated
external API requests fail
Why it works locally

The application likely works locally because:

local .env file exists
default fallback values or cached credentials are present
development environment is more permissive
Fix
Add missing environment variables:
JWT_SECRET
API_KEY
Ensure production environment loads .env or secure secret store
Remove insecure fallback defaults
Restart application after config update
Key Lesson

Environment differences between local and production are a major cause of real-world system failures. Proper configuration management is critical.