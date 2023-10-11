<p align="center">
    <a href="https://github.com/TypedDevs/bashunit/actions/workflows/tests.yml">
        <img src="https://github.com/TypedDevs/bashunit/actions/workflows/tests.yml/badge.svg" alt="Tests">
    </a>
    <a href="https://github.com/TypedDevs/bashunit/actions/workflows/static_analysis.yml">
        <img src="https://github.com/TypedDevs/bashunit/actions/workflows/static_analysis.yml/badge.svg" alt="Static analysis">
    </a>
    <a href="https://github.com/TypedDevs/bashunit/actions/workflows/deploy-docs.yml">
        <img src="https://github.com/TypedDevs/bashunit/actions/workflows/deploy-docs.yml/badge.svg" alt="Docs deployment">
    </a>
<a href="https://github.com/TypedDevs/bashunit/actions/workflows/linter.yml">
        <img src="https://github.com/TypedDevs/bashunit/actions/workflows/linter.yml/badge.svg" alt="Editorconfig checker">
    </a>
    <a href="https://github.com/TypedDevs/bashunit/blob/main/LICENSE">
        <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="MIT Software License">
    </a>
</p>
<br>
<p align="center">
    <picture>
        <source media="(prefers-color-scheme: dark)" srcset="docs/public/logo_name_dark.svg">
        <img alt="bashunit" src="docs/public/logo_name.svg" width="400">
    </picture>
</p>

<h1 align="center">A simple testing library for bash scripts</h1>

<p align="center">
    Test your bash scripts in the fastest and simplest way, discover the most modern bash testing library.
</p>

## Documentation

You can find the complete documentation for **bashunit** online, including installation instructions and the various features it provides, in the [official bashunit documentation](https://bashunit.typeddevs.com).

## Contribute

You are welcome to contribute reporting issues, sharing ideas,
or with your pull requests.

Make sure to read our [contribution guide](.github/CONTRIBUTING.md) where you will find, among other things, how to set up your environment with the various tools we use to develop this library.

## Contributors

<p align="center">
    <img src="https://contributors.nn.ci/api?repo=TypedDevs/bashunit" alt="Contributors list" />
</p>


This is a **proof of concept** PR of a simple data provider for test functions.

The main idea is having an "annotation" just before the test function where we can specify the data provider function as this:

```
# provider function_data_provider
function test_my_function_test() {
  ...
}
```

This function_data_provider can return a single or a list of values. Those are two examples of data provider:

```
function provider_test_data_array() {
  local data=("one" "two" "three")  
  echo "${data[@]}" 
}

function provider_test_data_single_value() {
  echo "one" 
}
```

The test function will receive the data provided in the $1 parameter.