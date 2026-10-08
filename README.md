# keel plugin: Jira

Bring Jira issues into Tasks and keep their status in step with your flows.

> **Status: planned.** The code still lives in [keel-v2](https://github.com/MiladNalbandi/keel-v2). It moves here step by step, as
> [the plugin plan](https://github.com/MiladNalbandi/keel-v2/tree/main/docs/plugins) says. There is nothing to install yet.

| | |
| --- | --- |
| id | `jira` |
| needs | keel core (plugin SDK 1), Tasks |
| works with | — |
| parts | api · web · migrations |
| trust level | runs code in keel |

**What it adds to keel**

- Jira connection
- Jira sync for Tasks

**Where the code is today (keel-v2)**

- `keel.api.jira` (api)
- `keel.api.tasks.JiraSync` (api)
- `web/src/components/JiraCard.tsx`

## Layout

```
keel-plugin.yml   the manifest
api/              Kotlin, a thin Spring Boot jar
web/              React pages and slots (an ES module)
migrations/       its own database tables (own Flyway history)
```

## Install

When it is released: in keel, **Control › Plugins › Marketplace › Jira › Install**. keel checks the file's
signature, shows what the plugin may do, and asks you before it installs.

## License

MIT
