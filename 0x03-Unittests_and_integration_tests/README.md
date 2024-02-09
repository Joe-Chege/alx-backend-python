# alx-backend-python - Unittests and Integration Tests

## Curriculum: Unittests and Integration Tests


## Project Overview
This project focuses on implementing unit tests and integration tests for various functions and classes in the `alx-backend-python` repository. The tasks involve parameterizing tests, mocking HTTP calls, understanding and applying memoization, and conducting integration tests using fixtures.

## Learning Objectives
Upon completing this project, you should be able to:

- Explain the difference between unit and integration tests.
- Understand common testing patterns such as mocking, parametrizations, and fixtures.

## Requirements
- All files will be interpreted/compiled on Ubuntu 18.04 LTS using Python 3 (version 3.7).
- All files should end with a new line.
- The first line of all files should be exactly `#!/usr/bin/env python3`.
- A `README.md` file, at the root of the project folder, is mandatory.
- Code should use the `pycodestyle` style (version 2.5).
- All files must be executable.
- All modules should have documentation.
- All classes should have documentation.
- All functions (inside and outside a class) should have documentation.
- A documentation is not a simple word; it’s a real sentence explaining the purpose of the module, class, or method.
- All functions and coroutines must be type-annotated.

## Required Files
1. `utils.py` (or download)
2. `client.py` (or download)
3. `fixtures.py` (or download)

## Tasks

### Task 0: Parameterize a Unit Test
- Familiarize yourself with the `utils.access_nested_map` function.
- Create a `TestAccessNestedMap` class that inherits from `unittest.TestCase`.
- Implement the `TestAccessNestedMap.test_access_nested_map` method and use `@parameterized.expand` to test the function for specific inputs.

### Task 1: Parameterize a Unit Test (Exception)
- Implement `TestAccessNestedMap.test_access_nested_map_exception` using `assertRaises` to test that a `KeyError` is raised for specific inputs.

### Task 2: Mock HTTP Calls
- Familiarize yourself with the `utils.get_json` function.
- Define the `TestGetJson(unittest.TestCase)` class and implement the `TestGetJson.test_get_json` method to test `utils.get_json`.
- Use `unittest.mock.patch` to patch `requests.get` and ensure it returns the expected result.

### Task 3: Parameterize and Patch
- Read about memoization and familiarize yourself with the `utils.memoize` decorator.
- Implement the `TestMemoize(unittest.TestCase)` class with a `test_memoize` method, using `@patch` to mock a method and test memoization.

### Task 4: Parameterize and Patch as Decorators
- Familiarize yourself with the `client.GithubOrgClient` class.
- Declare the `TestGithubOrgClient(unittest.TestCase)` class and implement the `test_org` method.
- Use `@patch` as a decorator to ensure `get_json` is called once with the expected argument.

### Task 5: Mocking a Property
- Implement the `test_public_repos_url` method to unit-test `GithubOrgClient._public_repos_url`.
- Use `patch` as a context manager to mock `GithubOrgClient.org` and test the result of `_public_repos_url`.

### Task 6: More Patching
- Implement `TestGithubOrgClient.test_public_repos` to unit-test `GithubOrgClient.public_repos`.
- Use `@patch` as a decorator to mock `get_json` and use `patch` as a context manager to mock `GithubOrgClient._public_repos_url`.

### Task 7: Parameterize
- Implement `TestGithubOrgClient.test_has_license` to unit-test `GithubOrgClient.has_license`.
- Parametrize the test with specific inputs and expected returned values.

### Task 8: Integration Test: Fixtures
- Create the `TestIntegrationGithubOrgClient(unittest.TestCase)` class.
- Implement `setUpClass` and `tearDownClass` methods, using `@parameterized_class` to parameterize the class with fixtures.
- Mock `requests.get` to return example payloads found in the fixtures.

## Copyright
© 2024 ALX, All rights reserved.