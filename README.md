<div align="center">

# ⚙️ .github — GitHub Profile & Automation Config
This repository contains the source code, automation workflows, and configuration assets for my GitHub profile.

</div>

<p align="center">
  <a href="https://github.com/x404x-dev"><img src="https://img.shields.io/badge/Visit_Profile-181717?style=for-the-badge&logo=github&logoColor=white" alt="Visit Profile" /></a>
  &nbsp;
  <a href="./profile/README.md"><img src="https://img.shields.io/badge/View_Generated_README-2088FF?style=for-the-badge&logo=markdown&logoColor=white" alt="View Generated README" /></a>
</p>

---

### 📁 Project Structure

```text
.github/
├── .github/workflows/   # Automated GitHub Actions workflows
│   ├── snake.yml
│   └── update.yml
├── profile/             # Output folder (Required by GitHub to display bio)
│   └── README.md
└── src/                 # Source code & original templates
    ├── icons/
    ├── snake/
    ├── README.md
    └── icons.json
```

---

### 🔄 How It Works

1. **Source Template**: All original content and custom variables are configured inside `src/README.md`.
2. **Automated Pipeline**: When changes are pushed or triggered on a schedule, GitHub Actions (`update.yml` & `snake.yml`) run automatically.
3. **Build & Render**: The workflow replaces template variables, updates dynamic data (snake animation, stats, etc.), and outputs the generated file to `profile/README.md`.
4. **Publish**: GitHub automatically fetches `profile/README.md` to display on the public profile page.

---

> [!NOTE]
> Any edits to the bio content should be made in **`src/README.md`**. Do not edit `profile/README.md` directly.
