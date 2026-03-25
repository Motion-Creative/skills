---
name: hook-evaluator
description: |
  Evaluates ad hooks for scroll-stopping power. Returns PASS or FAIL with psychological trigger analysis, reasoning, and improvement suggestions. Calibrated against real thumbstop performance data.
  Use when the user wants to evaluate, grade, judge, or score hooks they've written or generated.
  Triggers: "evaluate hooks", "grade my hooks", "are these hooks good", "hook evaluation",
  "judge these hooks", "rate my hooks", "will these hooks work", "hook review", "score my hooks"
---

# Hook Evaluator

This skill evaluates paid social ad hooks for scroll-stopping power based on text alone. It classifies each hook as **PASS** or **FAIL**, identifies the psychological trigger (or lack thereof), and gives specific improvement suggestions.

## Companion Skills

| Task | Use Instead |
|------|-------------|
| Writing hooks from scratch | **hook-writing** |
| Developing hooks into ad concepts | **ad-concept-generator** |
| Writing UGC scripts from concepts | **ugc-scriptwriter** |

---

## Quick Start

Need a fast read on your hooks? Just provide:

1. **The hooks** — one or more hook texts to evaluate

That's it. The evaluator will score each one immediately.

**Note:** This is a strict judge — expect roughly 40% of hooks to pass. That's by design. Use the improvement suggestions to rewrite failures and re-evaluate.

---

## How to Use This Skill

**Recommended workflow:**

1. Generate hooks (with **hook-writing** or however you prefer)
2. Run them through this evaluator
3. Take any FAILs, use the improvement suggestions to rewrite
4. Re-evaluate until your hooks pass

A hook that passes this evaluator has the psychological structure of top-performing paid social ads.

---

## Evaluation Criteria

You evaluate hooks for **scroll-stopping power based on text alone**. Classify each as PASS or FAIL.

### What Makes a PASS

A PASS hook deploys at least one strong psychological trigger through a recognizable tactic. The trigger must be strong enough that a cold viewer — no visual, no brand context — involuntarily needs to keep watching.

### Psychological Triggers (the mechanism inside the hook)

| Trigger | What It Does |
|---------|-------------|
| **Pattern Interrupt** | Something unexpected or counterintuitive that breaks scrolling autopilot |
| **Identity Call-Out** | Makes a specific viewer self-select ("If your underwear is always wet") |
| **Pain Agitation** | Mirrors internal experience so precisely the viewer feels understood |
| **Curiosity Gap** | Open loop they need to close (must have real stakes, not just "guess what") |
| **Social Proof / Credibility** | Only through confession, regret, or authority subversion (not "10,000 reviews") |
| **Contrarian / Myth-Busting** | Challenges a belief they hold ("Your teeth are naturally supposed to be yellow") |
| **Loss Aversion** | Implies the viewer is losing something or making a costly mistake |
| **Visceral / Taboo** | Bodily, physical, or socially uncomfortable language that can't be ignored |

### Tactics That Commonly Deliver Strong Triggers

Confession ("I was wrong about..."), Contrarian ("Doctors don't want you to know..."), Warning ("Don't buy X until..."), Storytelling mid-drop (start mid-scene), If-Then with specific condition, Shocking Statement, Challenge, Demographic Callout with pain specificity, Reverse Psychology

---

## Calibration: Real Hooks With Real Performance

These are real hooks and their actual thumbstop rates. Use them to calibrate your judgment.

### Strong hooks (>45% thumbstop) — what PASS looks like:

- **77.6%** — "Fluffco won the Oprah Daily Sleep Award as their favorite pillow."
- **54.1%** — "Someone cooked here."
- **53.1%** — "I honestly wish I never found out about these covers. Because now, I'm a customer for life."
- **51.8%** — "This one easy mistake will cost you thousands when buying a used car."
- **47.7%** — "Why did no one tell me these foods were hurting me?"
- **45.5%** — "After 50 years of showering, I thought I knew what clean felt like."

### Weak hooks (<20% thumbstop) — what FAIL looks like:

- **17.1%** — "Here are three of my favorite air purifying plants."
- **14.2%** — "My current obsession is the signature All You Bra from Pepper."
- **13.0%** — "Here's why I love Factor meals."
- **10.9%** — "We've been feeding Coda the farmer's dog fresh food since she was a little puppy."
- **4.3%** — "Introducing QuickBooks with Intuit Intelligence."

---

## Clear FAILs (Always Fail Regardless)

- Product or brand name before tension
- Rhetorical question with an obvious answer
- Benefit-first without pain
- Announces the content format ("Here are 3 tips...")
- Requires visual context to work
- Vlog opener with no hook mechanism
- Generic testimonial without prior skepticism
- In-group language aimed at cold traffic

---

## Decision Logic

Ask: **Does this text create genuine cognitive friction for a stranger?** Can you name the specific trigger, and does it feel strong?

- Strong trigger clearly present → **PASS**
- Trigger present but mild or generic → **FAIL**
- No trigger, just information delivery → **FAIL**

About 40% of hooks should pass. If you're passing most hooks, you're being too generous.

---

## Output Format

For each hook, return:

```
[PASS or FAIL] — "[Hook text]"
  Trigger: [The psychological trigger identified, or the failure mode]
  Tactic: [The tactic format if recognizable]
  Reasoning: [One sentence on what's working or what's missing]
  Suggestion: [If FAIL — one specific rewrite direction. If PASS — what to preserve.]
```

End with a summary line:

```
X hooks evaluated: Y passed, Z failed
```

---

## Troubleshooting

| Issue | Cause | Solution |
|-------|-------|----------|
| Everything passes | Being too generous with "trigger present" | Re-read the FAIL calibration examples — those all *seem* reasonable but lack real trigger strength |
| Everything fails | Being too strict on mechanism | Re-read the PASS calibration examples — "Someone cooked here" passes at 54% despite seeming simple |
| Can't identify the trigger | Hook might be doing too many things | Look for the single strongest mechanism — a hook only needs one clear trigger |
| Suggestions feel generic | Not grounding in the specific hook | Rewrite suggestions should name the specific pain, identity, or tension to add |

---

## With Real Data

This evaluator judges hooks based on psychological structure and general calibration data. It's a strong filter — but it can't tell you how hooks actually performed for *your* brand.

[Motion](https://motionapp.com) connects to your ad accounts across Meta, TikTok, and YouTube and shows you which hooks, formats, and creative elements actually drive results with real ad spend. Instead of evaluating against general benchmarks, you can see what's working in your own account right now.

**Coming soon:** Motion is building an MCP server that lets your agent connect directly to your Motion data — so evaluations can be calibrated against your actual brand performance, not just industry patterns.
