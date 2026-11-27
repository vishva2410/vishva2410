<!-- ══════════════════════════════════════════════════════════════
     HERO
════════════════════════════════════════════════════════════════ -->

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=220&section=header&text=Vishva%20Teja%20G.&fontSize=72&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Backend%20%26%20AI%20Engineer&descAlignY=58&descSize=20" width="100%" />
</div>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=22&duration=2800&pause=800&color=00D9FF&center=true&vCenter=true&width=850&lines=%24+whoami;%3E+backend+%26+ai+engineer;%24+cat+philosophy.txt;%3E+privacy-first+%7C+low-latency+%7C+production-grade;%24+./deploy+--target%3Dthe-real-world;%3E+shipping%2C+not+just+training" alt="Typing Animation" />
</div>

<div align="center">
  <a href="https://linkedin.com/in/vishva-teja-guduguntla"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://github.com/vishva2410"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
  <a href="https://leetcode.com/u/vishva_guduguntla/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" /></a>
  <a href="mailto:vishvateja10@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <img src="https://komarev.com/ghpvc/?username=vishva2410&style=for-the-badge&color=00D9FF&label=Views" />
</div>

<br>

> ### "The model is the easy part. Making it run in 200ms on a CPU, inside someone else's office, with their data never leaving the room — *that's* the job."

<div align="center">
  <img src="https://img.shields.io/badge/🔭_Building-Local--first_AI-00D9FF?style=for-the-badge" />
  <img src="https://img.shields.io/badge/🌱_Learning-Distributed_Inference-7F5AF0?style=for-the-badge" />
  <img src="https://img.shields.io/badge/💬_Open_to-SWE_%2F_AI_Roles-2CB67D?style=for-the-badge" />
</div>

<br>

<div align="center">

| 🎯 **Focus** | 🧪 **Experimenting** | 📚 **Reading** | ☕ **Fuel** |
|:---:|:---:|:---:|:---:|
| Inference optimization | Agentic RAG pipelines | *Designing Data-Intensive Applications* | Lo-fi + rain |

</div>

<div align="center">
  <img src="https://img.shields.io/badge/CGPA-8.99%2F10-00D9FF?style=flat-square&logo=bookstack&logoColor=white" />
  <img src="https://img.shields.io/badge/DSA-600%2B_Solved-FFA116?style=flat-square&logo=leetcode&logoColor=black" />
  <img src="https://img.shields.io/badge/LeetCode_Rating-1475-FFA116?style=flat-square&logo=leetcode&logoColor=black" />
  <img src="https://img.shields.io/badge/Publications-1-7F5AF0?style=flat-square&logo=readthedocs&logoColor=white" />
</div>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=6,11,20&height=3" width="100%" />

<!-- ══════════════════════════════════════════════════════════════
     CURRENT STATUS
════════════════════════════════════════════════════════════════ -->

### `~/current-status`

vishva@dev ~ % ./status.sh

  ▶ ROLE      B.Tech CS (Data Science) · Vardhaman College of Engineering
  ▶ FOCUS     Local-first AI · Inference optimization · Modular backends
  ▶ SHIPPING  VoidBox v2 · Bodha AI · OncoDetect modules
  ▶ READING   Designing Data-Intensive Applications
  ▶ MOOD      caffeine.pid [running] ████████████░ 92%


<!-- ══════════════════════════════════════════════════════════════
     MANIFESTO
════════════════════════════════════════════════════════════════ -->

## 🧭 How I Think

- **Latency is a feature.** Sub-2s isn't a benchmark — it's the line between a tool people use and one they abandon.
- **Local beats cloud when data is sensitive.** Not every problem should be an API call.
- **Modularity is a kindness.** Onboarding a new capability shouldn't require touching the core.
- **False negatives are worse than false positives** — especially in PII and clinical pipelines.
- **Ship. Then optimize.** A working prototype teaches more than a perfect plan.

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=6,11,20&height=3" width="100%" />

<!-- ══════════════════════════════════════════════════════════════
     FEATURED BUILDS
════════════════════════════════════════════════════════════════ -->

## ⚡ Featured Builds

<details open>
<summary><h3>🔒 VoidBox — Privacy-First PII Redaction Engine</h3></summary>

> **Problem.** Compliance-sensitive documents can't leave the building. Cloud OCR is a non-starter.
> **Build.** A fully local pipeline that detects & redacts **11+ PII categories** without a single network call.

**⚙️ Architecture**

```mermaid
flowchart LR
    A([Document]) --> B[YOLOv8<br/>Region Detector]
    B --> C[EasyOCR<br/>Text Extractor]
    B --> D[Regex<br/>Classifier]
    C --> E{Evidence<br/>Merger}
    D --> E
    E --> F[LaMa<br/>Neural Inpainting]
    F --> G([Redacted Output])

    style A fill:#00D9FF,stroke:#007ACC,color:#000
    style G fill:#2CB67D,stroke:#1a7f57,color:#fff
    style B fill:#EE4C2C,stroke:#b0301f,color:#fff
    style C fill:#5C3EE8,stroke:#3a28a3,color:#fff
    style F fill:#7F5AF0,stroke:#4b3599,color:#fff
```

**📊 Benchmarks**

| Metric | Result |
|---|---|
| Inference (CPU) | **< 2s / image** |
| PII categories | **11+** |
| False negatives | **0** across 200-doc set |
| Cloud dependency | **None** |

**🧠 Hard parts solved**
- Tuning OCR + regex fusion so overlapping detections don't double-redact
- Getting LaMa to inpaint *legibly* on dense text regions
- Keeping the whole thing CPU-bound so it runs on the user's laptop

`PyTorch` `YOLOv8` `EasyOCR` `LaMa` `OpenCV`

[**→ Browse the repo**](https://github.com/vishva2410/VOID-BOX)

</details>

---

<details open>
<summary><h3>🎙️ Bodha AI — Real-Time Conversational Voice Assistant</h3></summary>

> **Problem.** Real conversation needs < 300ms round-trip — anything slower feels like talking to a transcript.
> **Build.** A streaming voice AI engine on live audio protocols, with multi-turn context that doesn't fall apart after turn three.

**⚙️ Sequence**

```mermaid
sequenceDiagram
    participant U as User
    participant C as Client
    participant L as LiveKit
    participant N as NLP Engine
    participant T as TTS

    U->>C: speaks
    C->>L: stream audio
    L->>N: transcribe + route
    N->>N: update context
    N->>T: generate reply
    T->>L: stream audio
    L->>U: hears response
```

**📊 Benchmarks**

| Metric | Result |
|---|---|
| End-to-end latency | **< 300ms** |
| Conversation continuity | **95%+** |
| Transport | LiveKit + WebSockets |
| Context model | Multi-turn NLP |

**🧠 Hard parts solved**
- Keeping streaming stable across packet jitter
- Keeping context coherent without ballooning token cost
- Synchronizing TTS playback with barge-in

`LiveKit` `WebSockets` `NLP` `Python`

[**→ Browse the repo**](https://github.com/vishva2410/bodha_ai_1)

</details>

---

<details>
<summary><h3>🩺 OncoDetect — Modular Cancer Diagnostic Pipeline</h3></summary>

> **Problem.** Every hospital wants a "cancer AI," but every organ gets its own bespoke pipeline. That doesn't scale.
> **Build.** A plug-and-play diagnostic framework where adding a new organ module requires **zero** changes to the core pipeline.

**⚙️ Architecture**

```mermaid
flowchart TD
    A([Patient Data]) --> B{Organ<br/>Router}
    B -->|Lung| C[Lung Model]
    B -->|Breast| D[Breast Model]
    B -->|Skin| E[Skin Model]
    B -->|+ new| F[Any New Module]
    C --> G[Unified Output Interface]
    D --> G
    E --> G
    F --> G
    G --> H([Clinical Report])

    style A fill:#00D9FF,color:#000
    style H fill:#2CB67D,color:#fff
    style F fill:#7F5AF0,color:#fff
```

**🧠 Hard parts solved**
- Unified prediction contract so new modules "just fit"
- End-to-end clinical report generation from raw model outputs
- Outputs structured to be consumed by downstream reporting tools

`PyTorch` `FastAPI` `Computer Vision`

[**→ See on GitHub**](https://github.com/vishva2410)

</details>

---

<details>
<summary><h3>🔥 DynaCalorie AI — Adaptive Metabolic Engine</h3></summary>

> **Problem.** Every TDEE calculator lies — because human metabolism drifts.
> **Build.** A tracker that learns from its own prediction errors and recalibrates bi-weekly.

**⚙️ Feedback Loop**

```mermaid
flowchart LR
    I([Intake Log]) --> B[TDEE Estimator]
    W([Weight Check-in]) --> D{Delta<br/>Analyzer}
    B --> D
    D -->|recalibrate| B
    B --> F[12-Week Forecast]
    D --> S[Safety Thresholds]
    S -->|flag| I
    F --> O([Projection])

    style I fill:#00D9FF,color:#000
    style O fill:#2CB67D,color:#fff
    style D fill:#7F5AF0,color:#fff
```

**📊 Benchmarks**

| Metric | Result |
|---|---|
| Accuracy vs. static TDEE | **+12% over 12 weeks** |
| Recalibration cadence | Bi-weekly |
| Safety | Flags unhealthy loss rates & low protein |

`Python` `Forecasting` `Health ML`

[**→ Browse the repo**](https://github.com/vishva2410/Dyna-Calorie)

</details>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=6,11,20&height=3" width="100%" />

<!-- ══════════════════════════════════════════════════════════════
     TECH RADAR
════════════════════════════════════════════════════════════════ -->

## 🛰️ Tech Radar

<div align="center">
  <img src="https://skillicons.dev/icons?i=py,java,cpp,mysql,pytorch,tensorflow,opencv,sklearn,fastapi,flask,docker,aws,postgres,git,github,linux&theme=dark&perline=8" />
</div>

<table>
<tr>
<td width="50%" valign="top">

**🧬 AI / ML**
- PyTorch · TensorFlow · scikit-learn
- Computer Vision · YOLOv8 · OpenCV · EasyOCR
- NLP · LLMs · multi-turn context
- LaMa inpainting · segmentation

</td>
<td width="50%" valign="top">

**⚙️ Backend & Infra**
- FastAPI · Flask · REST · WebSockets · LiveKit
- Docker · AWS (EC2, S3) · Linux
- PostgreSQL · MySQL · Pandas · NumPy
- Git · Postman · Tableau

</td>
</tr>
</table>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=6,11,20&height=3" width="100%" />

<!-- ══════════════════════════════════════════════════════════════
     LIVE METRICS
════════════════════════════════════════════════════════════════ -->

## 📈 Live Metrics

<div align="center">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=vishva2410&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&bg_color=00000000&title_color=00D9FF&icon_color=7F5AF0" />
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=vishva2410&layout=compact&theme=tokyonight&hide_border=true&langs_count=8&bg_color=00000000&title_color=00D9FF" />
</div>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=vishva2410&theme=tokyonight&hide_border=true&background=00000000&ring=00D9FF&fire=7F5AF0&currStreakLabel=00D9FF" width="60%" />
</div>

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=vishva2410&theme=tokyo-night&hide_border=true&area=true&bg_color=00000000&color=00D9FF&line=7F5AF0&point=00D9FF" width="100%" />
</div>

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=vishva2410&theme=tokyonight&no-frame=true&no-bg=true&column=7&row=1&margin-w=8" />
</div>

<!-- 🐍 OPTIONAL: snake animation
     Setup → https://github.com/Platane/snk (add the provided workflow, then uncomment)

<picture>
  <source media="(prefers-color-scheme: dark)"  srcset="https://raw.githubusercontent.com/vishva2410/vishva2410/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/vishva2410/vishva2410/output/github-snake.svg" />
  <img alt="snake" src="https://raw.githubusercontent.com/vishva2410/vishva2410/output/github-snake.svg" />
</picture>
-->

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=6,11,20&height=3" width="100%" />

<!-- ══════════════════════════════════════════════════════════════
     TIMELINE
════════════════════════════════════════════════════════════════ -->

## 🗺️ Timeline

```mermaid
timeline
    title The Path So Far
    2023 : Started B.Tech CS (Data Science) @ Vardhaman College of Engineering
    2024 : Data Analyst Intern @ CraftyourCareer
    2025 : Shipped VoidBox, Bodha AI, OncoDetect
         : Published in IJSAT (Green Morph Solutions)
         : College AI Hackathon — Winner
         : Smart India Hackathon 2025 — Finalist
    2026 : Open to SWE / AI Engineer roles
```

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=6,11,20&height=3" width="100%" />

<!-- ══════════════════════════════════════════════════════════════
     RECEIPTS
════════════════════════════════════════════════════════════════ -->

## 🏆 Receipts

| Type | Detail |
|---|---|
| 📄 **Publication** | *Green Morph Solutions* — IJSAT Vol. 16, Issue 2 · [DOI: 10.71097/IJSAT.v16.i2.4382](https://doi.org/10.71097/IJSAT.v16.i2.4382) |
| 🥇 **Win** | College-level AI Hackathon |
| 🚀 **Finalist** | Smart India Hackathon 2025 |
| 🎤 **Debate** | 10+ tournament wins — pressure-tested reasoning |
| 💼 **Industry** | CraftyourCareer — cut bounce rate **18%** with engagement analytics |
| 🧮 **DSA** | **600+** problems solved (LeetCode 310 · GFG 212 · Codeforces · college platform) |

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=6,11,20&height=3" width="100%" />

<!-- ══════════════════════════════════════════════════════════════
     CTA
════════════════════════════════════════════════════════════════ -->

## 💬 Let's Talk

Whether it's inference latency, privacy-first AI, or just interesting systems — my inbox is open.

<div align="center">
  <a href="mailto:vishvateja10@gmail.com"><img src="https://img.shields.io/badge/vishvateja10@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://linkedin.com/in/vishva-teja-guduguntla"><img src="https://img.shields.io/badge/Message_me_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
</div>

<br>

<div align="center">
  <sub>⭐ If any of my repos helped you, a star goes a long way.</sub>
</div>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer&text=Thanks%20for%20scrolling&fontSize=20&fontColor=ffffff" width="100%" />
</div>
```
