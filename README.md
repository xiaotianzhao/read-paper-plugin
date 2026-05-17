# read-paper — Claude Code Plugin

A Claude Code plugin that provides deep academic paper analysis with bilingual (English/Chinese) output.

## What it does

When you share a research paper — via PDF path, pasted text, or arXiv link — this skill produces a structured five-section analysis report and saves it to `~/Papers/`:

1. **背景 (Context)** — Key abstract sentences with Chinese translation and synthesis
2. **相关工作 (Related Work)** — Prior work organized by theme
3. **核心贡献 (Contributions)** — Verbatim contribution statements with translations
4. **核心方案 (Methods)** — Deep method explanation with architecture diagram, key technical details, and training setup
5. **实验与消融 (Experiments & Ablation)** — Setup, main results, ablations, conclusions

## Installation

```bash
/plugin install read-paper@github:zhaoxiaotian0701/read-paper-plugin
```

Or browse via `/plugin > Discover` if this plugin is listed in a marketplace.

## Usage

Trigger phrases (Chinese or English both work):

- `帮我读这篇论文 /path/to/paper.pdf`
- `分析这篇paper: https://arxiv.org/abs/xxxx.xxxxx`
- `read this paper` + paste abstract or full text
- `总结这篇文章`

The skill saves a `.md` report to `~/Papers/<paper-title>.md` and tells you the path when done.

## Requirements

- Claude Code with skill support
- For PDF input: the `anthropic-skills:pdf` skill must be available (built-in to Claude Code)

## License

MIT
