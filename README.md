<p align="center">
  <img src="assets/branding/mompy-cover.webp" alt="Mompy retro CRT monitor preview" width="460">
</p>

<h1 align="center">Mompy</h1>

<p align="center">
  <strong>A retro Python training app with guided lessons, coding missions, XP, and CRT-style feedback.</strong>
</p>

<p align="center">
  Mompy helps beginners learn Python through short lessons, focused missions, instant validation, local progress, and a friendly old-computer interface.
</p>

<p align="center">
  <a href="https://github.com/hepter-studios/mompy/releases"><strong>Download</strong></a>
  ·
  <a href="https://mompy.co"><strong>Website</strong></a>
  ·
  <a href="https://github.com/hepter-studios/mompy/issues"><strong>Issues</strong></a>
  ·
  <a href="#-run-from-source"><strong>Run from source</strong></a>
</p>

<p align="center">
  <img alt="Status" src="https://img.shields.io/badge/status-in%20development-8cff3a?style=for-the-badge">
  <img alt="Python" src="https://img.shields.io/badge/Python-learning-3776ab?style=for-the-badge&logo=python&logoColor=white">
  <img alt="Frontend" src="https://img.shields.io/badge/frontend-HTML%20%7C%20CSS%20%7C%20JS-f7df1e?style=for-the-badge&logo=javascript&logoColor=black">
  <img alt="Backend" src="https://img.shields.io/badge/backend-Python-14354C?style=for-the-badge&logo=python&logoColor=white">
  <img alt="Local first" src="https://img.shields.io/badge/local--first-no%20account-8cff3a?style=for-the-badge">
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

## What is Mompy?

Mompy is a **gamified desktop learning app for Python beginners**.

Instead of starting with a plain editor, Mompy turns the first steps of programming into a training console:

- guided lessons before each mission block;
- beginner-friendly Python missions;
- instant validation and feedback;
- local profile, progress, XP, and level tracking;
- CRT-style visuals, sound effects, and monitor reactions;
- local-first learning with no required online account.

The goal is simple:

> Learn the concept, complete the mission, earn progress, and keep building.

---

## Why Mompy?

Many beginners open a code editor and immediately feel lost.

Mompy is designed to make the first programming experience feel guided, visual, and alive. It teaches before it tests, then asks the learner to solve small missions using the concept they just studied.

Mompy should feel like an old training machine built to teach Python step by step.

---

## Learning flow

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

A mission should not require a concept that the previous lesson did not introduce first.

---

## First learning module

The first public module focuses on Python fundamentals.

| Missions | Topic | Concepts |
| --- | --- | --- |
| 1–5 | First commands | `print`, text, quotes, parentheses, output |
| 6–10 | Variables and values | names, values, assignment, strings, numbers |
| 11–15 | Decisions | `if`, `else`, comparisons, truth, indentation |
| 16–20 | Repetition | `for`, `range`, loops, counters, indentation |
| 21–25 | Lists | items, brackets, positions, iterating values |
| 26–30 | Functions and final mission | `def`, calling functions, organization, review |

Mission 30 is planned as a small final challenge that combines the fundamentals from the first module.

---

## App experience

| Area | Purpose |
| --- | --- |
| Boot screen | Short CRT-style startup sequence and brand splash. |
| Start screen | Start or continue training with local profile and progress. |
| Guided lessons | Short lessons before each block of missions. |
| Mission screen | Objective, code editor, output, controls, and feedback. |
| Completion flow | Success reaction, repeat option, and next mission. |
| Settings | Audio, local profile, and progress reset. |

---

## Visual identity

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

## Architecture

Mompy is being organized as a **frontend + Python backend** project.

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

## Technology stack

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

## Downloads

Installable builds are being prepared.

| Platform | Status |
| --- | --- |
| Windows | Planned first |
| macOS | Planned later |
| Linux | Planned later |

Downloads will be published on GitHub Releases:

```txt
https://github.com/hepter-studios/mompy/releases
```

---

## Run from source

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

## Target project structure

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

## Roadmap

| Stage | Focus |
| --- | --- |
| Now | Finish the frontend, guided lessons, mission flow, audio, and local profile. |
| Next | Connect the frontend to the Python backend with a desktop bridge. |
| Backend | Move validation, progress, XP, and safe code execution into Python. |
| Release | Package the first Windows build and publish it on GitHub Releases. |
| Later | Add more Python modules beyond the first 30 missions. |

---

## Release checklist

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

## Local-first philosophy

Mompy should work without forcing the learner to create an online account.

For the first version, data such as profile name, current mission, completed missions, XP, level, audio settings, and progress should stay on the user's computer.

Future online features may exist, but they should be optional.

---

## Questions, bugs, or ideas?

Use GitHub Issues:

- [Report a bug](https://github.com/hepter-studios/mompy/issues/new?template=bug_report.md)
- [Request a feature](https://github.com/hepter-studios/mompy/issues/new?template=feature_request.md)
- [All issues](https://github.com/hepter-studios/mompy/issues)

Security reports should follow the [Security Policy](SECURITY.md).

---

## Community

Discord community: **coming soon**.

---

## Official website

```txt
https://mompy.co
```

The website will be used for presentation, screenshots, downloads, release notes, and documentation.

---

## Star History

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

## Contributors

<a href="https://github.com/hepter-studios/mompy/graphs/contributors" alt="View Contributors">
  <img src="https://contrib.rocks/image?repo=hepter-studios/mompy&max=1000&columns=10" alt="Mompy contributors" />
</a>

---

## Project standards

- [Code of Conduct](CODE_OF_CONDUCT.md)
- [Contributing Guide](CONTRIBUTING.md)
- [Security Policy](SECURITY.md)
- [License](LICENSE)

---

## Creator

Created by **Mackson Victor**.

GitHub: [macksonvictor](https://github.com/macksonvictor)

Organization: [Hepter Studios](https://github.com/hepter-studios)

---

## Project status

Mompy is currently in active development.

The repository may change frequently while the Python backend, guided lessons, safe execution, desktop packaging, and first public release are being completed.

---

## License

Mompy is not currently released under an open-source license.

See [LICENSE](LICENSE) for the current project notice.
