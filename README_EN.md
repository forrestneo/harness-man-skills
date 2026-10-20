# Yurenshu · 驭人术

> **The Art of Managing People — for everyone in the AI era.** A positive management-development system: 70 situations, 700 cases, nine management mindsets, and **two entry points** — bring a specific problem and get an action card (with a three-round game tree); bring only a vague situation and get a full assessment (situation naming + insight-grade output). Works in both Chinese and English.

[中文 README](README.md) · MIT License

---

## The mission: everyone is a manager now

For most of history, most people never managed anyone — management was a skill for the few. The AI era changes that: **everyone now manages intelligent agents.** Management is no longer an elective for leaders; it is basic literacy for everyone.

This library serves both: **learning to manage people is learning to manage AI agents.** Aligning goals, decomposing tasks, accepting deliverables, iterating on feedback, orchestrating collaboration — the five core management moves are identical for human teammates and AI agents (see `references/20-AI时代管理映射.md`). Never managed anyone? Start with AI — it's a zero-cost practice field for management.

## Two entry points, one system

**Entry A · Scenario matching** — when you can name the specific problem ("someone on my team is…"):

1. Restore the scenario → 2. **compound-match 2-4 of the 70 rules** (real situations are never single-rule) → 3. Assess (skill / will / structure) → 4. Action card → 5. **three-round game tree** → 6. Cases
   - Matching example: "a veteran complains about workload *and* slacks off" = Rule 21 + Rule 10 + Rule 26

**Entry B · Situation assessment** — when you can only describe the situation ("I just inherited a mess" / "my team is dead quiet"):

1. **Five-dimension assessment** (structure / power base / people / contradiction / window) → 2. **situation naming** (power vacuum, polite silence, firefighter trap, genius-dependency… naming routes to rules) → 3. core contradiction + your leverage → 4. **30/60/90-day path**
   - Sample output: "Bottom line first: your team doesn't lack problems — it has stopped reporting them. Silence isn't harmony; it's energy-saving." (Name: polite silence)

Both entries land on the 70 rules — assessment only translates and prioritizes; the methods always come from the seventy.

## The three-round game trees (the game layer)

Every method plays out as a **full game tree**: a move plus a counter is one round; three rounds, with each follow-up chaining off the flaw in the previous counter, converging on an equilibrium. Example (Rule 10 · random audits):

> Move: audit deliverables at random → Counter: performative busyness → Chain: audit external metrics (performance only fools insiders) → Counter: court downstream colleagues for good words → Chain: push metrics to terminal outcomes (faking now costs more than working) → Counter: return to real work. **Equilibrium**: by raising the cost of faking, the audit makes honesty the cheapest option — then retires.

Running through all of it, the **mirror principle**: only moves that survive being seen through are good moves — transparent, institutionalized methods win even when recognized. In one line: **the Nash equilibrium of management sits where both sides can see the board.**

## What we believe

- **Control earns compliance; growth earns followership.** This library teaches the ability to grow people, not tricks to control them.
- **Management is the discovery of value** (a distillation of Drucker): the 70 so-called "problems" are 70 misplaced values — chronic comparison = competitive drive; the "troublemaker" = conviction; the "veteran slacker" = organizational memory. The library ships a "value-discovery lens" table: find the value first, then apply the method.
- **Boundaries before methods**: five value boundaries (rotation ≠ exile; audits ≠ surveillance; rules public, feedback private; never optimize through informants; sometimes an amicable parting is kinder than forced reform) plus a four-question self-check. This library teaches management, never manipulation.
- **Half Chinese, half global — by design**: 700 cases split between East and West — Huawei and Pang Donglai alongside Toyota and Bridgewater; the *Records of the Grand Historian* alongside Google's Project Aristotle; Drucker alongside the *Zizhi Tongjian*.

## The content matrix

| Layer | Files | What's inside |
|---|---|---|
| Core method library | `01`–`09` (nine modules) | **70 situations × 10 cases = 700 entries** (enterprise / history / research / cautionary tags); each module trains one management mindset |
| Master file | `00-驭人七十策.md` | The Seventy Practices — four-character classical names, chantable one-liners, paired allusions, editorial notes |
| Case supplements | `11`–`18`, `21`, `22` | **Case material for the 70 rules**, pulled in when a rule is matched — rule-by-rule classical sourcing (Shiji & Zhanguoce), 30 cases from the Zizhi Tongjian, Three Kingdoms (history/novel tagged), Ming / Journey West / Water Margin, figure cases (Drucker / Selected Works / Inamori), manipulation-tactic identification. Case sources, not parallel systems |
| Scripts & boundaries | `10` | Verbatim scripts for 12 scenarios; five value boundaries; the four-question self-check; China labor-law notes |
| Function files | `19` · `20` · `23` · `24` | `19` bilingual index; `20` people×AI mapping; `23` the three-round game trees (15 rules); `24` situation assessment + naming library + six insight techniques |

## What an action card looks like

> "A senior engineer on my team does great work but bad-mouths the team privately."

```
[Scenario] Senior, output stable, high private negativity
[Matched] Rule 32 (back-channel venting) + Rule 26 (root cause: lost sense of value)
[Assessment] Will (belonging), not skill
[Primary] Module 7 · Rule 32: the one-on-one that opens the channel
[Support] Rule 26: send juniors to learn from him
[Steps] 1:1 this week, listen only → give a "needed" role next month → watch the group-chat temperature
[Script] "I hear you have thoughts. Nobody else is here — say it straight. If you're wrong, I'll pretend I didn't hear it; if you're right, I'll change."
[Timeline] Two weeks for temperature, one month for behavior
[Watch-out] Never ask "who told me" — protecting the channel beats knowing the name
[Game tree] Move: the 1:1 → Counter: boilerplate / blame → Chain: switch to concrete questions (a proposal outlet) → Counter: real opinions surface → Chain: land the good ideas publicly, with his name → Counter: he arrives with a list next time. Equilibrium: the venting energy is re-routed — from behind backs to the tabletop
[Cases] Huawei's open forum · Chayan Yuese 2021 (cautionary) · Di Renjie refusing to learn the informer's name
```

## The nine management mindsets

| Module | Mindset | In one line |
|---|---|---|
| 1 Rule-setting | System thinking | Good rules say the hard things for you |
| 2 Paper trails | Transparency | Trust is built on what can be seen |
| 3 Structure moves | Design thinking | Same person, different seat, different result |
| 4 Reality lessons | Growth thinking | Turn setbacks into controlled learning |
| 5 Pacing | Decomposition | Big goals become small steps everyone can climb |
| 6 Lanes & stakes | Motivation | Make people want to win |
| 7 Feedback & safety | Psychological safety | Safety is the foundation of high performance |
| 8 Reporting habits | Structured thinking | Clear speaking is proof of clear thinking |
| 9 Working habits | Process thinking | Turn individual smarts into team process |

## Quick start

```bash
git clone https://github.com/forrestneo/harness-man-skills.git

# Claude Code
cp -r harness-man-skills/skills/harness-man-skills ~/.claude/skills/

# ZCode
cp -r harness-man-skills/skills/harness-man-skills ~/.zcode/skills/

# Codex and other Agent Skills-compatible tools: same idea
```

Then just ask — a specific problem or a vague situation, in Chinese or English.

## Who it's for

- **Managers** with a live problem — get the action card plus the game tree
- **Everyone in the AI era** — the first "subordinate" you manage may well be an agent; all 70 rules work for both
- **Creators** — one practice = one short video; one module = one essay; all seventy = a course; the game trees are ready-made three-act sketches
- **Students of organizations** — 700 catalogued cases across 2,000 years, indexed by situation
- **Users worldwide** — two millennia of Chinese management wisdom (Sima Qian to Drucker), served bilingually

## Repository layout

```
skills/harness-man-skills/
├── SKILL.md                  # The mindset framework: mission → beliefs → assessment → dual entry → action card
└── references/
    ├── 00-驭人七十策.md        # Master file (names / jingles / allusions / notes)
    ├── 01…09-*.md            # Core method library (700 entries, nine mindsets)
    ├── 10-话术与红线.md        # Scripts, value boundaries, labor-law notes
    ├── 11…18, 21, 22-*.md    # Case supplements (pulled in when matched)
    ├── 19-中英索引.md          # Bilingual index
    ├── 20-AI时代管理映射.md    # People×AI mapping
    ├── 23-攻防三回合推演.md     # Full game trees + equilibria
    └── 24-环境评估与降维洞察.md  # Entry B: assessment + naming + insight techniques
```

## Notes & credits

- The original 70-rule list comes from internet folklore; this repo systematizes and expands it rule by rule
- Cases cite sources down to chapter and book; novelistic or invented material is explicitly tagged and never passed off as history
- "Management is the discovery of value" and similar lines are distillations of Drucker's thought, not verbatim quotes
- Nothing here is legal advice — for employment actions, run it past HR and counsel first

## License

[MIT](LICENSE) — use it, remix it, teach it. Attribution appreciated.
