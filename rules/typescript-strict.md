# TypeScript Strict Mode

Always use TypeScript strict mode with these settings:

```json
{
  "compilerOptions": {
    "strict": true,
    "noUncheckedIndexedAccess": true,
    "noImplicitOverride": true
  }
}
```

- Never use `any` - use `unknown` instead
- Prefer `interface` over `type` for objects
- Use const assertions for literals
