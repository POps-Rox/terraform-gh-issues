<!-- BADGES:START -->
[![CI](https://github.com/POps-Rox/tf-gh-issues/actions/workflows/ci.yml/badge.svg)](https://github.com/POps-Rox/tf-gh-issues/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/POps-Rox/tf-gh-issues/pulls)
[![Maintained](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/POps-Rox/tf-gh-issues/graphs/commit-activity)
[![Terraform](https://img.shields.io/badge/Terraform-%3E%3D1.5-623CE4.svg?logo=terraform)](https://www.terraform.io)
<!-- BADGES:END -->

# Terraform GitHub Issues ![release](https://img.shields.io/github/v/release/azurenoops/terraform-github-issues)![job runs](https://img.shields.io/docker/pulls/azurenoops/terraform-github-issues?label=job%20runs)

## Usage

This GitHub Action creates a new issue based on an issue template file. 

[GitHub Actions](https://github.com/features/actions) are a way to make automated workflows that trigger when events occur on your GitHub repository, using a YAML file that lives in your repo.
These actions can be used to easily perform [Terraform](https://www.terraform.io/) tasks as part of your workflow.

Here's an example workflow that creates a new issue any time you push a commit:
    
    ```yaml 
    name: Create issue
    on: [push]

    jobs:
      build:
        runs-on: ubuntu-latest
        steps:
        - uses: actions/checkout@v2
        - name: Create issue
          uses: azurenoops/terraform-github-issues@v1        
    ```

## License

The scripts and documentation in this project are released under the [MIT License](LICENSE)

## Contributions

Contributions are welcome! See [Contributor's Guide](CONTRIBUTING.md)

