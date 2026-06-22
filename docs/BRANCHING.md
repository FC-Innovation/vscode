# vscode — Git branching

**Updated:** 2026-06-22

Future Capital **FC-Innovation** standard — two long-lived branches only:

| Branch | Role | GitHub default |
|--------|------|----------------|
| **`dev`** | Integration; clone lands here | **Yes** |
| **`prod`** | Production (not `main`); deploy / release from here | No |

No **`main`** branch. Developers: feature → PR → **`dev`**. DevOps / seniors: **`dev` → `prod`**, then sync **`prod` → `dev`**.

```bash
git clone https://github.com/FC-Innovation/vscode.git
cd vscode
git pull origin dev
git checkout -b feature/my-change dev
# PR → dev

git checkout prod && git pull origin prod   # release / deploy
```
