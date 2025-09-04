# 🧠 INH Packages Repository

This repository contains the **official package index** for [INH CLI](https://github.com/inhtam/inh).
All installable packages are listed in [`data.json`](https://raw.githubusercontent.com/inhtam/packages/main/data.json).

---
## 🔹 Badges

![GitHub Repo stars](https://img.shields.io/github/stars/inhtam/packages)
![GitHub forks](https://img.shields.io/github/forks/inhtam/packages)
![GitHub issues](https://img.shields.io/github/issues/inhtam/packages)
![License](https://img.shields.io/github/license/inhtam/packages)


---

## 📦 How It Works

* The CLI fetches the `data.json` file to discover available packages.
* Each entry in `data.json` describes one package.
* When users run `inh install <name>`, the package source is downloaded from GitHub using the info in `data.json`.

---

## 📑 Example Entry

A package entry in `data.json` looks like this:

```json
{
  "name": "sayidisi",
  "version": "1.0.0",
  "repo": "https://github.com/aardaakpinar/sayidisi",
  "branch": "main",
  "path": "cli",
  "main": "main.js"
}
```

---

## 🔹 Required Fields

Every package **must** include the following fields:

| Field     | Description                                      |
| --------- | ------------------------------------------------ |
| `name`    | Package name (used in CLI: `inh install <name>`) |
| `version` | Version number (semver format)                   |
| `repo`    | GitHub repository URL                            |
| `branch`  | Branch name (e.g., `main`)                       |
| `path`    | Path to the package folder inside the repo       |
| `main`    | Entry file to execute (e.g., `index.js`)         |

Optional fields like `description` or `author` can be added, but are not required.

---

## 🔧 Contributing a Package

1. **Fork this repository.**
2. **Edit `data.json`** and add a new object for your package with all required fields.
3. **Commit your changes** and push them to your fork.
4. **Open a Pull Request** to the `main` branch of this repo.
5. A maintainer will review and approve your contribution. ✅

---

## 📂 Example `data.json`

```json
[
  {
    "name": "sayidisi",
    "version": "1.0.0",
    "repo": "https://github.com/aardaakpinar/sayidisi",
    "branch": "main",
    "path": "cli",
    "main": "main.js"
  }
]
```
