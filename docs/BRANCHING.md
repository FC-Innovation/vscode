# vscode — Git branching

**Updated:** 2026-06-22

Future Capital **FC-Innovation** standard — two long-lived branches only:

| Branch | Role | GitHub default |
|--------|------|----------------|
| **`dev`** | Integration; clone lands here | **Yes** |
| **`prod`** | Production (not `main`); deploy / release from here | No |

No **`main`** branch. Developers: feature → PR → **`dev`**. DevOps / seniors: **`dev` → `prod`**, then sync **`prod` → `dev`**.
