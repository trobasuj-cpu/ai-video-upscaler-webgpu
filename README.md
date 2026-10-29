# AI Video Upscaler — Browser WebGPU & Cloud RTX 4090 Super-Resolution

[![Live App - upscalex.video](https://img.shields.io/badge/Live_WebGPU_App-upscalex.video-059669?style=for-the-badge)](https://upscalex.video/?utm_source=github&utm_medium=readme)
[![Cloud RTX 4090 - fast.upscalex.video](https://img.shields.io/badge/Cloud_RTX_4090-fast.upscalex.video-0891b2?style=for-the-badge)](https://fast.upscalex.video/?utm_source=github&utm_medium=readme)
[![Architecture Docs](https://img.shields.io/badge/Architecture-WebGPU_%2B_WebCodecs-0f172a?style=for-the-badge)](https://upscalex.video/technical/architecture/?utm_source=github&utm_medium=readme)

![UpscaleX 720p vs 4K Ultra HD Comparison](https://upscalex.video/assets/press/slide-1-hero-720p-vs-4k.png)

**UpscaleX Video** is a dual-engine AI video & image super-resolution web suite built for creators, archivists, and AI video workflows (`Sora`, `Runway Gen-3`, `Kling`, `Veo`, `Pika`, `Wan`).

---

## Architecture & Live Endpoints

| Engine | Live URL | Compute Stack | Best Use Case | Pricing |
| :--- | :--- | :--- | :--- | :--- |
| **Client-Side WebGPU Engine** | **[upscalex.video](https://upscalex.video/?utm_source=github&utm_medium=readme)** | WGSL CNN Compute Shaders + WebGL2 Fallback + Hardware `WebCodecs` MP4/AAC Muxer | 100% private zero-upload clips, instant browser enhancement, zero watermarks | **100% Free** (No Signup) |
| **Serverless RTX 4090 Cloud** | **[fast.upscalex.video](https://fast.upscalex.video/?utm_source=github&utm_medium=readme)** | Dedicated NVIDIA RTX 4090 (24 GB VRAM) + `Real-ESRGAN` FP16 `3×3` Frame Montages | Long 4K 60fps videos, 25-video batch queues, mobile/lightweight laptops, live 4K crop preview | **Pay-As-You-Go** (from $0.01) |

---

## Specialized AI Super-Resolution Pipelines

- **[Upscale Video to 4K Ultra HD (3840×2160)](https://upscalex.video/upscale-video-to-4k/?utm_source=github&utm_medium=readme)** — Reconstruct 720p and 1080p H.264/HEVC streams to true 2160p MP4 with preserved stereo AAC audio.
- **[Free Online AI Video Enhancer](https://upscalex.video/video-enhancer/?utm_source=github&utm_medium=readme)** — Remove 8×8 DCT macroblocking, mosquito noise, and motion softness.
- **[AI-Generated Video Upscaler (Sora / Runway / Kling / Veo)](https://upscalex.video/ai-generated-video-upscaler/?utm_source=github&utm_medium=readme)** — Upgrade native 720p generative video outputs to crisp 4K delivery masters.
- **[Restore Old VHS, MiniDV & Camcorder Footage](https://upscalex.video/restore-old-video/?utm_source=github&utm_medium=readme)** — Clean archival family and documentary footage.
- **[Anime & 2D Animation 4K Upscaler](https://upscalex.video/anime-video-upscaler/?utm_source=github&utm_medium=readme)** — Dedicated `realesr-animevideov3` line-art reconstruction without ringing halos.
- **[4K AI Image Upscaler (PNG / JPG / WebP)](https://upscalex.video/image-upscaler/?utm_source=github&utm_medium=readme)** — Instant 2× and 4× still-frame super-resolution in the browser.
- **[WebGPU Browser Setup & Compatibility Guide](https://upscalex.video/enable-webgpu/?utm_source=github&utm_medium=readme)** — Enable hardware acceleration across Chrome, Edge, Brave, Safari, Windows, macOS, and Linux.
- **[Technical Architecture Whitepaper](https://upscalex.video/technical/architecture/?utm_source=github&utm_medium=readme)** — Deep-dive into deterministic `VideoDecoder`/`VideoEncoder` microsecond muxing and 3×3 RTX 4090 montage batching.

---

## Browser Requirements for Local WebGPU Mode

- **Chrome / Edge / Brave 113+** on Windows (Direct3D 12), macOS (Apple Silicon Metal), or Linux (Vulkan)
- **Safari 18+** on macOS Sequoia / iOS 18+
- Automatic **WebGL2** shader fallback on older devices, plus seamless handoff to **[fast.upscalex.video](https://fast.upscalex.video/?utm_source=github&utm_medium=readme)** for heavy cloud GPU workloads.
