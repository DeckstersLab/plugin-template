# plugin-template
Template repo for new plugins

## Local Development Setup
Follow the below steps to get set up with your local development environment in order to contribute to this repo..

### Install dev dependencies:
To set up all necessary tools (including pre-commit hooks), from the root directory of this repo, run the following
command:
```bash
make
```

### Detect secrets
If detect secrets fails dont forget to run a scan and audit any detected secrets. Don't commit real secrets to source control!

```bash
detect-secrets scan > .secrets.baseline
```

```bash
detect-secrets audit .secrets.baseline
```
