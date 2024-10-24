# fix-dubious-ownership-action

[![CI](https://github.com/datalens-tech/fix-dubious-ownership-action/workflows/Check%20PR/badge.svg)](https://github.com/datalens-tech/fix-dubious-ownership-action/actions?query=workflow%3A%22%22Check+PR%22%22)
[![GitHub Marketplace](https://img.shields.io/badge/Marketplace-fix-dubious-ownership-action-blue.svg)](https://github.com/marketplace/actions/fix-dubious-ownership-action)

Action to solve "detected dubious ownership" [error](https://github.com/actions/runner-images/issues/6775)

## Usage

### Example

```yaml
jobs:
  fix-dubious-ownership-action:
    steps:
      - name: fix-dubious-ownership-action
        uses: datalens-tech/fix-dubious-ownership-action@v1
```

### Action Inputs

| Name               | Description             | Default                             |
| ------------------ | ----------------------- | ----------------------------------- |
| `github_repo_name` | GitHub Repository Name. | ${{ github.event.repository.name }} |

### Action Outputs

None

## Development

### Global dependencies

- [Taskfile](https://taskfile.dev/installation/)
- [nvm](https://github.com/nvm-sh/nvm?tab=readme-ov-file#install--update-script)

### Taskfile commands

For all commands see [Taskfile](Taskfile.yaml) or `task --list-all`.

## License

[MIT](LICENSE)
