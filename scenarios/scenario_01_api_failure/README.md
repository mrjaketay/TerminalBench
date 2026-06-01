Scenario 01: API Service Failure
Overview

A backend API service that was previously working is now failing unexpectedly in production. Users are reporting intermittent errors when trying to access data from the system.

The service appears to start normally, but requests fail shortly after deployment.

Symptoms
API returns 500 Internal Server Error
Some requests timeout completely
Service restarts do not resolve the issue
No recent code changes were documented
Your Task

Investigate the logs and configuration to determine:

What is causing the failure
Why the system starts but fails under usage
How to fix the issue