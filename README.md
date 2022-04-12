# Install Helm Docs
Github Action to install Helm Docs. The Github action can enable CI to run helm docs and support multiple flows around docs automation.

## Inputs

Name | Description | Required | Default
--- | --- | --- | ---
`version` | Helm Docs version to install | `true` | `1.7.0`

## Example Usage

```
jobs:
  install-helm-docs:
    runs-on: ubuntu-latest
    steps:
    - name: Install Helm Docs
        uses: envoy/install-helm-docs@v1.0.0
        with:
          # Helm Docs Version to install (Mandatory)
          version: 1.7.0
```

## Local Development

Refer [this](https://docs.github.com/en/actions/creating-actions/creating-a-composite-action) document to learn more on how to create custom Github Actions (composite)
