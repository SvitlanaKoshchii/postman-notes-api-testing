# Notes API Testing with Postman

This repository contains automated API tests for the Notes API, implemented using Postman. The tests are orchestrated with a GitHub Actions pipeline but can also be executed locally without needing to run a GitHub Actions job during API test case creation.

[![Run API Tests via Postman CLI](https://github.com/SvitlanaKoshchii/postman-notes-api-testing/actions/workflows/run-api-tests-postman-cli.yml/badge.svg)](https://github.com/SvitlanaKoshchii/postman-notes-api-testing/actions/workflows/run-api-tests-postman-cli.yml)

[![Run API Tests via Newman](https://github.com/SvitlanaKoshchii/postman-notes-api-testing/actions/workflows/run-api-tests-newman.yml/badge.svg)](https://github.com/SvitlanaKoshchii/postman-notes-api-testing/actions/workflows/run-api-tests-newman.yml)


## What is this repository for?

The repository includes:
- **Postman Collection and Environment Files**: For testing the Notes API server.
- **GitHub Actions Workflow File**: Runs the test cases automatically in a pipeline.

## Prerequisites

To run the tests, you'll need:
- Postman installed.
- A clone of this repository (`git clone https://github.com/SvitlanaKoshchii/postman-notes-api-testing.git`).
- The Postman collection and environment imported into your Postman workspace.

## What is tested?

This collection is dedicated to testing the Notes API, which provides endpoints for managing both users and notes within the system. It serves as a comprehensive framework to validate the API’s functionality, structure, and performance. The tests ensure secure and reliable interactions between the client and server, maintaining data integrity.

**Key Features Tested:**
- **Health Check**: Verifies the API's availability and operational status.
- **User Management**: Tests endpoints for:
  - User creation (registration).
  - Login and logout.
  - Profile updates.
  - Account deletion.
- **Notes Management**: Validates the full lifecycle of notes:
  - Creating, retrieving, updating, and deleting notes.
- **Response Validation**: Ensures response codes, headers, and content meet expected standards.
- **Performance Metrics**: Measures response times to ensure the API meets performance requirements.

The collection supports both functional and non-functional testing, providing a robust framework to ensure the reliability, efficiency, and security of the Notes API.

## Executing Tests Locally

### Manual Execution:
1. Open Postman.
2. Select the **Notes API** collection.
3. Ensure the environment **Notes API Environment** is selected.
4. Click on **Run** to execute the tests.
5. Select the **Run Manually** option.
6. Press the **Run Notes API** button.

## GitHub Actions Workflows

This repository includes two GitHub Actions workflows that automate the execution of API tests:

1. **Run API Tests via Postman CLI**: This workflow uses the Postman CLI to execute the Postman collection directly. It is designed for environments where Postman CLI is preferred or where additional Postman-specific features are needed during test execution.

2. **Run API Tests via Newman**: This workflow uses Newman, the command-line tool for running Postman collections, to execute the tests. It is optimized for environments where lightweight command-line execution is preferred and provides a streamlined way to integrate Postman tests into CI/CD pipelines. This workflow also includes the generation of an HTML report, which is saved as an artifact for review.

Both workflows automatically execute the API test cases defined in the Postman collection whenever changes are made to the repository.

### Key Features:
- **Run API Tests via Postman CLI**: Provides detailed output from the Postman CLI with Postman-specific features.
- **Run API Tests via Newman**: A lightweight and efficient method for running Postman collections in CI environments. Includes generation of an HTML report, available as an artifact for detailed analysis.
