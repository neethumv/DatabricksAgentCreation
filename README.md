# Databricks Agent Creation – Mosaic AI Agent Framework

## Overview

Built a Multi-Tool HR Agent using Databricks Mosaic AI Agent Framework that demonstrates tool calling, agent evaluation, tracing, deployment, and monitoring.

## Scenarios Completed

### 1. First Tool-Calling Agent
- Created a bonus calculation tool using a Unity Catalog Function.
- Built an agent that decides when to call the tool versus answering directly.

### 2. Multi-Tool Composition
- Integrated two tools:
  - Bonus Calculation Tool
  - Databricks Genie
- Supported single-tool and multi-tool queries.

### 3. Evaluation Before Trust
- Created an evaluation dataset with 10 test questions.
- Evaluated agent responses.
- Identified failures for edge cases such as:
  - `100k`
  - `one hundred thousand`

### 4. Tracing and Root Cause Analysis
- Intentionally broke the Genie tool using an invalid Space ID.
- Used MLflow Tracing to identify the failed tool invocation.
- Determined the root cause without reviewing the entire codebase.

### 5. Deployment and Monitoring
- Registered the agent as an MLflow model.
- Deployed it to a Databricks Model Serving Endpoint.
- Sent live requests and monitored:
  - Request logs
  - Endpoint status
  - Latency and performance metrics

## Technologies Used

- Databricks Mosaic AI Agent Framework
- Databricks Genie
- Unity Catalog Functions
- MLflow Tracing
- MLflow Model Registry
- Databricks Model Serving
- Python

## Outcome

Successfully built, evaluated, debugged, deployed, and monitored a production-style multi-tool HR agent using Databricks services.
