# AJ-Davis2

A powerful task automation tool that streamlines your workflow by connecting GitHub issues, pull requests, and CI/CD pipelines.

## Installation

```bash
npm install aj-davis2
```

## Usage

1. **Initialize your project** - Run `aj-davis2 init` to set up configuration files
2. **Connect your repositories** - Link your GitHub repositories using your personal access token (see [GitHub Personal Access Tokens](https://docs.github.com/en/authentication/keeping-your-data-secure/managing-your-personal-access-tokens))
3. **Define workflows** - Create workflow rules in your `aj-davis2.config.json` file
4. **Execute automation** - Use `aj-davis2 run` to start automating your tasks

## Options

| Option | Type | Default | Description |
|--------|------|---------|-------------|
| `verbose` | boolean | `false` | Enable detailed logging output |
| `config` | string | `./aj-davis2.config.json` | Path to configuration file |
| `timeout` | number | `30000` | Request timeout in milliseconds |
| `retries` | number | `3` | Number of retry attempts on failure |
| `dry-run` | boolean | `false` | Preview changes without applying them |
| `token` | string | `process.env.GITHUB_TOKEN` | GitHub personal access token |

## Architecture

![AJ-Davis2 Architecture Diagram](https://user-images.githubusercontent.com/1234567/example-diagram.png "System architecture showing how AJ-Davis2 connects GitHub, workflows, and automation tasks")
