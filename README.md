TerminalBench

A collection of realistic system failure scenarios designed for debugging practice and engineering evaluation.

Overview

TerminalBench is a structured set of backend and infrastructure-style failure cases that simulate real-world production issues.

Each scenario is designed to reflect how systems actually fail in production environments, including:

service outages
performance degradation
configuration issues
dependency failures

The goal is to practice identifying root causes using logs, system behavior, and configuration data.

Project Purpose

Modern engineering systems fail in complex and non-obvious ways. This project is designed to simulate those failures in a controlled environment to help improve:

debugging skills
system reasoning
infrastructure understanding
incident analysis

It can also be used as a lightweight evaluation dataset for reasoning-based systems.

Structure
scenarios/
├── scenario_01_api_failure/
├── scenario_02_db_timeout/
└── scenario_03_env_misconfig/

Each scenario contains:

README.md → problem description
logs.txt → system logs and error traces
solution.md → root cause and fix explanation
(optional) config files or environment data
Scenario Types
1. API Failure

A service failure caused by a missing or unreachable dependency.

2. Database Timeout

Performance degradation due to resource constraints or pooling issues.

3. Environment Misconfiguration

System failure caused by missing or incorrect environment variables.

How to Use
Open any scenario folder
Read the scenario description
Analyze logs and configuration
Identify the root cause
Compare with solution.md
Key Learning Outcome

This project focuses on improving the ability to:

interpret system logs
diagnose production issues
understand infrastructure dependencies
reason through multi-step failures
Notes

These scenarios are intentionally simplified but designed to reflect real-world engineering failure patterns.

END OF README