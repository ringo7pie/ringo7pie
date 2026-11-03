# ringo7pie

**I build tools that let AI assistants work on real projects safely.**
ChatGPT reads only what I approve, Claude Code implements what I review, and self-tests decide whether it worked.

Windows and Ubuntu · Node.js · PowerShell 7 · Python · C++/Qt · Lua · local AI on a single 24 GB GPU

## Featured projects

| Project | What it is | Built with |
|---|---|---|
| **[chatgpt-project-bridge](https://github.com/ringo7pie/chatgpt-project-bridge)** | A read-only MCP bridge for ChatGPT: it reads the local projects I approve (approval by SHA-256 fingerprint) and hands approved coding jobs to Claude Code. Hub mode, 31 tools, about 1,250 self-test checks, zero npm dependencies. | Node.js, PowerShell 7, Python/GTK |
| **[single-gpu-local-ai](https://github.com/ringo7pie/single-gpu-local-ai)** | Running and measuring a pack of local AI services on one 24 GB GPU: GPU arbitration, MoE inference, image-to-3D, and an evaluation harness that compares cloud and local models on hidden tests. | Python, systemd, Ollama |
| **[crow-translate](https://github.com/ringo7pie/crow-translate)** | An unofficial Crow Translate fork with local OCR, local translation models, a Codex CLI backend, and a Windows installer. | C++/Qt, Python |
| **[wezterm-kitty-ja](https://github.com/ringo7pie/wezterm-kitty-ja)** | WezTerm for Windows with kitty-compatible key bindings, a Japanese command palette, and session restore. | Lua, PowerShell |
| **[RoboGen-GenesisWorld](https://github.com/ringo7pie/RoboGen-GenesisWorld)** | RoboGen and the Genesis physics simulator on Google Colab's free GPU. | Python, Jupyter |

## How I work

- **Plan, implement, verify.** I plan in ChatGPT, implement with Claude Code, and keep every change behind self-tests that run in CI.
- **Facts next to the code.** Each project keeps a small knowledge base of verified facts (environment limits, procedures, pitfalls), so the next session starts from what is true.
- **Safe to publish.** Pinned and verified dependencies, upstream licenses checked, and no private data in public repositories.

## 日本語

AI（ChatGPT・Claude Code）に、実際のプロジェクトを安全に扱わせるための道具を作っています。
ChatGPT には承認したものだけを読ませ、Claude Code には確認した計画だけを実装させ、結果は自己試験で確かめます。
Windows と Ubuntu の両方で動くこと、1 枚の GPU でローカル AI を動かして測ることにも取り組んでいます。
