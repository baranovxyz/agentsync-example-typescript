# AgentSync Example: TypeScript

Example AgentSync library demonstrating TypeScript best practices, testing guidelines, and common commands.

> Note: Any secrets in `mcp.json` use placeholder tokens like `{GITHUB_TOKEN}`. Do not paste real secrets into this repo. Configure real values via your local environment or user-level config only.

## Installation

**Option 1: Via GitHub** (recommended for private/custom libraries)
```json
{
  "extends": ["github:baranovxyz/agentsync-example-typescript"],
  "tools": ["cursor", "claude"]
}
```

**Option 2: Via npm** (future support in v0.4.0+)
```json
{
  "extends": ["npm:@agentsync/example-typescript"],
  "tools": ["cursor", "claude"]
}
```

Then sync:
```bash
agentsync sync
```

## What's Included

### Rules (3)
- `typescript-strict.md` - TypeScript strict mode settings
- `testing.md` - Testing guidelines and coverage targets
- `api-design.md` - API design best practices

### Commands (3)
- `commit.md` - Generate conventional commit messages
- `review.md` - Code review checklist
- `test.md` - Run tests with coverage

### Recommended MCPs (2)
- `context7` - Up-to-date documentation lookup
- `github` - GitHub API access

## Files Created

After sync, files appear as:

```
.cursor/rules/
├── typescript-example:typescript-strict.mdc
├── typescript-example:testing.mdc
└── typescript-example:api-design.mdc

.cursor/commands/
├── typescript-example:commit.md
├── typescript-example:review.md
└── typescript-example:test.md
```

## Namespace

Default namespace: `typescript-example` (from library.json)

Override in your config:
```json
{
  "extends": [{
    "source": "github:baranovxyz/agentsync-example-typescript",
    "namespace": "ts"
  }]
}
```

## License

MIT
