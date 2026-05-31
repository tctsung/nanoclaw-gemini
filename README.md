# NanoClaw (Gemini + OpenCode)

> No Claude Code. No credit card. One API key and one command.

A fork of [nanocoai/nanoclaw](https://github.com/nanocoai/nanoclaw) for people who don't have (or don't want to pay for) an Anthropic API key, bypassing the original setup's reliance on Claude Code

Pre-installed skills in this branch

- **OpenCode provider** — **Google Gemini** as the LLM backend (free tier: 1500 req/day)
- **Telegram channel** — message your agent from your phone (or choose other channels through `bash nanoclaw.sh`)

## Quick Start

1. **Clone this branch:**
```bash
git clone -b gemini-opencode https://github.com/tctsung/nanoclaw.git nanoclaw-v2
cd nanoclaw-v2
```

2. **Set up your API key:**
```bash
cp .env.example .env
nano .env
```

3. **Run the installation script:**

> **⚠️ IMPORTANT:** When the script asks *"How would you like to connect to Claude?"* — **select Skip**. We are using Gemini + OpenCode instead.
```bash
bash nanoclaw.sh
```

---
*Note: This branch is maintained as a clean template. Create a separate personal branch to store your own configuration and agent memories.*

## License

MIT

<img referrerpolicy="no-referrer-when-downgrade" src="https://static.scarf.sh/a.png?x-pxid=47894bd5-353b-42fe-bb97-74144e6df0bf" />
