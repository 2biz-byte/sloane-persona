# AI Persona References

Each repository this AI Persona depends on is linked here as a **git submodule**, so a
coding agent can clone the persona and reach every pipeline, list, and Operator command
repository from one place.

```bash
git submodule update --init
```

Private submodules need credentials that can read the linked repositories.

## Linked repositories

| Kind | Name | Path | Branch |
|------|------|------|--------|
| command | Renew a household service (personal) | `references/commands/6a90198a9334d064acf7c5de` | `main` |
| pipeline | service-renewal-workflow | `references/pipelines/pl-e13390d8fa6d` | `main` |

`registry.json` holds the same mapping as plain JSON, readable without fetching the
submodules. It is generated — edit the persona's pipelines, lists, and commands in the
product instead of editing this folder by hand.
