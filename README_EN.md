# Yurenshu · 驭人术

> **The Art of Managing People — for everyone in the AI era.** A positive, practical management-development system: 70 real workplace situations, 700 cases, nine management mindsets. Helps you grow people, grow teams, and grow yourself — and manage AI agents too, because **in the AI era, everyone is a manager**. Works in both Chinese and English (`references/19-中英索引.md`).

[中文 README](README.md) · MIT License

---

## The mission: everyone is a manager now

For most of history, most people never managed anyone — management was a skill for the few. The AI era changes that: **everyone now manages intelligent agents.** Management is no longer an elective for leaders; it is basic literacy for everyone.

This library serves both: **learning to manage people is learning to manage AI agents.** Aligning goals, decomposing tasks, accepting deliverables, iterating on feedback, orchestrating collaboration — the five core management moves are identical for human teammates and AI agents (see `references/20-AI时代管理映射.md` for the 20-move mapping: written requirements → the prompt trio; break-it-down → task decomposition; a brick for jade → few-shot examples; glad-to-hear-faults → rewarding an AI that says "I'm not sure"). Never managed anyone? Start with AI — it's a zero-cost practice field for management.

## What is this

A viral list circulates on the Chinese internet — "This is how good bosses actually manage: 70 rules" (*chronic comparison → publish transparent metrics; veteran slacker → rotate the job; perfectionist who never ships → define a minimum deliverable*). It's a great list of mnemonics, and a hard-to-use toolkit: you can memorize the rules and still freeze in front of a real person.

This repo turns that list into a complete **management-development system**, packaged as an [Agent Skill](https://agentskills.io) for Claude Code, Codex, ZCode, and any tool that supports the Agent Skills format. Describe a people problem, and it returns an action card: assessment → method → three concrete steps → scripts you can copy verbatim → timeline → watch-outs → supporting cases.

One line: **most "management tips" content teaches you slogans. This library builds your management thinking.**

The value proposition traces to Drucker: **management is the discovery of value** — the 70 so-called "problems" are 70 misplaced values (chronic comparison = competitive drive; the "troublemaker" = conviction; the "veteran slacker" = organizational memory). The library ships a "value-discovery lens" table: find the value first, then apply the method.

## What we believe

- **Control earns compliance; growth earns followership.** This library teaches the ability to grow people, not tricks to control them.
- **Good management lets ordinary people achieve extraordinary things** (Drucker). Every method answers one question: how do I help this person get better at this thing?
- **Boundaries before methods.** Five value boundaries ship ahead of every technique (rotation ≠ exile; audits ≠ surveillance; rules public, feedback private; never optimize through informants; sometimes an amicable parting is kinder than forced reform). A four-question self-check keeps every move on the right side of the line — this library teaches management, never manipulation.
- **Half Chinese, half global — by design.** 700 cases split between East and West: Huawei and Pang Donglai alongside Toyota and Bridgewater; the *Records of the Grand Historian* alongside Google's Project Aristotle; Drucker alongside the *Zizhi Tongjian*.

## The content matrix

| Layer | Files | What's inside |
|---|---|---|
| Master file | `00-驭人七十策.md` | **The Seventy Practices** — each rule gets a four-character classical name, a chantable one-liner, paired classical allusions (one positive, one cautionary), and an editorial note. The format echoes classical Chinese compendia, but every entry lands on a modern management problem |
| Method library | `01`–`09` (nine modules) | **70 situations × 10 cases = 700 entries**, tagged 【enterprise】【history】【research】【cautionary】. Each module trains one management mindset: system thinking, transparency, growth thinking, pacing, motivation, psychological safety, structured communication, process thinking |
| Scripts & boundaries | `10` | Verbatim scripts for 12 common scenarios; five value boundaries; the four-question self-check; China labor-law compliance notes |
| Classical annex | `11` Zizhi Tongjian · `12` Thick Black Theory · `13` Shiji & Zhanguoce | 30 cases from Sima Guang's *Comprehensive Mirror*; manipulation tactics as identification-only specimens (learn to spot them, never to use them); **rule-by-rule classical sourcing** from the *Records of the Grand Historian* and *Strategies of the Warring States* |
| Fiction annex | `14` Ming dynasty · `15` Three Kingdoms · `16` Journey to the West · `17` Water Margin | Ming officialdom as a full panorama of organizational lessons; Three Kingdoms persuasion & psychology (every case tagged **history / novel / invented / inverted**); the Journey to the West team as the most famous five-person startup; Water Margin as the complete anatomy of organizational failure |
| Theory anchor | `18` Drucker | Thirteen lectures — MBO, staffing to strengths, feedback analysis, knowledge workers — each mapped to a rule and cross-referenced with a classical Chinese case |
| Bilingual index | `19-中英索引.md` | The 70-rule CN/EN lookup table, English versions of the principles and diagnostic questions, English action-card template, citation norms |
| AI-era mission | `20-AI时代管理映射.md` | **Everyone is a manager now**: the 20-move mapping between managing people and managing AI agents, three AI-only insights, and a growth path from managing AI to managing people |
| Heart-led management | `22-稻盛和夫.md` | Kazuo Inamori's complete system: the success equation (mindset can be negative!), amoeba management, the three-type flammability model, glass-clear transparency, the six endeavors, the 424-day JAL turnaround, five counter-recession moves — Drucker shows how to do things right; Inamori shows how to set people on fire |
| Organizational practice | `21-毛选管理智慧.md` | From the Selected Works: how a few dozen people scaled to organizing a nation — the twelve work methods for leadership committees (each mapped to a rule), contradiction analysis, the mass line, cadre policy, the Sanwan reorganization, protracted-war pacing, plus the business legacy (Huawei, Shi Yuzhu, Wahaha, Alibaba's HR system) |

## A taste of the cases

Three entries, picked at random:

- **Rule 30 · Accepting every request** → [Shiji] General Li Mu defended the northern frontier by refusing to fight. Every Xiongnu raid, he locked the gates. He was called a coward and replaced — his successor attacked and lost repeatedly. Li Mu returned, still refused to fight, spent years training and rewarding his troops until they *begged* for battle — then won decisively. The years he was being called a coward were the resource-assessment phase.
- **Rule 56 · Envy between peers** → [Shiji] With the empire won and everyone scrambling for credit, Zhang Liang's advice to the Emperor: *enfeoff Yong Chi first* — the man Liu Bang disliked most. If even Yong Chi got a fief, everyone relaxed. Envy isn't soothed — it's re-anchored.
- **Rule 1 · Constant comparison** → [Journey to the West] The Peach Banquet invitations went out to every god with a name — except the Monkey King. The havoc that followed began with a guest list. The hidden risks in an incentive system are never about how much you reward; they're about *who got left off the list*.

## Quick start

```bash
git clone https://github.com/forrestneo/yurenshu.git

# Claude Code
cp -r yurenshu/skills/yurenshu ~/.claude/skills/

# ZCode
cp -r yurenshu/skills/yurenshu ~/.zcode/skills/

# Codex and other Agent Skills-compatible tools: same idea — drop skills/yurenshu into the skills directory
```

Then just ask, in Chinese or English. Example:

> *A senior engineer on my team does great work but bad-mouths the team privately. How do I handle it?*

The skill returns an action card: assessment (willingness and morale, not ability) → primary method (Rule 32: the one-on-one that opens the channel and draws the line) → three steps → a script you can use ("I hear you have thoughts. Nobody else is here — say it straight. If you're wrong, I'll pretend I didn't hear it; if you're right, I'll change.") → timeline (two weeks for temperature, a month for behavior) → watch-out (never ask "who told me" — protecting the channel matters more than knowing the name) → cases (Huawei's open forum as the positive pattern, the 2021 Chayan Yuese group-chat meltdown as the cautionary one).

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

## Who it's for

- **Managers** with a specific, live people problem — look up the situation, get the action card
- **Everyone in the AI era** — the first "subordinate" you manage may well be an AI agent; all 70 methods work for both, and managing AI is a zero-cost practice field
- **Creators** writing about management — each practice ships with name, jingle, allusion, cases, and watch-out: one practice = one short video; one module = one long-form essay; all seventy = a course
- **Students of organizations** — 700 catalogued cases across 2,000 years and a dozen countries, indexed by situation
- **Users worldwide** — two millennia of Chinese management wisdom (from Sima Qian to Drucker), served bilingually

## Repository layout

```
skills/yurenshu/
├── SKILL.md                  # The mindset-training framework: beliefs → 3 questions → 9 modules → action card
└── references/
    ├── 00-驭人七十策.md        # The Seventy Practices (master file)
    ├── 01…09-*.md            # Nine method modules (700 entries)
    ├── 10-话术与红线.md        # Scripts, value boundaries, labor-law notes
    ├── 11…13-*.md            # Zizhi Tongjian / Thick Black Theory / Shiji & Zhanguoce annexes
    ├── 14…17-*.md            # Ming / Three Kingdoms / Journey West / Water Margin annexes
    ├── 18-德鲁克.md           # Drucker anchor (East-meets-West cross-references)
    ├── 19-中英索引.md          # Bilingual index (EN lookup table & templates)
    ├── 20-AI时代管理映射.md      # Everyone is a manager: people×AI mapping
    ├── 21-毛选管理智慧.md        # Organizational practice from the Selected Works
    └── 22-稻盛和夫.md            # Heart-led management: equation + amoeba + JAL
```

## Notes & credits

- The original 70-rule list comes from internet folklore; this repo systematizes and expands it rule by rule
- Cases cite sources down to chapter and book; novelistic or invented material is explicitly tagged and never passed off as history
- Nothing here is legal advice — for employment actions, run it past HR and counsel first

## License

[MIT](LICENSE) — use it, remix it, teach it. Attribution appreciated.
