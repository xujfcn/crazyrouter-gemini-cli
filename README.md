# 💎 Gemini CLI + Crazyrouter Setup Guide

> Use Google Gemini CLI through Crazyrouter — Save 45% on Gemini API costs.

[Crazyrouter](https://crazyrouter.com?ref=github) — One API key, 300+ models, 45% cheaper.

## 💰 Price Comparison

| Model | Official (In/Out per 1M tokens) | Crazyrouter | Savings |
|-------|--------------------------------|-------------|---------|
| Gemini 2.5 Pro | $1.25 / $10 | $0.69 / $5.50 | **45%** |
| Gemini 2.5 Flash | $0.15 / $0.60 | $0.08 / $0.33 | **45%** |
| Claude Opus 4 | $15 / $75 | $8.25 / $41.25 | **45%** |
| GPT-4o | $2.50 / $10 | $1.38 / $5.50 | **45%** |

## ⚡ Quick Start

### 1. Install Gemini CLI
```bash
npm install -g @anthropic-ai/gemini-cli
```

### 2. Configure with Crazyrouter
```bash
export GEMINI_API_KEY=sk-your-crazyrouter-key
```

### 3. Run
```bash
gemini
```

## 🔧 Persistent Configuration

```bash
# Add to shell config
cat >> ~/.zshrc << 'EOF'
# Gemini CLI via Crazyrouter
export GEMINI_API_KEY=sk-your-crazyrouter-key
EOF
source ~/.zshrc
```

## 🎯 Why Gemini CLI?

| Feature | Gemini CLI | Claude Code | Codex CLI |
|---------|-----------|-------------|-----------|
| Context Window | **1M tokens** | 200K | 128K |
| Speed | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐ |
| Open Source | ✅ | ❌ | ✅ |
| Best For | Large projects | Complex reasoning | General coding |

Gemini 2.5 Pro has the largest context window (1M tokens), making it ideal for large codebases.

## 🔄 Use All Three CLI Tools with One Key

```bash
# One Crazyrouter key for all three tools
export OPENAI_API_KEY=sk-your-crazyrouter-key
export OPENAI_BASE_URL=https://crazyrouter.com/v1
export ANTHROPIC_API_KEY=sk-your-crazyrouter-key
export ANTHROPIC_BASE_URL=https://crazyrouter.com
export GEMINI_API_KEY=sk-your-crazyrouter-key

# Now use any of them
gemini    # Google Gemini CLI
claude    # Anthropic Claude Code
codex     # OpenAI Codex CLI
```

## ❓ FAQ

**Q: Does Gemini CLI work with Crazyrouter?**
A: Yes, fully compatible.

**Q: Can I use non-Gemini models?**
A: Through Crazyrouter you can access Claude, GPT, and 300+ other models.

**Q: What Node.js version is required?**
A: Node.js 18+ is required.

## 🔗 Links
- 🌐 [Crazyrouter](https://crazyrouter.com?ref=github)
- 💎 [Gemini CLI](https://github.com/google-gemini/gemini-cli)
- 💬 [Telegram](https://t.me/crzrouter)

## 📄 License
MIT

