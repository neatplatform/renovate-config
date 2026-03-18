# renovate-config

Shareable [Renovate](https://www.renovatebot.com/) configuration presets for all repositories.

This repository provides standardized, opinionated dependency update configurations for different languages and projects,
which individual repositories can extend and override as needed.

## Quick Start

### Reuse Config

**General-purpose**

```json
{
  "extends": [
    "github>neatplatform/renovate-config"
  ]
}
```

**Go**

```json
{
  "extends": [
    "github>neatplatform/renovate-config:go"
  ]
}
```

**JavaScript**

```json
{
  "extends": [
    "github>neatplatform/renovate-config:javascript"
  ]
}
```

### Reuse Workflow

```yaml
name: Renovate
on: [push]

jobs:
  call:
    name: Call
    uses: neatplatform/renovate-config/.github/workflows/reusable-renovate.yml@main
```

## Resources

  - **Renovate**
    - [Presets](https://docs.renovatebot.com/key-concepts/presets/)
    - [Shareable Config Presets](https://docs.renovatebot.com/config-presets/)
      - [Default Presets](https://docs.renovatebot.com/presets-default/)
      - [Full Config Presets](https://docs.renovatebot.com/presets-config/)
      - [Schedule Presets](https://docs.renovatebot.com/presets-schedule/)
      - [Security Presets](https://docs.renovatebot.com/presets-security/)
    - [Configuration Options](https://docs.renovatebot.com/configuration-options/)
    - [String Pattern Matching - Regex or Glob](https://docs.renovatebot.com/string-pattern-matching/)
    - [JSON Schema](https://docs.renovatebot.com/json-schema/)
  - **Reusable Workflows**
    - [Reuse workflows](https://docs.github.com/en/actions/how-tos/reuse-automations/reuse-workflows)
    - [Reusing workflow configurations](https://docs.github.com/en/actions/reference/workflows-and-actions/reusing-workflow-configurations)
