<h1 align="center">Anish</h1>

<p align="center">
  <b>Computer engineering student building automation, computer vision, and full-stack systems.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" alt="OpenCV" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white" alt="Playwright" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" />
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React" />
  <img src="https://img.shields.io/badge/Qt-41CD52?style=for-the-badge&logo=qt&logoColor=white" alt="Qt" />
</p>

---

<p align="center">
  <img src="https://anishrtech-stats.vercel.app/api?username=anishrtech&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" alt="GitHub stats" />
  <img src="https://anishrtech-stats.vercel.app/api/top-langs?username=anishrtech&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages" />
</p>

---

## About

I mostly create software that automates work people would normally do by hand. This includes browser automation, real-time computer vision, and focuses on local machine learning that runs without the cloud.<b></b>
I am currently a student at the **University of Minnesota: Twin Cities** (Class of **2030**).

---

## Featured Projects

### [Block Blast Vision Bot](https://github.com/anishrtech/blockblast-vision-bot)

A closed-loop autonomous agent that reads a live Android screen over USB, reconstructs game state with computer vision, plans an optimal move sequence with beam search, and executes the plan as real touch input while at high frame rates.

Implements the `scrcpy` wire protocol directly against a raw ADB socket and decodes H.264 in-process, achieving roughly 30 FPS where repeated screenshot calls cap out near 1 FPS. Piece detection is fully self-calibrating: it estimates background color per tray slot in HSV rather than hard-coding any colors, so it survives the game's changing themes.

`Python` `OpenCV` `NumPy` `PyAV` `ADB` `scrcpy`

### [Speak: Offline GPU Dictation](https://github.com/anishrtech/speak-local-dictation)

A Windows desktop app that transcribes speech to punctuated, formatted text entirely on-device and injects it into whatever application has focus. No cloud APIs, no audio ever leaving the machine.

Runs Whisper `large-v3-turbo` locally on the GPU via CTranslate2, with automatic fallback to an int8 CPU model when CUDA is unavailable. Global hotkeys work while any other app is focused, implemented with a low-level Win32 keyboard hook through `ctypes`, and text is injected using synthesized `SendInput` keystrokes.

`Python` `PySide6/Qt` `faster-whisper` `CUDA` `Win32 API` `ctypes`

### [DMV Appointment Monitor](https://github.com/anishrtech/dmv-appointment-monitor)

An unattended service that drives a headless browser through Minnesota's DVS booking funnel — including a mid-flow popup handoff and a geolocation-gated station search — and alerts Discord the moment a road test slot opens.

Alerts fire on the *transition* into availability and re-arm only once the slot is gone, which is the difference between a usable alerting system and one that pings a channel every twenty minutes.

`Python` `Playwright` `Headless Chromium` `Discord Webhooks`

### [DuoQuiz Landing](https://github.com/anishrtech/duoquiz-landing)

A landing page that renders its animated background as a procedural WebGL shader instead of a looping video — no meaningful network transfer, mathematically sharp at any pixel density, and no visible loop.

Isolates the browser-only WebGL context behind a dynamic import with SSR disabled, so the server still emits crawlable HTML while the GPU layer hydrates on the client.

`Next.js 16` `React 19` `TypeScript` `Tailwind CSS 4` `WebGL`

---

## What I Work With

| Area | Tools |
|---|---|
| Languages | Python, TypeScript, JavaScript, Lua |
| Automation | Playwright, ADB, Win32 API, headless browsers |
| Computer Vision & ML | OpenCV, NumPy, Whisper / CTranslate2, CUDA |
| Web | Next.js, React, Node.js, Express, Tailwind CSS |
| Desktop | PySide6 / Qt 6 |
| Practices | Environment-based configuration, assertion-backed self-checks, structured logging |

---

## Contact

- Email: **[anishr2008@gmail.com]**
