![](https://github.com/Acelogic/Acelogic/raw/master/Github.gif?raw=true)

# Hey, I'm Miguel 👋

**Systems hacker in NY** · Writing code since 2011 · Linux bring-up on new silicon · Options trader

![C](https://img.shields.io/badge/-C-A8B9CC?style=flat&logo=c&logoColor=black)
![Rust](https://img.shields.io/badge/-Rust-000000?style=flat&logo=rust&logoColor=white)
![Swift](https://img.shields.io/badge/-Swift-F05138?style=flat&logo=swift&logoColor=white)
![Java](https://img.shields.io/badge/-Java-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Kotlin](https://img.shields.io/badge/-Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white)
![Go](https://img.shields.io/badge/-Go-00ADD8?style=flat&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![ARM64](https://img.shields.io/badge/-ARM64-0091BD?style=flat&logo=arm&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Vulkan](https://img.shields.io/badge/-Vulkan-AC162C?style=flat&logo=vulkan&logoColor=white)

I've been taking operating systems apart since 2011, starting with iOS 5 jailbreaks and Android Gingerbread, and picked up robotics, [emulators](https://github.com/Acelogic/CHIP-8-C) and a [Unix shell](https://github.com/Acelogic/TSHImplementation) along the way. These days I'm booting Linux on undocumented Apple and Qualcomm silicon, building a PS5 runtime, and porting new generative models to MLX, usually with a few coding agents running alongside me. Off the clock, I sell options and build tools to stress-test my portfolio.

---

## 🐧 Bringing Up New Silicon

- **[Aurora Silicon](https://github.com/aurora-silicon)** — Linux and Windows-on-Arm for Apple Silicon, M1 through M6. I have 25 merged patches across [linux](https://github.com/aurora-silicon/linux/pulls?q=is%3Apr+author%3AAcelogic+is%3Amerged), [m1n1](https://github.com/aurora-silicon/m1n1/pulls?q=is%3Apr+author%3AAcelogic+is%3Amerged) and [u-boot](https://github.com/aurora-silicon/u-boot/pulls?q=is%3Apr+author%3AAcelogic+is%3Amerged): initial native boot on **M5** (J813) and **M6** (J873g), SMP for all 10 M5 and all 12 M6 cores, CPU frequency scaling, DCP display, USB3/USB4 and USB-C DisplayPort, plus hardware video decode and Wi-Fi/Bluetooth on the **J700** MacBook Neo.
- **[q1n1](https://github.com/Acelogic/q1n1)** — [m1n1](https://github.com/AsahiLinux/m1n1) retargeted from Apple Silicon to a **Snapdragon X2E** laptop (ASUS Zenbook A16). It's a UEFI app that takes the machine at EL2 after `ExitBootServices` and serves m1n1's proxy protocol over its own USB stack, so a host can drive the hardware interactively.

## 🎮 Emulation

My first emulator was CHIP-8 in C. The latest is a PS5 runtime.

- **[VibeStation5](https://github.com/Acelogic/VibeStation5)** — An experimental PS4/PS5 runtime for macOS, iPadOS and Android, derived from [SharpEmu](https://github.com/sharpemu/sharpemu). It uses an ARM64-native interpreter that works within iPadOS's executable-memory limits, and on Android a C++ runtime over JNI with Vulkan rendering.
- **[sharpemu-agentic-toolkit](https://github.com/Acelogic/sharpemu-agentic-toolkit)** — Reverse-engineering tooling for SharpEmu: NID research, Ghidra-assisted analysis, and timestamped screenshot contact sheets for visual regression.

## 🧠 Generative Models on Apple Silicon

Been playing with transformers since GPT-2. These are native [MLX](https://github.com/ml-explore/mlx) ports, so the models run on a Mac without a CUDA box.

| Project | What it does | |
|---|---|---|
| **[LTX-2-MLX](https://github.com/Acelogic/LTX-2-MLX)** | Port of the LTX-2 video generation model | ![](https://img.shields.io/github/stars/Acelogic/LTX-2-MLX?style=flat&label=%E2%98%85&color=555) |
| **[RVC-MLX](https://github.com/Acelogic/Retrieval-based-Voice-Conversion-MLX)** | Voice conversion that runs 8.71× faster than PyTorch MPS | ![](https://img.shields.io/github/stars/Acelogic/Retrieval-based-Voice-Conversion-MLX?style=flat&label=%E2%98%85&color=555) |
| **[personaplex-mlx](https://github.com/Acelogic/personaplex-mlx)** | NVIDIA's PersonaPlex 7B, full-duplex real-time voice chat | ![](https://img.shields.io/github/stars/Acelogic/personaplex-mlx?style=flat&label=%E2%98%85&color=555) |
| **[heartlib-mlx](https://github.com/Acelogic/heartlib-mlx)** | HeartMuLa music models, about 2× faster than PyTorch MPS | ![](https://img.shields.io/github/stars/Acelogic/heartlib-mlx?style=flat&label=%E2%98%85&color=555) |
| **[daVinci-MagiHuman-mlx](https://github.com/Acelogic/daVinci-MagiHuman-mlx)** | 15B text-to-video model (work in progress) | ![](https://img.shields.io/github/stars/Acelogic/daVinci-MagiHuman-mlx?style=flat&label=%E2%98%85&color=555) |
| **[macgtop](https://github.com/Acelogic/macgtop)** | `htop` for the Apple Silicon GPU, via private IOReport APIs | ![](https://img.shields.io/github/stars/Acelogic/macgtop?style=flat&label=%E2%98%85&color=555) |

## 📈 Markets

- **[Earnings-Volatility-Calculator](https://github.com/Acelogic/Earnings-Volatility-Calculator)** — Scores options setups around earnings (IV30/RV30, ATR, Yang-Zhang volatility) as Recommended, Consider or Avoid.
- **[Testfol-MarginStresser](https://github.com/Acelogic/Testfol-MarginStresser)** — Portfolio backtester that models margin and taxes.
- **[Market Drawdown Dashboard](https://mcruz.me/market-drawdown-dashboard/)** — Live drawdowns from all-time highs for the S&P 500, Nasdaq 100 and Nasdaq Composite, compared against intra-year drawdowns back to 1928.
- **[Maginator](https://github.com/Acelogic/Maginator)** · **[WayBackMachineStockScraper](https://github.com/Acelogic/WayBackMachineStockScraper)** — A $MAGS ETF price projector, and a tool that recovers price history for delisted tickers from archived Yahoo Finance CSVs.

## 🛠️ Mac Apps & Tools

- **[Ignition](https://github.com/Acelogic/Ignition)** — A native SwiftUI manager for launchd agents and daemons, and a free alternative to LaunchControl.
- **[reddit-youtube-comments](https://github.com/Acelogic/reddit-youtube-comments)** — Shows Reddit threads under YouTube videos. A clean replacement for the malicious Comet extension.
- **[pi](https://github.com/earendil-works/pi) extensions** — [pi-lm-studio](https://github.com/Acelogic/pi-lm-studio) · [pi-statusline](https://github.com/Acelogic/pi-statusline) · [pi-memories](https://github.com/Acelogic/pi-memories) · [pi-claude-memories](https://github.com/Acelogic/pi-claude-memories) · [pi-cd](https://github.com/Acelogic/pi-cd) · [pi-buddy](https://github.com/Acelogic/pi-buddy)

---

## 🌍 Upstream

Merged contributions to projects I use:

| Project | Contribution |
|---|---|
| [aurora-silicon/linux](https://github.com/aurora-silicon/linux/pulls?q=is%3Apr+author%3AAcelogic+is%3Amerged), [m1n1](https://github.com/aurora-silicon/m1n1/pulls?q=is%3Apr+author%3AAcelogic+is%3Amerged), [u-boot](https://github.com/aurora-silicon/u-boot/pulls?q=is%3Apr+author%3AAcelogic+is%3Amerged) | 25 patches of M5/M6/J700 bring-up |
| [FDH2/UxPlay](https://github.com/FDH2/UxPlay/pull/490) | Native macOS AirPlay renderer on VideoToolbox + Metal ([#490](https://github.com/FDH2/UxPlay/pull/490), [#497](https://github.com/FDH2/UxPlay/pull/497), [#505](https://github.com/FDH2/UxPlay/pull/505)) |
| [sharpemu/sharpemu](https://github.com/sharpemu/sharpemu/pull/216) | Extended PS5 runtime and AGC/Vulkan rendering compatibility |
| [wagonbomb/kawaiidra-mcp](https://github.com/wagonbomb/kawaiidra-mcp/pulls?q=is%3Apr+author%3AAcelogic+is%3Amerged) | JPype bridge to Ghidra (100–1000× faster), Ghidra 12 support, iOS research tools (7 PRs) |
| [astral-sh/ruff](https://github.com/astral-sh/ruff/pull/23899) | `pep8-naming` checks for `match` pattern bindings |
| [exo-explore/exo](https://github.com/exo-explore/exo/pull/1706) | Partial download progress on initial dashboard load |
| [0xMiden/miden-vm](https://github.com/0xMiden/miden-vm/pull/2838) | Reject `@locals` values that overflow word alignment |
| [majd/homebrew-repo](https://github.com/majd/homebrew-repo/pull/5) | Fixed macOS dependency syntax for ipatool |

---

## 📊 GitHub Stats

[![Profile Details](https://raw.githubusercontent.com/Acelogic/Acelogic/master/profile-summary-card-output/github_dark/0-profile-details.svg)](https://github.com/vn7n24fzkq/github-profile-summary-cards)

<details>
<summary>📈 More Stats</summary>
<br>

[![Repos Per Language](https://raw.githubusercontent.com/Acelogic/Acelogic/master/profile-summary-card-output/github_dark/1-repos-per-language.svg)](https://github.com/vn7n24fzkq/github-profile-summary-cards)
[![Most Commit Language](https://raw.githubusercontent.com/Acelogic/Acelogic/master/profile-summary-card-output/github_dark/2-most-commit-language.svg)](https://github.com/vn7n24fzkq/github-profile-summary-cards)

[![Stats](https://raw.githubusercontent.com/Acelogic/Acelogic/master/profile-summary-card-output/github_dark/3-stats.svg)](https://github.com/vn7n24fzkq/github-profile-summary-cards)
[![Productive Time](https://raw.githubusercontent.com/Acelogic/Acelogic/master/profile-summary-card-output/github_dark/4-productive-time.svg)](https://github.com/vn7n24fzkq/github-profile-summary-cards)

</details>

---

## 🤝 Let's Connect

[![Website](https://img.shields.io/badge/-mcruz.me-111111?style=flat&logo=googlechrome&logoColor=white)](https://mcruz.me)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mcruz4600/)
[![X](https://img.shields.io/badge/-X-000000?style=flat&logo=x&logoColor=white)](https://x.com/Acelogic_)
[![Email](https://img.shields.io/badge/-Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:miguelc4600@gmail.com)

---

> *"Always open to new challenges and collaborations. Reach out if you'd like to build something together."*
