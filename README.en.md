# metric-alignment-advisor

A personal advisor Skill for reviewing `KPI / OKR / evaluation schemes / operational metrics`.

It is not a generic management advisor. Its job is to judge whether a set of goals and metrics will push a team in the wrong direction, especially by identifying:

- metrics replacing goals
- Goodhart effects
- gaming, vanity metrics, completion-rate inflation
- short-term optimization killing long-term value
- incentive misalignment
- local optimization hurting the whole system
- hiding risk instead of surfacing it

## Use Cases

Useful for prompts like:

- Help me review whether these KPIs / OKRs make sense
- Will this metric design drive the wrong behavior?
- Why is the team working hard but the outcomes getting stranger?
- What bad behavior will this evaluation scheme induce?
- Will these metrics encourage gaming, blame-shifting, or short-termism?

## Output Style

This Skill is designed as a strong-judgment personal advisor:

- judgment first, explanation second
- no vague balancing language
- call out the most dangerous issues directly
- recommend what to `keep / remove or downgrade / add as guardrails`

## Repository Structure

```text
metric-alignment-advisor/
├── README.md
├── README.en.md
└── metric-alignment-advisor/
    ├── SKILL.md
    └── references/
        └── examples.md
```

## Installation

### Install into Codex

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo Qianxiao7135/metric-alignment-advisor \
  --path metric-alignment-advisor
```

### Install into Claude Code

Copy the `metric-alignment-advisor/` directory into your user-level skills directory, for example:

- `~/.claude/skills/metric-alignment-advisor`

## Core Questions This Skill Answers

1. What is the real goal?
2. What are the current metrics actually proxying?
3. Where will Goodhart effects appear?
4. What behavior distortions will they induce?
5. What should be removed, kept, or added?

## Version

Current version: `v1`
