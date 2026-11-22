# Learnings

Corrections, insights, and knowledge gaps captured during development.

**Categories**: correction | insight | knowledge_gap | best_practice
**Areas**: frontend | backend | infra | tests | docs | config
**Statuses**: pending | in_progress | resolved | wont_fix | promoted | promoted_to_skill

## Status Definitions

| Status | Meaning |
|--------|---------|
| `pending` | Not yet addressed |
| `in_progress` | Actively being worked on |
| `resolved` | Issue fixed or knowledge integrated |
| `wont_fix` | Decided not to address (reason in Resolution) |
| `promoted` | Elevated to SOUL.md, TOOLS.md, or AGENTS.md |
| `promoted_to_skill` | Extracted as a reusable skill |

Status is not validation. A fixed incident or repeated observation does not prove a reusable rule. Use Maintenance for scoped evidence and active-guidance disposition; preserve historical observations and earlier reviews. Initialize legacy entries only on relevant review.

## Entry Template

Copy this entry when logging; replace placeholders. Unknown classifications stay unknown until triage. Do not copy an example's validation as evidence.

```markdown
## [LRN-YYYYMMDD-XXX] correction | insight | knowledge_gap | best_practice

**Logged**: ISO-8601 timestamp
**Priority**: low | medium | high | critical
**Status**: pending
**Area**: frontend | backend | infra | tests | docs | config

### Summary
One-line description of what was learned

### Details
What happened, the correction, and the limits of what was observed

### Suggested Action
Specific fix or improvement to make

### Metadata
- Source: conversation | error | user_feedback
- Related Files: path/to/file.ext
- Tags: tag1, tag2
- See Also: related learning ID, if any
- Pattern-Key: area.symptom
- Recurrence-Count: 1
- First-Seen: YYYY-MM-DD
- Last-Seen: YYYY-MM-DD

### Maintenance
- Claim: unknown — identify the reusable inference/instruction during triage
- Scope: unknown
- Authority: unknown
- Decay: unknown / unknown
- Revalidate: before relying on the claim, establish scope/authority and choose the cause-specific check and trigger
- Validation: pending
- Evidence: none yet
- Disposition: retain — provisional, not validated
- Guidance: none

---
```

Choose type (`reality`, `decision`, `dependency`, `relevance`) and rate (`fast`, `medium`, `slow`, `durable`) using the skill's Maintenance instructions, not age/status. Record actual check date, source/version/configuration, and result. Missing/conflicting evidence is `unresolved`. Add dated review notes for retain/revise/externalize/retire; preserve old claims and promotion history. Reviews never increase recurrence counts or Last-Seen.

## Skill Extraction Fields

When a learning is promoted to a skill, add these fields:

```markdown
**Status**: promoted_to_skill
**Skill-Path**: skills/skill-name
```

Only create/modify skill assets with explicit scoped approval. Record the promotion date and target section in the learning's history/Guidance, and the original file + learning ID in the skill. `promoted_to_skill` does not establish current validity.

Example:
```markdown
## [LRN-20250115-001] best_practice

**Logged**: 2025-01-15T10:00:00Z
**Priority**: high
**Status**: promoted_to_skill
**Skill-Path**: skills/docker-m1-fixes
**Area**: infra

### Summary
Docker build fails on Apple Silicon due to platform mismatch
...
```

---

## [LRN-20261122-001] correction

家长反馈数学综合练习 01 偏浅，接近三四年级水平。后续常规卷维持五年级中等目标，增加需要自己确定数量关系、逆推和说明理由的题。当前反馈已写入出题偏好；具体难度随学校样卷和学生作答再校准。

## [LRN-20261122-002] correction

第4题把正向平均题改成逆推与解释。家长转述孩子很少接触；已依据实卷05改回给总量求平均，并逐问校准其余题目。

## [LRN-20261122-003] correction

完整数学卷优先从个人错题选材，保留学校已学解题结构，只小改情境、数字或条件，附错题编号对照。已同步至出题偏好。
