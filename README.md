# RECON UGC skills

Companion skills for [RECON UGC](https://reconugc.com) — they teach your AI
assistant how to use RECON well: research what is working on TikTok, benchmark
competitors, and turn findings into a shoot brief.

## Install

```bash
npx skills add ottiwroteit/recon-skills
```

Works with Claude Code, Cursor, and Codex.

## Connect RECON first

The skills need access to your RECON account. Either:

**Remote connector (easiest).** In Claude: Settings → Connectors → Add custom
connector, paste `https://reconugc.com/mcp`, sign in, Allow.

**CLI.** For Claude Code, Codex, and anything that runs a local connector:

```bash
npm i -g @reconugc/cli
reconugc auth login
```

Requires a paid RECON plan.

## The skills

| Skill | Use it for |
|---|---|
| `recon-research` | Find what is working and explain why — search the library, read beat-by-beat breakdowns |
| `recon-competitors` | Benchmark against tracked rivals, head-to-head verdicts, format gaps |
| `recon-brief` | Turn findings into hooks, beats, and a shot list grounded in real outliers |

## The idea they all encode

RECON scores every video by how far it beat **its own creator's** normal reach —
the outlier score. A 40M-view video from a huge account is unremarkable. A 60K-view
video that scored 32x did something you can copy.

These skills keep your assistant judging on that number instead of raw view counts,
and keep it citing real indexed videos instead of inventing trends.

## Setup guide

Full instructions: [reconugc.com/faq#mcp-access](https://reconugc.com/faq#mcp-access)

## License

MIT
