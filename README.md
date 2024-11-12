# GitHub Actions CI/CD Practice Repository

This repository contains various GitHub Actions workflows to practice Continuous Integration (CI) techniques. Each workflow showcases different triggers, strategies, and setups commonly used in CI/CD pipelines.

## Workflows Overview

1. **Playwright Tests - Simple Sharding** (`sharding.yml`): 
   - Runs Playwright tests in parallel using sharding.
   - Merges reports into an HTML report, available in GitHub Actions Artifacts.

2. **API Triggered Workflow** (`api-workflow.yml`): 
   - Triggered by API call or manual dispatch.
   - Contains two jobs: `run-tests` and `final-job`, showcasing job dependencies.

3. **Manual Trigger Workflow** (`manual-triger.yml`): 
   - Runs jobs triggered by manual dispatch.

4. **Master Branch Workflow** (`master-workflow.yml`): 
   - Triggers automatically on pushes to the `main` branch.

5. **Matrix Strategy Workflow** (`matrix.yml`): 
   - Runs Playwright tests across multiple Node.js versions with matrix strategy for compatibility checks.

6. **Scheduled Workflow** (`sheduler-cron.yml`): 
   - Executes at regular intervals using cron, supporting routine testing.

7. **Simple Jobs Workflow** (`simple-jobs.yml`): 
   - Demonstrates sequential job dependencies.

## Requirements
- Node.js and Git (for local setup and testing).

## Usage

- **Triggering Workflows**: Trigger workflows manually, via API, on branch push, or by schedule.
- **Viewing Reports**: Find test reports and logs in the GitHub Actions Artifacts section.

Each workflow highlights different CI/CD practices to automate testing and ensure code quality. See `.github/workflows` for full configurations and further details.
