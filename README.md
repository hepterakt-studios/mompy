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
  <a href="#run-from-source"><strong>Run from source</strong></a>
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
  <a href="https://zdoc.app/pt/hepter-studios/mompy">Portugues</a>
</p>

> [!NOTE]
> Mompy is under active development. The first Windows desktop package is prepared and locally tested with PyInstaller.

---

## What Is Mompy?

Mompy is a gamified desktop learning app for Python beginners.

Instead of starting with a plain editor, Mompy turns the first steps of programming into a training console:

- guided lessons before each block of missions;
- 30 beginner-friendly missions;
- real Python validation in the backend;
- safe initial execution of learner code in a separate process;
- progress, XP and level controlled by Python;
- local-first desktop app with pywebview;
- CRT/industrial interface with Mompy reacting to success, errors and actions.

The visual layer stays in HTML/CSS/JavaScript. The app logic, mission data, validation, progress, XP and desktop shell are Python.

## Preview

![Mompy preview](frontend/assets/previews/mompy-preview-refined.png)

## Architecture

```txt
mompy/
  frontend/
    index.html
    css/
    js/
    assets/

  backend/
    api.py
    briefings.py
    code_runner.py
    lessons.py
    missions.py
    profile.py
    progress.py
    storage.py
    validator.py
    xp.py

  data/
    progress.example.json

  tests/
  scripts/
    build_windows.ps1

  main.py
  requirements.txt
```

## Run From Source

Install dependencies:

```bash
python -m pip install -r requirements.txt
```

Open as a desktop app:

```bash
python main.py
```

Check the backend without opening a window:

```bash
python main.py --check
```

Run the browser preview for development:

```bash
python main.py --serve --port 8770
```

Then open:

```txt
http://127.0.0.1:8770/frontend/index.html
```

## Build For Windows

Generate a Windows desktop build with PyInstaller:

```powershell
powershell -ExecutionPolicy Bypass -File scripts/build_windows.ps1
```

Generate a zip package for a GitHub Release:

```powershell
powershell -ExecutionPolicy Bypass -File scripts/build_windows.ps1 -Zip
```

The build output is created under:

```txt
dist/Mompy/Mompy.exe
dist/Mompy-windows-x64.zip
```

Build outputs are ignored by Git and should be attached to GitHub Releases, not committed to the repository.

## Tests

```bash
python -m unittest discover -s tests
```

## Releases

Installable builds are published in GitHub Releases:

https://github.com/hepter-studios/mompy/releases

## Platform Status

- Windows: build pipeline prepared and locally tested with PyInstaller.
- macOS: planned.
- Linux: planned.

## Roadmap Status

- 10.1: project organized and stable version saved.
- 10.2: frontend + Python backend architecture.
- 10.3: frontend connected to Python through pywebview/local API.
- 10.4: mission validation migrated to Python.
- 10.5: safer learner-code execution.
- 10.6: progress, XP and level controlled by Python.
- 10.7: Python desktop packaging prepared and locally tested.

## Community

- Bug reports: https://github.com/hepter-studios/mompy/issues
- Feature requests: https://github.com/hepter-studios/mompy/issues
- Security policy: see `SECURITY.md`
- Contributing guide: see `CONTRIBUTING.md`
