# AJ-Davis2

A lightweight automation tool for managing GitHub workflows, issue tracking, and CI/CD task execution.

## Install

```bash
npm install aj-davis2
```

## Usage

1. Initialize your project by running `aj-davis2 init` to create the default configuration files.
2. Connect your repositories and GitHub account using a personal access token as described in the [GitHub Personal Access Tokens documentation](https://docs.github.com/en/authentication/keeping-your-data-secure/managing-your-personal-access-tokens).
3. Define workflow rules in your configuration file to automate tasks such as triage, review checks, and deployment steps.
4. Run the automation with `aj-davis2 run` to start processing the configured workflow.

## Options

| Option | Type | Default | Description |
|--------|------|---------|-------------|
| `verbose` | boolean | `false` | Enable detailed logging output for troubleshooting. |
| `config` | string | `./aj-davis2.config.json` | Path to the project configuration file. |
| `timeout` | number | `30000` | Request timeout in milliseconds. |
| `retries` | number | `3` | Number of retry attempts after a failed task. |
| `dry-run` | boolean | `false` | Preview workflow actions without applying changes. |
| `token` | string | `process.env.GITHUB_TOKEN` | GitHub personal access token used for authentication. |

## Architecture

![AJ-Davis2 workflow architecture diagram showing how repository data, automation rules, and CI/CD pipelines connect](https://user-images.githubusercontent.com/1234567/example-diagram.png)