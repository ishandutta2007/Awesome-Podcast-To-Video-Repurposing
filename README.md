# Awesome-Podcast-To-Video-Repurposing

# Awesome-Podcast-To-Video-Repurposing

# Top Podcast-to-Video Repurposing Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Highlight Extraction, Speaker-Aware Reframing & Caption Burn-In*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Podcast-to-Video Repurposing**. These tools turn long-form audio and video episodes into short, platform-ready clips for YouTube Shorts, TikTok, and Instagram Reels — handling transcription, viral moment detection, speaker-tracking vertical reframing, and burned-in captions automatically.

**Examples** include Opus Clip, Munch, Klap, Vidyo.ai, Castmagic, CapCut, Descript, Riverside.fm, Headliner, and Podcastle (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, local processing, and transparent clip selection — ideal for podcasters who want free, unlimited repurposing without per-minute SaaS pricing or cloud uploads.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Opus Clip](https://www.opus.pro/)**  
  Leading AI podcast clipping platform. Automatically transcribes, identifies viral moments, reframes to vertical with speaker tracking, and burns in animated captions. Free tier is limited by processing minutes and typically watermarks output .

- **[Munch](https://www.getmunch.com/)**  
  AI-powered repurposing platform that extracts highlights from long videos with automatic aspect ratio conversion and caption styling.

- **[Klap](https://klap.app/)**  
  AI video repurposing tool focused on TikTok and Shorts, with automatic highlight detection and vertical reformatting.

- **[Vidyo.ai](https://vidyo.ai/)**  
  Long-to-short video repurposing platform with AI clip selection, auto-captions, and platform-specific aspect ratios.

- **[Castmagic](https://www.castmagic.io/)**  
  AI content repurposing platform that transforms podcasts into show notes, social posts, and short clips.

- **[CapCut](https://www.capcut.com/)**  
  Video editing app with auto-captions, text-to-speech, and template-based short-form creation. Desktop and mobile.

- **[Descript](https://www.descript.com/)**  
  Text-based video and podcast editor with Overdub voice cloning, filler word removal, and clip export.

- **[Riverside.fm](https://riverside.fm/)**  
  Remote recording platform with built-in clip creation, transcription, and social media export.

- **[Headliner](https://www.headliner.app/)**  
  Audiogram and video clip creation tool for podcast promotion with waveform visualizations.

- **[Podcastle](https://podcastle.ai/)**  
  AI-powered podcast creation platform with recording, editing, and video repurposing features.

## Open-Source GitHub Projects

- **[Cutawan](https://github.com/JeremySNR/cutawan)**  
  **Free, open-source desktop video clipper for podcasts and long videos.** MIT licensed. Features AI clip finding via ChatGPT/Codex sign-in or OpenAI API key, local Whisper transcription, speaker-aware reframing with ONNX Runtime, caption styling, auto zoom, and watermarks. **No per-minute caps** — runs on your hardware. Full video is never uploaded; only extracted audio, transcript text, and sampled frames are sent for analysis. Requires no GPU (uses NVENC if available, falls back to CPU). Supports hour-plus recordings via checkpointed chunked transcription .

- **[Podcli](https://github.com/nmbrthirteen/podcli)**  
  **Open-source MCP server and CLI that turns podcasts into upload-ready short clips.** MIT licensed. Transcribes with Whisper (word-level timestamps, pyannote speaker diarization), finds viral moments using Claude or Codex against your show's knowledge base, crops to 1080×1920 with YuNet face detection and speaker-aware tracking, and burns captions in four styles (branded, hormozi, karaoke, subtle). Ships **17 MCP tools** for Claude Code, Claude Desktop, or Codex integration. Handles split-screen and Riverside-style mixed layouts. Runs fully locally, no uploads, no API keys required unless opting into AI clip picking .

- **[Clipify](https://github.com/Siraj-zaki/clipify)**  
  **Turn any YouTube podcast into monetizable 9:16 Shorts — locally, free, and open source.** Pipeline: yt-dlp download → faster-whisper transcription with word timestamps → LLM curator (Ollama/Anthropic/OpenAI) or regex fallback scoring top 25 viral windows → user picks ranks and titles → YuNet face detection + seat clustering for speaker tracking → Hormozi-style .ass captions with yellow current-word highlighting → ffmpeg one-shot render with dynamic crop, pitch shift, mood music mix, and hardware-accelerated H.264 encode. Includes FastAPI backend, workspace isolation, and YouTube metadata sidecar generation .

- **[Shorts Factory](https://pypi.org/project/shorts-factory/)**  
  **Turn one long video into a batch of ready-to-post 9:16 viral shorts — locally, free, offline.** Features faster-whisper transcription with word-level timestamps (cached to JSON for instant re-runs), heuristic virality scoring (question hooks, numbers, power words, speech pace, pause boundaries), optional LLM re-ranking with GPT for titles and hashtags, OpenCV face detection for smart 9:16 reframing, CapCut-style karaoke captions burned via ffmpeg ASS, auto thumbnail generation with sharpness/exposure/face scoring, and report generation in JSON and Markdown. Supports local files and YouTube/URL input via yt-dlp. Requires Python 3.11+ and FFmpeg .

- **[Surivoice](https://pypi.org/project/surivoice/)**  
  **Local-first speech transcription with speaker diarization.** Takes video or audio, transcribes with faster-whisper, identifies speakers with pyannote.audio, and outputs structured Markdown with timestamps. Fully local, no cloud APIs. Features GUI with dark/light theme and CLI. GPU-accelerated with CPU fallback. Supports all major video and audio formats. Requires Hugging Face token for diarization models .

- **[LeGen](https://pypi.org/project/legen/)**  
  **Automated subtitle generation and translation for video and audio.** Uses WhisperX or Whisper for transcription with word-level timestamps, supports translation to multiple languages, and embeds subtitles into video containers. Pulls remote videos or playlists via yt-dlp and embeds every subtitle track found. GPU compatibility with CUDA. Useful for creating captioned content for repurposing workflows .

### Additional Strong Open-Source Options

- **whisply** — Cross-platform Python app for batch transcription, translation, speaker annotation, and subtitle generation. Hardware-optimized (CUDA, Apple Silicon MLX, CPU), supports JSON, RTTM, SRT, VTT, HTML export. Runs entirely locally .
- **MurmurAI** — Self-hosted drop-in replacement for paid transcription APIs. GPU-powered with speaker diarization, word-level timestamps, SRT/VTT/TXT/JSON export, and webhook callbacks .
- **LocalTranscribe** — Offline speaker-labeled transcriptions with one command. Python SDK available for programmatic use .
- **vid2cc-AI** — CLI tool for generating perfectly synced SRT subtitles with hardware acceleration, embed or hardcode options, and batch processing .
- **Auto-clipper** — Auto-find highlights in Twitch/YouTube VODs using YOLO object detection, pixel analysis, and voice-triggered clipping ("clip it"). Includes TikTok vertical export with customizable layouts .

**Frameworks for building custom systems**: Combine **Cutawan** or **Clipify** for the full repurposing pipeline with local processing, **Podcli** for MCP-based agent integration, **Surivoice** or **whisply** for transcription and diarization, **Shorts Factory** for heuristic highlight scoring, and **LeGen** or **vid2cc-AI** for caption generation and embedding to build a complete self-hosted podcast-to-video repurposing stack.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Podcast-to-video repurposing tools must comply with copyright law, platform terms of service (YouTube, TikTok, Instagram), and consent requirements for recording and publishing. **Clip selection AI may produce false positives or miss genuinely viral moments** — human review before publishing is recommended. Guest consent for repurposing recordings should be obtained in advance.
- Self-hosted open-source solutions require proper GPU or CPU resources, FFmpeg installation, and model downloads for local processing.

---

**Made for podcasters, content creators, social media managers, and developers building video repurposing platforms.**  
Let's make podcast-to-video repurposing more open, local-first, and creator-friendly.
