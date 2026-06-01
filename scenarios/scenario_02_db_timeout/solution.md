Root Cause

The database connection pool is too small (max=2), causing requests to queue when traffic increases.

This leads to:

connection starvation
request queuing delays
eventual timeouts
Why the system does not crash

The system is still running because:

application server is healthy
only database access layer is bottlenecked
no fatal exceptions occur
Fix
Increase database connection pool size
Optimize slow queries (if applicable)
Add query indexing if needed
Implement proper request timeout handling
Monitor DB performance under load
Key Lesson

Performance issues often appear as “system slowness” rather than errors.
Connection limits and resource pooling are critical in backend systems.