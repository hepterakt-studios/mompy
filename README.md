<p align="center">
  <img src="assets/branding/mompy-cover.webp" alt="Mompy monitor showing GitHub logo" width="420">
</p>

# Mompy: Learn Python with a Retro Training Console

[![Status](https://img.shields.io/badge/status-in%20development-8cff3a?style=for-the-badge)](#project-status)
[![Platform](https://img.shields.io/badge/platform-cross--platform-6f42c1?style=for-the-badge)](#platform-strategy)
[![Built with](https://img.shields.io/badge/built%20with-HTML%20%7C%20CSS%20%7C%20JS-f7df1e?style=for-the-badge&logo=javascript&logoColor=black)](#technology-stack)
[![Desktop](https://img.shields.io/badge/desktop-Electron-47848f?style=for-the-badge&logo=electron&logoColor=white)](#desktop-app)
[![Python Training](https://img.shields.io/badge/python-training-3776ab?style=for-the-badge&logo=python&logoColor=white)](#what-mompy-does)

<!-- Future community badge:
[![Discord](https://img.shields.io/badge/Discord-Join%20the%20community-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/YOUR_INVITE)
-->

[English](https://zdoc.app/en/macksonvictor/mompy) | [Português](https://zdoc.app/pt/macksonvictor/mompy)

**Mompy** is a retro CRT-style desktop app that helps beginners learn Python through guided missions, instant feedback, local progress, sound effects, and a friendly monitor mascot.

> [!NOTE]
> Mompy is currently in active development. The source code is public, but the first downloadable desktop releases are still being prepared.

---

## Quick links

| Resource | Status | Link |
| --- | --- | --- |
| Source code | Available | [GitHub Repository](https://github.com/macksonvictor/mompy) |
| Desktop downloads | Planned | [GitHub Releases](https://github.com/macksonvictor/mompy/releases) |
| Official website | Planned | [mompy.co](https://mompy.co) |
| Documentation | Planned | Coming soon |
| Discord community | Planned | Coming soon |
| Issues / feedback | Available | [GitHub Issues](https://github.com/macksonvictor/mompy/issues) |

---

## What Mompy does

Mompy turns beginner Python practice into small interactive missions.

The app is designed to:

- teach Python step by step;
- give the user short coding challenges;
- validate the code written by the user;
- show output and feedback immediately;
- save progress locally;
- react with animations and sounds;
- make learning feel like using an old intelligent training terminal.

The goal is simple: **open Mompy, complete missions, learn Python, and keep progressing.**

---

## Download options

Mompy is planned to be distributed as a desktop app through GitHub Releases.

| Platform | Package | Status |
| --- | --- | --- |
| Windows | `.exe` / installer | Planned |
| macOS | `.dmg` | Planned |
| Linux | `.AppImage` or another Linux package | Planned |
| Web preview | Browser-based preview or documentation page | Possible later |

Example future release assets:

```txt
Mompy-Setup-Windows.exe
Mompy-macOS.dmg
Mompy-Linux.AppImage
```

The repository should contain the source code. Generated builds and installers should be published through **GitHub Releases**, not committed into the main codebase.

---

## Core learning loop

1. Open the app.
2. Wait for the CRT-style loading screen.
3. Start or continue training.
4. Read the mission.
5. Write Python code.
6. Run the code.
7. Receive feedback from Mompy.
8. Complete the mission and unlock the next one.

---

## Main app areas

### Loading screen

The app starts with a CRT-style loading screen that feels like an old training terminal turning on.

Expected behavior:

- show Mompy branding;
- animate a real loading bar;
- avoid sound during loading;
- transition cleanly to the start screen.

### Start screen

The start screen is the user entry point.

Expected behavior:

- show Mompy monitor/mascot;
- show `START` and `CONTINUE` actions;
- display local user data;
- show level and completed missions;
- play only the calm CRT ambient sound.

### Mission screen

The mission screen is where learning happens.

Expected behavior:

- show the mission objective;
- provide a code editor area;
- provide output feedback;
- offer Help, Back, Run, Settings, and Exit controls;
- validate the answer;
- update Mompy's state based on success or error.

### Completion flow

When a mission is completed, Mompy should react and ask the user what to do next.

Expected behavior:

- show success feedback;
- change Mompy to a happy state;
- display completion text inside Mompy's screen;
- allow `REPEAT`;
- allow `NEXT MISSION`;
- prevent accidental auto-advance.

### Settings

Settings should control the local experience without requiring an online account.

Expected behavior:

- audio on/off;
- music volume;
- sound effects volume;
- language preference;
- local profile editing;
- progress reset with confirmation.

---

## Visual identity

Mompy uses a retro-futuristic visual style inspired by old terminals, CRT monitors, and industrial control panels.

Main characteristics:

- dark industrial interface;
- green CRT glow;
- terminal-style typography;
- pixel/scanline effects;
- metallic panels;
- retro monitor mascot;
- old-computer atmosphere.

Mompy should feel like an old intelligent training machine, not a normal website.

---

## Feature status

| Area | Status |
| --- | --- |
| Retro CRT interface | In development |
| Loading screen | In development |
| Start screen | In development |
| Mission screen | In development |
| Code editor area | In development |
| Output panel | In development |
| Help / Run / Back buttons | In development |
| Settings modal | In development |
| Local user profile | Planned / in progress |
| Local progress saving | Planned / in progress |
| Mompy mascot states | Planned / in progress |
| Mission completion flow | Planned / in progress |
| Audio system | Planned / in progress |
| Electron packaging | Planned |
| GitHub Releases | Planned |
| Official website | Planned |
| Discord community | Planned |

---

## Planned features

### Learning system

- Python beginner missions
- Step-by-step challenges
- Mission validation
- Mission hints
- Mission progress
- Repeat mission
- Next mission
- Level system

### Mompy character

- Idle state
- Talking animation
- Happy state
- Sad/error state
- CRT shutdown animation
- Terminal animation on the start screen
- Mission completion messages inside Mompy's screen

### Audio

- Button click sound
- Run sound
- Success sound
- Error sound
- CRT shutdown sound
- Calm CRT ambient sound for the start screen

### User profile

- First-name setup
- Local profile
- Language preference
- Audio settings
- Progress reset
- Future optional cloud sync

### Desktop app

- Electron app
- Windows build
- macOS build
- Linux build
- Local-first storage
- GitHub Releases
- Official website/download page

---

## Local-first philosophy

Mompy is designed to work without requiring an online account.

For the first version, the following data should stay on the user's computer:

- first name;
- language preference;
- current mission;
- completed missions;
- audio settings;
- interface settings;
- progress state.

No server, password, or cloud account is required for the first desktop version.

Future online features may exist, but they should be optional.

---

## Desktop app

Mompy is being built with web technologies, but the final goal is to make it feel like a real installed desktop app.

```txt
HTML + CSS + JavaScript
↓
Electron
↓
Desktop app releases
```

Distribution model:

```txt
Mompy app = installable desktop app
mompy.co = official website / download page
GitHub Releases = app downloads
```

---

## Platform strategy

Mompy should not be described as Windows-only.

The project can start with one platform during early testing, but the long-term direction is:

| Platform | Status |
| --- | --- |
| Windows | Planned |
| macOS | Planned |
| Linux | Planned |
| Web preview | Possible future option, mainly for preview or documentation |

Each operating system may need its own build/package later. GitHub Releases can contain separate downloads for each platform.

---

## System requirements

### For users

The first public releases are planned for desktop computers.

Expected requirements:

- Windows, macOS, or Linux depending on the release package;
- keyboard and mouse;
- enough storage for a small desktop app;
- no required online account.

### For developers

To run or package the project locally, the recommended tools are:

- Git;
- Node.js;
- npm;
- VS Code or another code editor;
- Electron / Electron Builder when desktop packaging is configured.

---

## Technology stack

Current / planned stack:

- HTML
- CSS
- JavaScript
- LocalStorage
- Electron
- Electron Builder
- Git
- GitHub
- GitHub Releases

Possible future additions:

- Node.js helpers
- Local file storage
- Cloud sync
- Online accounts
- Mission editor
- AI-assisted hints

---

## Project structure

Planned structure:

```txt
mompy/
  src/
    index.html
    styles.css
    main.js

    assets/
      images/
      audio/
      icons/
      branding/

  electron/
    main.js
    preload.js

  README.md
  package.json
  .gitignore
```

The structure may change while the project is still in development.

---

## Development

Clone the repository:

```bash
git clone https://github.com/macksonvictor/mompy.git
cd mompy
```

Install dependencies:

```bash
npm install
```

Run the app in development:

```bash
npm run dev
```

Or, depending on the current setup:

```bash
npm start
```

> [!NOTE]
> The development commands may change while the Electron structure is being completed.

---

## Build

When Electron is configured, the app should be built with:

```bash
npm run build
```

The generated installer or executable should not be committed directly into the repository.

Do not commit:

```txt
node_modules/
dist/
build/
release/
out/
.env
*.exe
*.dmg
*.AppImage
*.log
```

Installers and packaged builds should be published later through **GitHub Releases**.

---

## Release model

The repository contains the source code.

GitHub Releases will be used for downloadable versions of the app.

Example future release:

```txt
Mompy v1.0.0
Mompy-Setup-Windows.exe
Mompy-macOS.dmg
Mompy-Linux.AppImage
```

Users will be able to download the app without touching the source code.

---

## Audio files

Expected audio files:

```txt
assets/audio/click.wav
assets/audio/run.wav
assets/audio/success.wav
assets/audio/error.wav
assets/audio/shutdown.wav
assets/audio/mompy_crt_ambient_loop_minimal.wav
```

Audio behavior:

- Loading screen: no sound
- Start screen: ambient sound only
- Mission screen: sound effects only
- Run: run sound
- Correct answer: success sound
- Wrong answer: error sound
- CRT shutdown animation: shutdown sound

---

## Roadmap

### Phase 1 — Main Layout

Fix the main mission screen layout, alignment, panels, editor, output, and top bar.

### Phase 2 — Buttons

Add and organize Settings, Exit, Back, Help, and Run buttons.

### Phase 3 — Button Functions

Implement modals, shortcuts, confirmation dialogs, and mission completion behavior.

### Phase 4 — Start Screen

Create the entry screen with Mompy, Start, Continue, user information, level, and missions completed.

### Phase 5 — Loading Screen

Create the CRT-style loading screen with Mompy and a real animated progress bar.

### Phase 6 — Mompy Animations

Implement Mompy states, talking animation, happy/sad states, terminal animation, and CRT shutdown interaction.

### Phase 7 — Audio

Implement sound effects and ambient sound behavior.

### Phase 8 — Progress and Missions

Implement local mission data, validation, progress saving, Start, Continue, Reset Progress, and level updates.

### Phase 9 — Polish and Testing

Fix bugs, improve alignment, test screens, test audio, test progress, and create a test checklist.

### Phase 10 — Desktop App and GitHub

Configure Electron, prepare desktop packaging, organize the repository, and push the project to GitHub.

---

## Test checklist

Before release:

### Loading

- [ ] Loading screen appears
- [ ] Loading progress works
- [ ] Loading has no sound
- [ ] Loading transitions to start screen

### Start screen

- [ ] Start button works
- [ ] Continue button works
- [ ] User name is loaded from local profile
- [ ] Level appears correctly
- [ ] Missions completed count appears correctly
- [ ] Ambient sound works only here

### Mission screen

- [ ] Run button works
- [ ] Correct code completes mission
- [ ] Wrong code shows hint
- [ ] Help opens mission help
- [ ] Back asks confirmation
- [ ] Output updates correctly
- [ ] Mompy reacts correctly

### Completion flow

- [ ] Mission completed message appears on Mompy screen
- [ ] Back, Help, and Run disable after completion
- [ ] Repeat works
- [ ] Next Mission works
- [ ] Settings and Exit still work

### Settings

- [ ] Settings modal opens
- [ ] Audio settings save
- [ ] Profile editing works
- [ ] Progress reset asks confirmation
- [ ] Language preference is saved

### GitHub

- [ ] `.gitignore` exists
- [ ] `node_modules` is not committed
- [ ] Build folders are not committed
- [ ] README is updated
- [ ] Project pushes correctly
- [ ] Main branch is stable
- [ ] Dev branch is used for changes

---

## Git workflow

Recommended workflow:

```txt
main = stable version
dev = development version
```

Before major changes:

```bash
git add .
git commit -m "Save current working version"
git push
```

After a successful feature:

```bash
git add .
git commit -m "Add Mompy audio system"
git push
```

---

## Official website

Planned official website:

```txt
https://mompy.co
```

The website can be used for:

- project presentation;
- screenshots;
- download button;
- GitHub link;
- release notes;
- future documentation.

---

## Related projects

Mompy can grow into a small ecosystem over time.

| Project | Status | Description |
| --- | --- | --- |
| **Mompy Desktop** | Current repository | The main retro Python training app. |
| **Mompy Website** | Planned | Official website for downloads, screenshots, release notes, and documentation. |
| **Mompy Missions** | Planned | A future mission/content area for Python lessons and challenge packs. |
| **Mompy Docs** | Planned | Future documentation for users, developers, and contributors. |

> [!NOTE]
> Related projects will only be linked here when they exist. This section is prepared for future expansion without pretending that unfinished repositories already exist.

---

## Community

Mompy does not have an official community server yet, but this README is prepared for it.

Planned community channels:

- Discord server for announcements, feedback, and testing;
- GitHub Issues for bugs and feature requests;
- GitHub Discussions for ideas and questions, if enabled later.

Future Discord badge placeholder:

```md
[![Discord](https://img.shields.io/badge/Discord-Join%20the%20community-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/YOUR_INVITE)
```

---

## Stars stats

<p align="center">
<a href="https://star-history.com/#macksonvictor/mompy">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=macksonvictor/mompy&type=Date&theme=dark" />
    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=macksonvictor/mompy&type=Date" />
    <img alt="Mompy Star History Chart" src="https://api.star-history.com/svg?repos=macksonvictor/mompy&type=Date" />
  </picture>
</a>
</p>

---

## Contributors

<a href="https://github.com/macksonvictor/mompy/graphs/contributors" alt="View Contributors">
  <img src="https://contrib.rocks/image?repo=macksonvictor/mompy&max=1000&columns=10" alt="Mompy contributors" />
</a>

---

## Author

Created by **Mackson Victor**.

GitHub:

```txt
https://github.com/macksonvictor
```

---

## Project status

Mompy is currently in active development.

This repository may change frequently while the interface, mission system, audio, and desktop packaging are being completed.

---

## License

License not defined yet.

Until a license is chosen, all rights are reserved by the author.
