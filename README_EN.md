# Yurenshu · 驭人术

> **The Art of Managing People** — 70 stratagems, 700 cases, and a complete playbook for leading a team. In the spirit of *The Art of War*, but for the wars that happen inside offices. **Works in both Chinese and English**: ask in English, get an English prescription card (see `references/19-中英索引.md` — the bilingual index with the full 70-rule lookup table and English templates).

[中文 README](README.md) · MIT License

---

## What is this

A viral list circulates on the Chinese internet — "This is how bosses actually manage their subordinates: 70 rules" (*攀比 → publish transparent metrics; veteran slacker → rotate the job; perfectionist who never ships → define a minimum deliverable*). It's a great list of mnemonics, and a useless toolkit: you can memorize the rules and still freeze in front of a real person.

This repo turns that list into a complete **diagnose-and-prescribe system**, packaged as an [Agent Skill](https://agentskills.io) for Claude Code, Codex, ZCode, and any tool that supports the Agent Skills format. Describe a people problem, and it returns a prescription card: diagnosis → remedy → three concrete steps → scripts you can copy verbatim → dosage → contraindications → supporting cases.

One line: **most "management tricks" content teaches you slogans. This library teaches you how to write prescriptions.**

## The content matrix

Everything is in Chinese (the source material and the corpus are deeply Chinese — from Sima Qian to Drucker, from *Journey to the West* to Welch). The structure:

| Layer | Files | What's inside |
|---|---|---|
| Master code | `00-驭人七十策.md` | **The Seventy Stratagems** — modeled on *The Thirty-Six Stratagems*: each rule gets a four-character name (e.g. 立木取信 *Erect the Pole to Establish Trust*, 擒贼擒王 *Catch the King First*, 大成若缺 *Great Completion Looks Incomplete*), a chantable one-liner, paired classical allusions (one positive, one cautionary), and an editorial note |
| Case library | `01`–`09` (nine cabinets) | **70 problems × 10 cases = 700 entries**, tagged as 【enterprise】【history】【research】or 【cautionary tale】. Half Chinese (Huawei, Pang Donglai, Haidilao, Records of the Grand Historian), half global (Toyota, Bridgewater, Netflix, Google's Project Aristotle) |
| Scripts & red lines | `10` | Verbatim scripts for 12 common scenarios; five "autopsy report" red lines; a four-question PUA test; China labor-law compliance notes |
| Classical annex | `11` Zizhi Tongjian · `12` Thick Black Theory · `13` Shiji & Zhanguoce | 30 cases from Sima Guang's *Comprehensive Mirror*; Li Zongwu's *Thick Black Theory* treated as pathogen specimens (identified, never prescribed); **rule-by-rule classical sourcing** — every one of the 70 rules matched to a case from the *Records of the Grand Historian* or *Strategies of the Warring States* |
| Fiction annex | `14` Ming dynasty · `15` Three Kingdoms · `16` Journey to the West · `17` Water Margin | Ming officialdom as a full pathology slide of organizational disease; Three Kingdoms tactics & psychology (every case tagged **history / novel / invented / inverted** — cite without fear); the Journey to the West team as the most famous five-person startup; Water Margin as the complete anatomy of organizational failure |
| Theory anchor | `18` Drucker | Thirteen lectures — MBO, staffing to strengths, feedback analysis, knowledge workers — each mapped to a rule and cross-referenced with a classical Chinese case |

## A taste of the cases

Three entries, picked at random:

- **Rule 30 · Accepting every request** → [Shiji] General Li Mu defended the northern frontier by refusing to fight. Every Xiongnu raid, he locked the gates. He was called a coward and replaced — his successor attacked and lost repeatedly. Li Mu returned, still refused to fight, spent years fatting his troops until they *begged* for battle — then destroyed 100,000 Xiongnu cavalry in one engagement. The years he was being called a coward were the resource-assessment phase.
- **Rule 56 · Envy between peers** → [Shiji] With the empire won and everyone scrambling for credit, Zhang Liang's advice to the Emperor: *enfeoff Yong Chi first* — the man Liu Bang hated most. If even Yong Chi got a fief, everyone relaxed. Envy isn't soothed — it's re-anchored.
- **Rule 1 · Constant comparison** → [Journey to the West] The Peach Banquet invitations went out to every god with a name — except the Monkey King. The havoc that followed, the one that reordered Heaven itself, began with a guest list. The hidden mines in an incentive system are never about how much you reward; they're about *who got left off the list*.

## Quick start

```bash
git clone https://github.com/forrestneo/yurenshu.git

# Claude Code
cp -r yurenshu/skills/yurenshu ~/.claude/skills/

# ZCode
cp -r yurenshu/skills/yurenshu ~/.zcode/skills/

# Codex and other Agent Skills-compatible tools: same idea — drop skills/yurenshu into the skills directory
```

Then just ask. Example:

> *A senior engineer on my team does great work but bad-mouths the team privately. How do I handle it?*

The skill returns a prescription card (diagnosis: willingness, not ability → primary remedy: one-on-one within the week → script: "I hear you have thoughts. Nobody else is here — say it straight. If you're wrong, I'll pretend I didn't hear it; if you're right, I'll change." → dosage: two weeks for temperature, one month for behavior → contraindication: never ask "who told me" — burning your source kills the one-on-one channel forever → cases: Huawei's Xinsheng community vs. the 2021 Chayan Yuese WeChat-group meltdown).

## The red lines (what this is NOT)

This library teaches *leading*, not *breaking*. Five hard red lines ship with the library, each backed by a real-world autopsy:

1. **Rotation ≠ exile** — Japan's *oidashi-beya* ("expulsion rooms") lost in court, twice.
2. **Spot checks ≠ surveillance** — auditing deliverables is management; reading someone's screen is invasion.
3. **Public rules ≠ public humiliation** — rules address behavior, in the open; criticism addresses a person, in private.
4. **Breaking up cliques ≠ breeding informants** — restructure, never recruit snitches.
5. **Some conditions have no cure** — value conflicts, integrity violations, honest capability ceilings. Replacing is faster and kinder than reforming.

And the four-question PUA test: *Did this move make him stronger, or more afraid? Did he know the rule in advance? Does he have a channel to appeal? Would I dare explain this move to the whole team?* — Fail one, and it's not management. It's domestication.

## Who it's for

- **Managers** with a specific, live people problem — look up the symptom, get the prescription
- **Creators** writing about management — each stratagem ships with name, jingle, allusion, cases, and contraindication: one stratagem = one short video; one cabinet = one long-form essay; all seventy = a course
- **Students of organizations** — 700 catalogued cases across 2,000 years and a dozen countries, indexed by symptom

## Repository layout

```
skills/yurenshu/
├── SKILL.md                  # The diagnostic framework: 3 questions → 9 cabinets → prescription card
└── references/
    ├── 00-驭人七十策.md        # The Seventy Stratagems (master code)
    ├── 01…09-*.md            # Nine case cabinets (700 entries)
    ├── 10-话术与红线.md        # Scripts, red lines, labor-law notes
    ├── 11…13-*.md            # Zizhi Tongjian / Thick Black Theory / Shiji & Zhanguoce annexes
    ├── 14…17-*.md            # Ming / Three Kingdoms / Journey West / Water Margin annexes
    └── 18-德鲁克.md           # Drucker anchor (East-meets-West cross-references)
```

## Notes & credits

- The original 70-rule list comes from internet folklore; this repo systematizes and expands it rule by rule
- Cases cite sources down to chapter and book; novelistic or invented material is explicitly tagged and never passed off as history
- Nothing here is legal advice — for employment actions, run it past HR and counsel first

## License

[MIT](LICENSE) — use it, remix it, teach it. Attribution appreciated.
