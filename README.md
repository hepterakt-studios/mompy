<p align="center">
  <img src="assets/branding/mompy-cover.webp" alt="Mompy retro CRT monitor preview" width="440">
</p>

<h1 align="center">Mompy</h1>

<p align="center">
  <strong>Learn Python through a retro CRT training console.</strong>
</p>

<p align="center">
  Mompy is a local-first desktop learning app where beginners study Python through guided lessons, coding missions, feedback, progress, XP, and a friendly old-computer atmosphere.
</p>

<p align="center">
  <a href="https://github.com/hepter-studios/mompy/releases">Download</a>
  ·
  <a href="https://mompy.co">Website</a>
  ·
  <a href="https://github.com/hepter-studios/mompy/issues">Issues</a>
  ·
  <a href="#-run-from-source">Run from source</a>
</p>

<p align="center">
  <img alt="Status" src="https://img.shields.io/badge/status-in%20development-8cff3a?style=for-the-badge">
  <img alt="Python" src="https://img.shields.io/badge/Python-learning-3776ab?style=for-the-badge&logo=python&logoColor=white">
  <img alt="Frontend" src="https://img.shields.io/badge/frontend-HTML%20%7C%20CSS%20%7C%20JS-f7df1e?style=for-the-badge&logo=javascript&logoColor=black">
  <img alt="Backend" src="https://img.shields.io/badge/backend-Python-14354C?style=for-the-badge&logo=python&logoColor=white">
  <a href="https://github.com/hepter-studios/mompy/issues"><img alt="Issues" src="https://img.shields.io/github/issues/hepter-studios/mompy?style=for-the-badge&logo=github"></a>
  <a href="https://github.com/hepter-studios/mompy/stargazers"><img alt="Stars" src="https://img.shields.io/github/stars/hepter-studios/mompy?style=for-the-badge&logo=github"></a>
</p>

<p align="center">
  <a href="https://zdoc.app/en/hepter-studios/mompy">English</a>
  ·
  <a href="https://zdoc.app/pt/hepter-studios/mompy">Português</a>
</p>

> [!NOTE]
> Mompy is under active development. The source is public now, and installable builds will be published through GitHub Releases when the first stable package is ready.

---

## ✨ What is Mompy?

Mompy is a retro-futuristic Python training app for beginners.

Instead of starting with a boring editor, Mompy turns programming practice into a training terminal:

- short guided lessons before each mission block;
- small Python missions for beginners;
- instant feedback after running code;
- local progress, XP, and level tracking;
- CRT-style visuals, sound effects, and monitor reactions;
- a local-first experience without requiring an online account.

The goal is simple:

> Open Mompy, learn the concept, complete the mission, and keep progressing.

---

## 🧠 Learning flow

```txt
Open Mompy
↓
Boot / loading screen
↓
Guided lesson
↓
Python mission
↓
Code validation
↓
Feedback from Mompy
↓
Progress, XP, and next mission
```

Mompy should teach before it tests. A mission should not require a concept that the lesson did not introduce first.

---

## 🕹️ App experience

| Area | Purpose |
| --- | --- |
| Boot screen | Short CRT-style startup sequence and brand splash. |
| Start screen | Start or continue training with local profile and progress. |
| Guided lessons | Short lessons before each block of missions. |
| Mission screen | Objective, code editor, output, controls, and feedback. |
| Completion flow | Success reaction, repeat option, and next mission. |
| Settings | Audio, local profile, and progress reset. |

---

## 🎨 Visual identity

Mompy uses a dark retro-computer style inspired by CRT monitors, old terminals, industrial control panels, and pixel-era learning machines.

Core visual traits:

- black and dark green interface;
- neon CRT glow;
- scanlines and terminal effects;
- metallic panels;
- retro monitor mascot;
- old-computer boot atmosphere.

Mompy should feel like an intelligent training machine, not a normal website.

---

## 🧱 Architecture

Mompy is being organized as a frontend + Python backend project.

```txt
Mompy
├─ frontend
│  ├─ HTML
│  ├─ CSS
│  └─ JavaScript
│
└─ backend Python
   ├─ mission validation
   ├─ learner progress
   ├─ safe code execution
   └─ XP / level rules
```

The frontend keeps the visual experience. The Python backend is the official logic layer for missions, validation, progress, XP, and future safe execution of user code.

---

## 🛠️ Technology stack

Current / planned stack:

- HTML;
- CSS;
- JavaScript;
- Python;
- local JSON storage;
- pywebview bridge for desktop integration;
- PyInstaller or another Python packaging path for installable builds;
- GitHub Releases for downloads.

The project is local-first. Online accounts, cloud sync, and remote services are not required for the first version.

---

## 📦 Downloads

Installable builds are being prepared.

| Platform | Status |
| --- | --- |
| Windows | Planned first |
| macOS | Planned later |
| Linux | Planned later |

Downloads will be published here:

```txt
https://github.com/hepter-studios/mompy/releases
```

---

## 🚀 Run from source

Clone the repository:

```bash
git clone https://github.com/hepter-studios/mompy.git
cd mompy
```

When the Python desktop setup is ready, the expected flow will be:

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python main.py
```

On macOS/Linux, the activation command may be:

```bash
source .venv/bin/activate
```

> [!NOTE]
> Development commands may change while the Python backend and desktop bridge are being completed.

---

## 📁 Target project structure

```txt
mompy/
  frontend/
    index.html
    css/
    js/
    assets/

  backend/
    __init__.py
    missions.py
    lessons.py
    validator.py
    progress.py
    xp.py
    code_runner.py
    storage.py
    api.py

  data/
    progress.example.json

  tests/
    test_validator.py
    test_progress.py
    test_xp.py

  main.py
  requirements.txt
  README.md
  LICENSE
```

---

## 🧭 Roadmap

| Stage | Focus |
| --- | --- |
| Now | Finish the frontend, guided lessons, mission flow, audio, and local profile. |
| Next | Connect the frontend to the Python backend with a desktop bridge. |
| After that | Move validation, progress, XP, and safe code execution into Python. |
| Release | Package the first Windows build and publish it on GitHub Releases. |

---

## 🧪 Release checklist

Before the first public installable build:

- [ ] App opens through Python desktop shell.
- [ ] Frontend loads correctly.
- [ ] Backend responds to the frontend.
- [ ] Missions validate through Python.
- [ ] Code execution is safe and controlled.
- [ ] Progress saves locally.
- [ ] XP and level come from the backend.
- [ ] Assets and audio load in the packaged build.
- [ ] README has real download instructions.
- [ ] Build artifacts are attached to GitHub Releases, not committed to the repository.

---

## 🔒 Local-first philosophy

Mompy should work without forcing the learner to create an online account.

For the first version, data such as profile name, current mission, completed missions, XP, level, audio settings, and progress should stay on the user's computer.

Future online features may exist, but they should be optional.

---

## 🤔 Questions, bugs, or ideas?

Use GitHub Issues:

- [Report a bug](https://github.com/hepter-studios/mompy/issues/new?template=bug_report.md)
- [Request a feature](https://github.com/hepter-studios/mompy/issues/new?template=feature_request.md)
- [All issues](https://github.com/hepter-studios/mompy/issues)

Security reports should follow the [Security Policy](SECURITY.md).

---

## 💬 Community

Discord community: **coming soon**.

---

## 🌐 Official website

```txt
https://mompy.co
```

The website will be used for presentation, screenshots, downloads, release notes, and documentation.

---

## ⭐ Star History

<p align="center">
  <a href="https://www.star-history.com/?repos=hepter-studios%2Fmompy&type=date&legend=top-left">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/chart?repos=hepter-studios/mompy&type=date&theme=dark&legend=top-left" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/chart?repos=hepter-studios/mompy&type=date&legend=top-left" />
      <img alt="Mompy Star History Chart" src="https://api.star-history.com/chart?repos=hepter-studios/mompy&type=date&legend=top-left" />
    </picture>
  </a>
</p>

---

## ⚡ Contributors

<a href="https://github.com/hepter-studios/mompy/graphs/contributors" alt="View Contributors">
  <img src="https://contrib.rocks/image?repo=hepter-studios/mompy&max=1000&columns=10" alt="Mompy contributors" />
</a>

---

## 📚 Project standards

- [Code of Conduct](CODE_OF_CONDUCT.md)
- [Contributing Guide](CONTRIBUTING.md)
- [Security Policy](SECURITY.md)
- [License](LICENSE)

---

## 👤 Creator

Created by **Mackson Victor**.

GitHub: [macksonvictor](https://github.com/macksonvictor)

Organization: [Hepter Studios](https://github.com/hepter-studios)

---

## 📌 Project status

Mompy is currently in active development.

The repository may change frequently while the Python backend, guided lessons, safe execution, desktop packaging, and first public release are being completed.

---

## 📄 License

Mompy is not currently released under an open-source license.

See [LICENSE](LICENSE) for the current project notice.
