# Unity Common Services Testing

## Introduction
This document provides an overview of the testing architecture for Unity Common Services (Unity-CS). It encompasses continuous testing concepts such as testing across the software development lifecycle as well as automated execution of tests through automation.

---

## Testing Categories

The below list of test categories are included in our testing setup. Further details are provided below.

<!-- ADD / MODIFY BELOW CATEGORIES TO AS NEEDED -->
- [x] **Static Code Analysis:** checks code for syntax, style, vulnerabilities, and bugs
- [x] **Unit Tests:** tests functions or components to verify that they perform as intended

### Static Code Analysis Tests

- Location: `.github/`
- Purpose: To ensure code adheres to coding standards and guidelines and to identify potential vulnerabilities early.
- Running Tests:
  - Manually:
    1. Navigate to the `.github` directory.
    2. Run the static code analysis tool defined in the project configuration.
    3. Review the results displayed in the command line or tool interface.
  - Automatically:
    - Frequency:
      - Triggered by code changes or pull requests.
      - Runs on every commit to the repository.
    - Results Location: `GitHub Actions` or the configured CI/CD pipeline interface.
- Contributing:
  - Framework Used: SonarQube or similar static analysis tools.
  - Tips:
    - Ensure that all code follows the documented coding standards.
    - Regularly review and address any issues flagged by the analysis tool.

### Unit Tests

- Location: `tests/unit/`
- Purpose: To verify individual functions or components perform as expected.
- Running Tests:
  - Manually:
    1. Navigate to the `tests/unit/` directory.
    2. Execute the unit tests using the testing framework command, e.g., `pytest`.
    3. View results in the command line interface.
  - Automatically:
    - Frequency:
      - Triggered by commits or pull requests.
      - Runs in the CI/CD pipeline for every code update.
    - Results Location: `GitHub Actions` or the configured CI/CD pipeline interface.
- Contributing:
  - Framework Used: PyTest, JUnit, or other unit testing frameworks.
  - Tips:
    - Write tests for each non-trivial function or method.
    - Include tests for edge cases, error conditions, and invalid inputs.

