# Toolkits

Tools and configurators used by me

## AI Skills (`ai-skills/`)
- **[anti-slop](./ai-skills/anti-slop)** — Output guardrails and anti-slop prompt rules for cleaner LLM responses.
- **[claude-skills-llm-council](./ai-skills/claude-skills-llm-council)** — Multi-LLM council deliberation skill for structured reasoning workflows.
- **[impeccable](https://github.com/pbakaus/impeccable)** — Frontend design vocabulary and UI critique/polish skill for coding agents.

## macOS Utilities (`mac-utility/`)
- **[vorssaint-utils](./mac-utility)** — Native Swift menu bar utility suite (`brew install --cask vorssaint`).

## Selective Pull (Sparse Checkout)
Pull only a specific module without cloning the entire repository:

```bash
git clone --filter=blob:none --no-checkout https://github.com/mielevoevo/toolkits.git
cd toolkits
git sparse-checkout init --cone
git sparse-checkout set ai-skills/<module-name>
git checkout main
```
