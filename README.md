# fit

A plugin with one skill, `will-fibery-work-for-me`, for the "Is Fibery for me?" flow on fibery.com. A visitor describes their problem; the skill gives a short, honest verdict on whether Fibery fits, and says no when it does not.

## What is inside

```
.claude-plugin/plugin.json                    plugin manifest (name: fit)
skills/will-fibery-work-for-me/SKILL.md       verdict rules, blockers, reply format, examples
skills/will-fibery-work-for-me/references/    facts opened on demand
```

References:

- `hard-limits.md`: compliance, hosting, scale and other limits, with sources
- `pricing.md`: plans, limits, which plan a feature needs, discounts
- `integrations.md`: native integrations, sync direction, other ways to connect a tool
- `proof-points.md`: public customer stories the skill may cite
- `examples.md`: example replies modelled on real pre-sales chats
- `use-cases/`: what paying customers run in Fibery, one file per segment group

## Keeping it current

Facts were checked on 12 November 2026 and carry source links. Re-check `pricing.md` and `hard-limits.md` when plans or product limits change. The `use-cases/` files are generated from customer usage data that lives outside this repo.
