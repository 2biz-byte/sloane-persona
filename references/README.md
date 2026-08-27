# AI Persona References

This folder is a **depth-1 composition workspace**. Every linked repository is a git
submodule of this Persona — never a submodule of another submodule.

```bash
git submodule update --init
```

## Portable bundle (`registry.json`)

Import materializes one Workflow per distinct command workflowRef, plus exactly one Pipeline and one List.

| Kind | Resource key | Name | Path | Branch |
|---|---|---|---|---|
| list *(portable)* | `list.sloane.service-renewals` | service-renewals | `references/lists/list-sloane-service-renewals` | `main` |
| pipeline *(portable)* | `pipeline.sloane.service-renewal-workflow` | service-renewal-workflow | `references/pipelines/pipeline-sloane-service-renewal-workflow` | `main` |
| workflow *(portable)* | `workflow.sloane.renew-a-household-service-personal` | Renew a household service (personal) | `references/workflows/workflow-sloane-renew-a-household-service-personal` | `main` |

## Authoring graph (`workspace.json`)

Generated. Do not edit by hand. Extra workflows and team agents live here so one clone
reaches the whole graph. They are **not** cross-environment portable imports.

| Kind | Id | Name | Path | Branch |
|---|---|---|---|---|
| — | _No extra workspace repositories._ | | | |

Commit content in each child repository first, then **publish the workspace** so this
Persona lock (gitlinks, fingerprints, and `workspace.json`) advances in one root commit.
