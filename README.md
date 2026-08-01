## Joshua Gustafson-Juarez

**I build local-first AI infrastructure — systems that run on hardware you already own, and can prove what they did.**

Houston, TX. Field and implementation background: multi-site ownership, customer-facing troubleshooting under P1–P4 SLAs, operations leadership. For the past eight months I've been building and operating a distributed AI system across six machines on a private mesh network — local models with cloud rationed on top, and a governance layer so nothing executes without an explicit gate and everything leaves an audit trail.

Most of that work is private. Here's what I can show you.

---

### 🎼 [Mozart](https://github.com/joshuagjuarez/mozart) · MIT

Turn the computers you already own into a measured local-AI orchestra.

Mozart discovers every machine on your private mesh, benchmarks every model on every node with a uniform prompt, and recommends where each model should actually run. It replaces spec-sheet guessing with measurements from your own hardware. Answer-quality judgment stays with the operator, downloads require approval, and cloud-tagged models default to hold — so a local benchmark can never silently become off-device execution.

`Python` · `Tailscale` · `SSH` · `Ollama` · `macOS / Windows / Linux+WSL`

---

### Things I measured that contradict common advice

Same-prompt benchmarks across mixed consumer hardware:

- **Format beats parameter count on Apple Silicon.** A 35B in MLX beat 20B and 27B GGUF models on the same machine — ~19s vs 46–48s.
- **One consumer GPU box is two inference lanes, not one.** 12GB VRAM + 32GB system RAM runs a 14B at 100% GPU *concurrently* with a second model at 100% CPU. Node throughput roughly doubles.
- **A 1B model beat a 3B on old CPUs** on both speed and quality — 7.2s vs 17s. The right scout model for weak hardware is smaller than intuition says.
- **Residency dominates UX.** Identical query: 32.5s cold-load vs 2.3s hot. Never make a human wait for a model to wake up.
- **The quantization cliff is real.** A 70B at q2 is unusable — over 400 seconds. Parameter count stops meaning anything once quantization butchers it.

Anyone can say "run models locally." Saying *which* model, on *which* hardware, in *which* format, with numbers, is the difference between an opinion and an engineering recommendation.

---

### The record

```
alfred_backend    252 commits    2025-12-27 → 2026-05-26    trading simulation, containerized
memex             553 commits    2026-05-30 → 2026-07-26    AI orchestration + governance
MemexRuntime      140 commits    2026-07-24 → present       the live system
────────────────────────────────────────────────────────────────────────────────
                  945 commits    eight continuous months    three domains
```

Alfred's last commit is four days before Memex's first. No gap.

What I care about, and what shows up in that history: **evidence over assertion.** Receipts for every action, cross-checking a model's output instead of trusting its self-report, and deleting my own work when it turns out to be theater. There's a commit from December 2025 called *"extract deterministic evidence payload builder"* — I've been building the same idea since the first week, in three different domains.

---

### What I'm looking for

AI Solutions Engineer · Forward Deployed Engineer · Applied AI / Solutions Architect · Technical Implementation

Especially where **the data can't leave the building** — energy, healthcare, anything regulated. Running useful AI on infrastructure a company controls, with an audit trail, is the problem I've spent the past eight months on.

Houston or remote. 📫 [joshuagjuarez@gmail.com](mailto:joshuagjuarez@gmail.com)

---

<sub>No CS degree — self-taught, and the commit history is the transcript. Most repositories here are private because they contain network topology and business material; Mozart is the public code sample and I'm happy to walk through the rest in a conversation.</sub>
