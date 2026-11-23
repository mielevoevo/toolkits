# Toolkits

Tools and configurators used by me

## AI Skills (ai-skills)
- **[anti-slop](./ai-skills/anti-slop)** — Output guardrails and anti-slop prompt rules for cleaner LLM responses.
- **[claude-skills-llm-council](./ai-skills/claude-skills-llm-council)** — Multi-LLM council deliberation skill for structured reasoning workflows.

## Selective Pull (Sparse Checkout)
Pull only a specific module without cloning the entire repository:

```bash
git clone --filter=blob:none --no-checkout https://github.com/mielevoevo/toolkits.git
cd toolkits
git sparse-checkout init --cone
git sparse-checkout set ai-skills/<module-name>
git checkout main
