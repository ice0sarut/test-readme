🌀 VibeObs (v0.1.0-alpha)
The Observability Tool for Vibe Coders. Stop staring at complex dashboards. Start feeling the "vibe" of your system through AI-powered summaries and proactive insights.

🚀 Why VibeObs?
Traditional monitoring tools (Prometheus + Grafana) are great, but they require heavy setup and cognitive load. VibeObs is built for developers who want to focus on shipping code, not configuring panels.

Zero-Dashboard Policy: Get human-readable status updates via Telegram/Discord.

AI-First Root Cause: When a panic occurs, VibeObs doesn't just alert; it tells you why and suggests a fix.

High Performance: Powered by Vector (Rust) and VictoriaMetrics (Go) for industry-leading efficiency.

Karpenter Friendly: Native support for EKS node scaling insights.

🛠 Tech Stack
Collector: Vector (High-performance observability data pipeline)

Storage: VictoriaMetrics (Cost-effective time-series DB)

Analysis: Go (Golang) + LLM Integration

Notification: Telegram / Discord / Slack

📦 Quick Start
1. Prerequisites
Docker & Docker Compose

OpenAI API Key (or Local LLM via Ollama)

A Bot Token (Telegram/Discord)

2. Installation
Bash
# Clone the repository
git clone https://github.com/yourusername/vibeobs.git
cd vibeobs

# Setup environment variables
cp .env.example .env
# Edit .env with your API Keys and Bot Tokens
3. Deploy
Bash
docker-compose up -d
4. Instrument your App
Send your logs/metrics to localhost:2259 (Vector default port).

Go
// Example for Go
log.Printf("VIBE_CHECK: {status: 'ok', latency: '150ms'}")
🧠 Features
Vibe Summary: A daily human-like report of your system's health.

Anomaly Detection: AI identifies unusual patterns before they become outages.

Cost Guard: Notifies you if your cloud infra (AWS/EKS) is burning more credits than usual.

🤝 Contributing
We love contributions! Whether it's adding a new integration or improving the AI prompts, feel free to:

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingVibe)

Commit your Changes (git commit -m 'Add some AmazingVibe')

Push to the Branch (git push origin feature/AmazingVibe)

Open a Pull Request

📄 License
Distributed under the MIT License. See LICENSE for more information.

✨ Built by Developers, for Developers.
"Don't let your metrics ruin your vibe." — The VibeObs Team
