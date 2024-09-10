# Notes API Testing with Postman

This repository contains automated API tests for the Notes API, implemented using Postman. The tests are orchestrated with a GitHub Actions pipeline but can also be executed locally without needing to run a GitHub Actions job during API test case creation.

[![Automated API tests using Postman CLI](https://github.com/SvitlanaKoshchii/postman-notes-api-testing/actions/workflows/postman-workflow.yml/badge.svg)](https://github.com/SvitlanaKoshchii/postman-notes-api-testing/actions/workflows/postman-workflow.yml)

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

