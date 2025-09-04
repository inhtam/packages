# 🧠 INH Packages Repository

Welcome to the official **INH CLI packages repository**.  
This repo contains JavaScript-based terminal packages that can be installed and run using the [INH CLI](https://github.com/inhtam/inh).

---
## 🔹 Badges

![GitHub Repo stars](https://img.shields.io/github/stars/inhtam/packages)
![GitHub forks](https://img.shields.io/github/forks/inhtam/packages)
![GitHub issues](https://img.shields.io/github/issues/inhtam/packages)
![License](https://img.shields.io/github/license/inhtam/packages)


---

## 📦 How It Works

- Each package is in its own folder with a `package.json` including `"inh": true` and `"main"` fields.
- The INH CLI downloads packages directly from this repository via GitHub raw links.
- Users **cannot upload directly** to this repo; contributions must be made via Pull Requests (PRs).

---

## 🔹 Installing Packages

Using INH CLI:

```bash
# Install a package
inh install sayidisi
````

---

## 🔹 Contributing Packages

We welcome contributions via GitHub Pull Requests.

1. **Fork this repository**.
2. **Create a new branch** for your package or changes:

```bash
git checkout -b feature/my-new-package
```

3. **Add your package** in a separate folder, include `package.json` with:

```json
{
  "name": "my-package",
  "version": "1.0.0",
  "inh": true,
  "main": "index.js"
}
```

4. **Commit and push** your changes:

```bash
git add .
git commit -m "Add new INH package: my-package"
git push origin feature/my-new-package
```

5. **Create a Pull Request** against the main branch of this repo.
6. Your PR will be reviewed and merged by the INH maintainers.

---

## 🔹 Directory Structure

```
inh-packages/
├─ package-one/
│  ├─ package.json
│  └─ index.js
├─ package-two/
│  ├─ package.json
│  └─ main.js
└─ README.md
```

---
