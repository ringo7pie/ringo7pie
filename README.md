# ringo7pie

**[日本語](#日本語)** | **[English](#english)**

<img width="1365" height="768" alt="Demon of the Crown（デーモン・クラウン）" src="https://github.com/user-attachments/assets/c7ea0c1b-33cf-400d-94ae-91f5b9fe864b" />

## 日本語

個人でインディーゲーム **Demon of the Crown（デーモン・クラウン）** を開発しています。
AI（ChatGPT・Claude Code）に、実際のプロジェクトを安全に扱わせるための道具も作っています。

### Demon of the Crown（デーモン・クラウン）― アルファテスト版

AI の仲間に、声（または文字）で指示を出して進むダンジョン探索ゲームです。
仲間は声で答え、自分で考えて戦います。音声認識・会話・音声合成は、遊ぶ人の PC の中で動きます。
Windows 用・無料です。アルファテスト版で遊べるのは、最初の 5 マップです。未完成で、不具合があります。

- **ダウンロード**: [DemonCrown-0.1.0-alpha-win64-setup.exe（インストーラー・709 MB）](https://github.com/ringo7pie/demoncrown/releases/download/v0.1.0-alpha/DemonCrown-0.1.0-alpha-win64-setup.exe)
  - ダウンロードの前に、リポジトリの「プレイ記録の送信」を必ずお読みください。
- **リポジトリ**: [ringo7pie/demoncrown](https://github.com/ringo7pie/demoncrown)（説明・動作環境・インストール・不具合の報告）
- **YouTube**: [予告動画](https://www.youtube.com/watch?v=uC_fTwHhQyI) ・ [機能紹介の動画](https://www.youtube.com/watch?v=dSyVj8uGO6Y) ・ [チャンネル](https://www.youtube.com/@ringo7pie)
- **SNS**: [X](https://x.com/ringo7pie) ・ [Instagram](https://www.instagram.com/ringo7pie/)

### AI と開発の道具

ChatGPT には承認したものだけを読ませ、Claude Code には確認した計画だけを実装させ、結果は自己試験で確かめます。
Windows と Ubuntu の両方で動くこと、1 枚の GPU でローカル AI を動かして測ることにも取り組んでいます。

Windows・Ubuntu · Godot · Node.js · PowerShell 7 · Python · C++/Qt · Lua · 24 GB の GPU 1 枚で動かすローカル AI

### 公開しているプロジェクト

| プロジェクト | 内容 | 使っている物 |
|---|---|---|
| **[demoncrown](https://github.com/ringo7pie/demoncrown)** | ゲーム「Demon of the Crown」のアルファテスト版の配布ページ。AI の仲間に声で指示を出すダンジョン探索ゲーム（Windows・無料）。 | Godot |
| **[voicechanger](https://github.com/ringo7pie/voicechanger)** | ゲーム実況の録画用に、マイクの声をリアルタイムで変えるボイスチェンジャー（Windows）。ピッチ・フォルマント変換と AI 声質変換（Beatrice 2）を切り替え、VB-CABLE 経由で OBS に渡す。素の声を録画に入れない設計。 | Python, PySide6 |
| **[chatgpt-project-bridge](https://github.com/ringo7pie/chatgpt-project-bridge)** | ChatGPT 用の読み取り専用の MCP ブリッジ。承認したローカルのプロジェクトだけを読ませ（承認は SHA-256 の指紋で行う）、承認したコーディングの仕事を Claude Code に渡す。ハブモード、31 個のツール、約 1,250 項目の自己試験、npm の依存はゼロ。 | Node.js, PowerShell 7, Python/GTK |
| **[single-gpu-local-ai](https://github.com/ringo7pie/single-gpu-local-ai)** | 24 GB の GPU 1 枚で、複数のローカル AI サービスを動かして測る。GPU の調停、MoE 推論、画像からの 3D 生成、クラウドとローカルのモデルを非公開の試験で比べる評価の仕組み。 | Python, systemd, Ollama |
| **[crow-translate](https://github.com/ringo7pie/crow-translate)** | Crow Translate の非公式フォーク。ローカルの OCR と翻訳モデル、Codex CLI のバックエンド、同時通訳（Windows）、Windows 用インストーラー。 | C++/Qt, Python |
| **[wezterm-kitty-ja](https://github.com/ringo7pie/wezterm-kitty-ja)** | Windows の WezTerm を、kitty と同じキー操作にする設定。日本語のコマンドパレット、セッションの復元。 | Lua, PowerShell |
| **[RoboGen-GenesisWorld](https://github.com/ringo7pie/RoboGen-GenesisWorld)** | RoboGen と物理シミュレーター Genesis を、Google Colab の無料の GPU で動かす。 | Python, Jupyter |

### 進め方

- **計画し、実装し、確かめる。** ChatGPT で計画し、Claude Code で実装し、すべての変更を CI で流れる自己試験で確かめます。
- **事実をコードの隣に置く。** 各プロジェクトに、確かめた事実（環境の制約・手順・落とし穴）の小さなナレッジベースを置き、次の作業を事実から始めます。
- **安全に公開する。** 依存物は版を固定して検証し、元のライセンスを確かめ、公開するリポジトリに個人のデータを入れません。

---

## English

I'm a solo developer making the indie game **Demon of the Crown**.
I also build tools that let AI assistants (ChatGPT, Claude Code) work on real projects safely.

### Demon of the Crown — alpha test build

A dungeon crawler where you lead AI companions by voice (or typed text).
They answer by voice and fight on their own judgment. Speech recognition, conversation and speech synthesis run on your own PC.
Windows, free. The alpha covers the first 5 maps. It is unfinished and has bugs.

- **Download**: [DemonCrown-0.1.0-alpha-win64-setup.exe (installer, 709 MB)](https://github.com/ringo7pie/demoncrown/releases/download/v0.1.0-alpha/DemonCrown-0.1.0-alpha-win64-setup.exe)
  - Please read the play-data notice in the repository before downloading.
- **Repository**: [ringo7pie/demoncrown](https://github.com/ringo7pie/demoncrown) (description, requirements, installation, bug reports)
- **YouTube**: [trailer](https://www.youtube.com/watch?v=uC_fTwHhQyI) · [feature overview](https://www.youtube.com/watch?v=dSyVj8uGO6Y) · [channel](https://www.youtube.com/@ringo7pie)
- **Social**: [X](https://x.com/ringo7pie) · [Instagram](https://www.instagram.com/ringo7pie/)

### Tools for working with AI

ChatGPT reads only what I approve, Claude Code implements only the plans I review, and self-tests decide whether it worked.
I also work on running on both Windows and Ubuntu, and on running and measuring local AI on a single GPU.

Windows and Ubuntu · Godot · Node.js · PowerShell 7 · Python · C++/Qt · Lua · local AI on a single 24 GB GPU

### Featured projects

| Project | What it is | Built with |
|---|---|---|
| **[demoncrown](https://github.com/ringo7pie/demoncrown)** | The download page for the alpha test build of "Demon of the Crown", a dungeon crawler where you lead AI companions by voice (Windows, free). | Godot |
| **[voicechanger](https://github.com/ringo7pie/voicechanger)** | A real-time voice changer for recording gameplay on Windows: pitch/formant DSP or Beatrice 2 AI voice conversion, routed via VB-CABLE into OBS so the raw voice never reaches the recording. | Python, PySide6 |
| **[chatgpt-project-bridge](https://github.com/ringo7pie/chatgpt-project-bridge)** | A read-only MCP bridge for ChatGPT: it reads the local projects I approve (approval by SHA-256 fingerprint) and hands approved coding jobs to Claude Code. Hub mode, 31 tools, about 1,250 self-test checks, zero npm dependencies. | Node.js, PowerShell 7, Python/GTK |
| **[single-gpu-local-ai](https://github.com/ringo7pie/single-gpu-local-ai)** | Running and measuring a pack of local AI services on one 24 GB GPU: GPU arbitration, MoE inference, image-to-3D, and an evaluation harness that compares cloud and local models on hidden tests. | Python, systemd, Ollama |
| **[crow-translate](https://github.com/ringo7pie/crow-translate)** | An unofficial Crow Translate fork with local OCR, local translation models, a Codex CLI backend, simultaneous interpretation (Windows), and a Windows installer. | C++/Qt, Python |
| **[wezterm-kitty-ja](https://github.com/ringo7pie/wezterm-kitty-ja)** | WezTerm for Windows with kitty-compatible key bindings, a Japanese command palette, and session restore. | Lua, PowerShell |
| **[RoboGen-GenesisWorld](https://github.com/ringo7pie/RoboGen-GenesisWorld)** | RoboGen and the Genesis physics simulator on Google Colab's free GPU. | Python, Jupyter |

### How I work

- **Plan, implement, verify.** I plan in ChatGPT, implement with Claude Code, and keep every change behind self-tests that run in CI.
- **Facts next to the code.** Each project keeps a small knowledge base of verified facts (environment limits, procedures, pitfalls), so the next session starts from what is true.
- **Safe to publish.** Pinned and verified dependencies, upstream licenses checked, and no private data in public repositories.
