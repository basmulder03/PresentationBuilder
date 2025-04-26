# 📦 My Electron App

A modern **Electron** application built with **TypeScript** and managed with **pnpm**.  
Designed for scalability, developer productivity, and clean workflows.

---

## 🚀 Features

- ⚡ Electron 27
- 🧹 TypeScript 5
- 🛠 pnpm workspace management
- 🧪 GitHub Actions CI for build and commit linting
- 🔥 Husky pre-commit hooks
- 📝 Conventional Commits enforced
- ✅ Protected `master` branch with PR templates

---

## 🛠 Project Setup

### Install dependencies

```bash
pnpm install
```

Run in development mode

```bash
pnpm start
```

- Builds the TypeScript source
- Launches the Electron app

Build TypeScript manually

```bash
pnpm run build
```

Outputs compiled files into `/dist/.`

📂 Project Structure

```
my-electron-app/
├── .husky/ # Git hooks (commit-msg hook)
├── .github/                    
│ ├── workflows/ # GitHub Actions (build and commit linting)
│ └── pull_request_template.md # Default PR checklist
├── dist/ # Compiled JavaScript (output)
├── src/                         
│ ├── main.ts # Electron main process
│ ├── preload.ts # Preload script
│ └── index.html # HTML UI
├── package.json # Project metadata and scripts
├── pnpm-lock.yaml # pnpm dependency lockfile
├── tsconfig.json # TypeScript config
├── .gitignore # Ignored files
├── .gitattributes # Line-ending and file handling
├── commitlint.config.js # Conventional commit rules
└── README.md # Project documentation
```

### 🛡 Git Workflow

1. All development happens through feature branches.
2. Open a Pull Request against master when ready.
3. PRs must:
    1. Pass build check (GitHub Actions)
    2. Pass commit message linting (GitHub Actions)
    3. Be reviewed if branch protection requires it.

### 📝 Commit Message Guidelines

This project follows the Conventional Commits standard.
Examples:

- `feat: add user authentication`
- `fix: correct crash on login`
- `docs: update API documentation`
- `refactor: simplify main window logic`

### 🔥 How to Start Contributing

1. Fork this repo
2. Clone your fork
3. Create a new branch:
   `git checkout -b feat/my-feature`
4. Make your changes
5. Commit with a valid Conventional Commit message
6. Open a Pull Request to main

## 📜 License

MIT

✨ Extra
This project was bootstrapped manually without templates, ensuring clean architecture for production Electron apps.