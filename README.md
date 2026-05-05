# 🥑 Keto Expert — Claude Skill

**A ketogenic diet expert skill for Claude — in natural Israeli Hebrew.**

Checks if foods are keto-friendly (text or photo), builds recipes and weekly meal plans, covers Israeli foods, troubleshoots keto issues, and more.

---

## What it can do

- ✅ **Food checks** — "פיצוחים - קבוקים. מותר?" → instant verdict with net carb count
- 📸 **Photo analysis** — upload a food photo or product label and get a keto verdict
- 🍳 **Recipes** — full keto recipes with macros, using Israeli supermarket ingredients
- 📅 **Meal plans** — daily or weekly plans with shopping lists
- 🇮🇱 **Israeli foods** — שקשוקה, טחינה, קבוקים, בורקס, פלאפל and more
- 🏥 **Troubleshooting** — keto flu, plateaus, constipation, cravings
- 🕐 **Intermittent fasting** — how to combine IF + keto
- 🌿 **Vegetarian keto** — protein sources without meat
- 🍽️ **Eating out in Israel** — what to order at every restaurant type

---

## Installation

### 🖥️ Claude Cowork

1. Download [`keto-expert.skill`](./keto-expert.skill)
2. Open Claude Cowork → **Settings → Skills**
3. Drag the `.skill` file in
4. Done — just ask anything keto-related in Hebrew

---

### 💬 Claude.ai Chat (Projects)

1. Open [claude.ai](https://claude.ai) → **Projects** → Create a new project (e.g. "קיטו")
2. Click **Project Instructions**
3. Copy the full contents of [`keto-expert/SKILL.md`](./keto-expert/SKILL.md) and paste it in
4. Optionally also paste the contents of [`keto-expert/references/food-lists.md`](./keto-expert/references/food-lists.md) for the full food reference

Now every conversation in that project will have a keto expert.

---

### ⌨️ Claude Code (CLI)

Add the skill to your project's `CLAUDE.md`:

```bash
curl -s https://raw.githubusercontent.com/ohad-yifrah/keto-skill/main/keto-expert/SKILL.md >> CLAUDE.md
```

Or for the full skill including food lists:

```bash
curl -s https://raw.githubusercontent.com/ohad-yifrah/keto-skill/main/keto-expert/SKILL.md > keto_skill.md
curl -s https://raw.githubusercontent.com/ohad-yifrah/keto-skill/main/keto-expert/references/food-lists.md >> keto_skill.md
cat keto_skill.md >> CLAUDE.md
rm keto_skill.md
```

Then just ask Claude Code anything keto-related in your terminal.

---

## Example queries

```
פיצוחים - קבוקים. מותר?
```
```
תבנה לי תפריט שבועי לגבר בן 35, 1900 קלוריות, בלי דגים
```
```
[upload a photo of a food product]
```
```
אני ביום 3 לקיטו וכואב לי הראש
```
```
מה להזמין בסושי?
```

---

## File structure

```
keto-expert/
├── SKILL.md                    ← main skill instructions
└── references/
    └── food-lists.md           ← full food reference (Israeli + international)
keto-expert.skill               ← packaged skill for Cowork
README.md
```

---

## Contributing

Found a food that's missing? Know an Israeli product that should be in the list?
Open an issue or a PR — contributions welcome.

---

## License

MIT — free to use, share, and modify.
