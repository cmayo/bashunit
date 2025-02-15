# Changelog

## [Unreleased](https://github.com/TypedDevs/bashunit/compare/0.6.0...main)

## [0.6.0](https://github.com/TypedDevs/bashunit/compare/0.5.0...0.6.0) - 2023-09-19

- Added `assertExitCode`
- Added `assertSuccessfulCode`
- Added `assertGeneralError`
- Added `assertCommandNotFound`
- Added `assertArrayContains`
- Added `assertArrayNotContains`
- Added `assertEmpty`
- Added `assertNotEmpty`
- Added `setUp`, `setUpBeforeScript`, `tearDown` and `tearDownAfterScript` function execution before and/or after test and/or script execution
- Improved the readability of the assert by using guard clause
- Update documentation
- Add support for the static analysis on macOS
- Fix bug with watcher for the development of bashunit
- Fix error on count assertions
- Added pipeline to add contributors to the readme
- Added documentation with VitePress
- Stop runner when found duplicate test functions

## [0.5.0](https://github.com/TypedDevs/bashunit/compare/0.4.0...0.5.0) - 2023-09-10

- Added logo
- Added `assertNotEquals`
- Added `assertMatches`
- Added `assertNotMatches`
- Added `make test/watch` to run your test every second
- Added time taken to run the test in ms (only to Linux)
- Simplified assertions over test results
- Added acceptance test to the library
- Added pre-commit to the project
- Allow parallel tests to run base on a .env configuration enabled by default
- Added static analysis tools to the deployment pipelines
- New summary output

## [0.4.0](https://github.com/TypedDevs/bashunit/compare/0.3.0...0.4.0) - 2023-09-08

- Better output colors and symbols
- Add option `--filter` to `./bashunit` script
    - Trigger tests filtered by name
- Change the output styles
    - Emojis
    - Colors
    - Bolds
- Added count to all test

## [0.3.0](https://github.com/TypedDevs/bashunit/compare/0.2.0...0.3.0) - 2023-09-07

- Added `assertContains`
- Added `assertNotContains`
- Display Passed tests in green, and Failed tests in red
- Avoid stop running tests after a failing one test

## [0.2.0](https://github.com/TypedDevs/bashunit/compare/0.1.0...0.2.0) - 2023-09-05

- Fix keeping in memory test func after running them
- Create a `./bashunit` entry point
- Change ROOT_DIR to BASH_UNIT_ROOT_DIR
- Allow writing test with camelCase as well
- Allow running example log_test from anywhere

## [0.1.0](https://github.com/TypedDevs/bashunit/compare/27269c2...0.1.0) - 2023-09-04

- Added `assertEquals` function
