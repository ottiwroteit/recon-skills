# RECON UGC skills

Companion skills for [RECON UGC](https://reconugc.com). They teach your AI
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

## What the connector can do

| Tool | What it does |
|---|---|
| `search_videos` | Search viral TikToks by niche, format, tone, or free text |
| `get_breakdown` | Beat-by-beat breakdown of one video: hook, mechanism, why it worked |
| `compare_videos` | Why one video beat another, head to head |
| `competitor_report` | Your competitor board: rank, engagement, top format, share of voice |
| `trending` | The newest breakouts across your niches |
| `write_hooks` | TikTok hooks for your product, grounded in the top real hooks in your category |
| `meta_ads` | **New.** The Facebook and Instagram ads any brand you name is running, longest-running first |

`write_hooks` and `meta_ads` are available through the remote connector. The CLI
covers the first five.

Meta publishes no views or spend for ads, so `meta_ads` ranks by how long each ad
has run (brands keep paying for ads that work) and by how many versions are running.

## The skills

| Skill | Use it for |
|---|---|
| `recon-research` | Find what is working and explain why: search the library, read beat-by-beat breakdowns |
| `recon-competitors` | Benchmark against tracked rivals, head-to-head verdicts, format gaps, and the Meta ads a rival is running |
| `recon-brief` | Turn findings into hooks, beats, and a shot list grounded in real outliers |

## The idea they all encode

RECON scores every video by how far it beat **its own creator's** normal reach:
its **Heat Signature**. A 40M-view video from a huge account is unremarkable. A 60K-view
video that scored 32x did something you can copy.

These skills keep your assistant judging on that number instead of raw view counts,
and keep it citing real indexed videos instead of inventing trends.

## Setup guide

Full instructions: [reconugc.com/faq#mcp-access](https://reconugc.com/faq#mcp-access)

## License

MIT
